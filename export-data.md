// Fonction pour convertir un tableau d'objets en CSV et télécharger automatiquement le fichier
function exportToCSV(data, filename = 'data.csv') {
    // Convertit chaque objet en une ligne CSV, en entourant les valeurs de guillemets pour éviter les erreurs avec des virgules dans les valeurs
    const csvData = data.map(row => 
        Object.values(row).map(value => `"${value}"`).join(',')
    );

    // Crée le contenu CSV avec un en-tête (les clés des objets) suivi des données
    const csvContent = `data:text/csv;charset=utf-8,${[Object.keys(data[0]).join(','), ...csvData].join('\n')}`;

    // Crée un lien de téléchargement et déclenche automatiquement le téléchargement
    const link = document.createElement('a');
    link.href = encodeURI(csvContent);
    link.download = filename;
    link.click();
}

Explication de chaque étape :

1. Map sur les objets : csvData est créé en convertissant chaque objet en une ligne CSV.


2. Prépare le contenu du CSV : Ajoute une ligne d’en-tête avec les clés et combine les lignes en une seule chaîne.


3. Lien de téléchargement automatique : Crée un lien invisible et déclenche le téléchargement.




---

// Fonction pour convertir un tableau d'objets en fichier Excel et télécharger automatiquement le fichier
function exportToExcel(data, filename = 'data.xlsx') {
    // Convertit les données en une feuille de calcul avec `json_to_sheet` de la bibliothèque XLSX
    const worksheet = XLSX.utils.json_to_sheet(data);

    // Crée un nouveau classeur (workbook) et ajoute la feuille de calcul à ce classeur
    const workbook = XLSX.utils.book_new();
    XLSX.utils.book_append_sheet(workbook, worksheet, 'Sheet1');

    // Génère et télécharge le fichier Excel
    XLSX.writeFile(workbook, filename);
}

Explication de chaque étape :

1. Conversion en feuille Excel : Utilise json_to_sheet pour transformer le tableau d'objets en une feuille de calcul Excel.


2. Création du classeur : Un nouveau classeur est créé et la feuille de calcul y est ajoutée.


3. Téléchargement du fichier : La fonction writeFile enregistre et télécharge le fichier.




---

// Fonction pour convertir un tableau d'objets en fichier PDF et télécharger automatiquement le fichier
function exportToPDF(data, filename = 'data.pdf') {
    // Initialisation de jsPDF pour créer un document PDF
    const { jsPDF } = window.jspdf;
    const doc = new jsPDF();

    // Position de départ sur l'axe Y
    let yPos = 10;

    // Ajoute chaque ligne de données dans le PDF
    data.forEach((row, index) => {
        // Ajoute chaque valeur de l'objet sur une même ligne, avec un espacement horizontal (50px)
        Object.values(row).forEach((value, i) => {
            doc.text(`${value}`, 10 + (i * 50), yPos);
        });
        // Déplace vers le bas pour la prochaine ligne
        yPos += 10;
    });

    // Génère et télécharge le fichier PDF
    doc.save(filename);
}

Explication de chaque étape :

1. Initialisation du document PDF : Crée un nouvel objet PDF.


2. Ajout de chaque ligne de données : Pour chaque objet du tableau, les valeurs sont ajoutées au document à la position (x, y).


3. Téléchargement du fichier PDF : save génère le PDF et déclenche le téléchargement.




---

Exemple d'utilisation de toutes les fonctions

// Exemple de données à exporter
const data = [
    { name: "Alice", age: 25, city: "Paris" },
    { name: "Bob", age: 30, city: "London" },
    { name: "Charlie", age: 35, city: "New York" }
];

// Exécution de chaque fonction pour télécharger les données dans les formats souhaités
exportToCSV(data);
exportToExcel(data);
exportToPDF(data);

Ces fonctions permettent de convertir un tableau d'objets dans les formats CSV, Excel, et PDF et de télécharger automatiquement les fichiers sans intervention supplémentaire.

