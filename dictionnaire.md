### Fonctions JavaScript

#### Les plus utilisées

1. **Pour afficher quelque chose dans la console.**
   ```javascript
   console.log(value);
   ```

2. **Pour obtenir l'élément avec un ID spécifique.**
   ```javascript
   document.getElementById('id');
   ```

3. **Pour obtenir les éléments avec une classe spécifique.**
   ```javascript
   document.getElementsByClassName('class');
   ```

4. **Pour obtenir les éléments avec un nom de balise spécifique.**
   ```javascript
   document.getElementsByTagName('tag');
   ```

5. **Pour sélectionner un élément avec un sélecteur CSS.**
   ```javascript
   document.querySelector('selector');
   ```

6. **Pour sélectionner tous les éléments avec un sélecteur CSS.**
   ```javascript
   document.querySelectorAll('selector');
   ```

7. **Pour ajouter un écouteur d'événement à un élément.**
   ```javascript
   element.addEventListener('event', callback);
   ```

8. **Pour supprimer un écouteur d'événement d'un élément.**
   ```javascript
   element.removeEventListener('event', callback);
   ```

9. **Pour créer un nouvel élément.**
   ```javascript
   document.createElement('tag');
   ```

10. **Pour ajouter un enfant à un élément.**
    ```javascript
    parent.appendChild(child);
    ```

11. **Pour supprimer un enfant d'un élément.**
    ```javascript
    parent.removeChild(child);
    ```

12. **Pour définir le contenu HTML d'un élément.**
    ```javascript
    element.innerHTML = 'content';
    ```

13. **Pour obtenir ou définir le texte d'un élément.**
    ```javascript
    element.innerText = 'text';
    ```

14. **Pour définir ou obtenir la valeur d'un attribut d'un élément.**
    ```javascript
    element.setAttribute('attribute', 'value');
    element.getAttribute('attribute');
    ```

15. **Pour supprimer un attribut d'un élément.**
    ```javascript
    element.removeAttribute('attribute');
    ```

16. **Pour vérifier si un élément contient une classe.**
    ```javascript
    element.classList.contains('class');
    ```

17. **Pour ajouter une classe à un élément.**
    ```javascript
    element.classList.add('class');
    ```

18. **Pour supprimer une classe d'un élément.**
    ```javascript
    element.classList.remove('class');
    ```

19. **Pour basculer une classe sur un élément.**
    ```javascript
    element.classList.toggle('class');
    ```

20. **Pour définir un délai d'exécution.**
    ```javascript
    setTimeout(callback, milliseconds);
    ```

21. **Pour définir un intervalle d'exécution.**
    ```javascript
    setInterval(callback, milliseconds);
    ```

22. **Pour annuler un délai.**
    ```javascript
    clearTimeout(timeoutID);
    ```

23. **Pour annuler un intervalle.**
    ```javascript
    clearInterval(intervalID);
    ```

24. **Pour récupérer ou définir la valeur d'un élément de formulaire.**
    ```javascript
    element.value = 'value';
    ```

25. **Pour rediriger vers une nouvelle URL.**
    ```javascript
    window.location.href = 'url';
    ```

26. **Pour recharger la page actuelle.**
    ```javascript
    window.location.reload();
    ```

27. **Pour obtenir la largeur et la hauteur de la fenêtre.**
    ```javascript
    window.innerWidth;
    window.innerHeight;
    ```

28. **Pour obtenir la largeur et la hauteur d'un élément.**
    ```javascript
    element.offsetWidth;
    element.offsetHeight;
    ```

29. **Pour empêcher le comportement par défaut d'un événement.**
    ```javascript
    event.preventDefault();
    ```

30. **Pour arrêter la propagation d'un événement.**
    ```javascript
    event.stopPropagation();
    ```

31. **Pour vérifier si une variable est un tableau.**
    ```javascript
    Array.isArray(variable);
    ```

32. **Pour créer une nouvelle instance de Date.**
    ```javascript
    new Date();
    ```

33. **Pour obtenir la date et l'heure actuelles en millisecondes.**
    ```javascript
    Date.now();
    ```

34. **Pour convertir une chaîne en nombre entier.**
    ```javascript
    parseInt(string);
    ```

35. **Pour convertir une chaîne en nombre flottant.**
    ```javascript
    parseFloat(string);
    ```

36. **Pour convertir une valeur en chaîne JSON.**
    ```javascript
    JSON.stringify(value);
    ```

37. **Pour convertir une chaîne JSON en objet.**
    ```javascript
    JSON.parse(string);
    ```

38. **Pour vérifier si une variable est définie.**
    ```javascript
    typeof variable !== 'undefined';
    ```

39. **Pour vérifier si une variable est null.**
    ```javascript
    variable === null;
    ```

40. **Pour obtenir un sous-tableau à partir d'un index de début et de fin.**
    ```javascript
    array.slice(start, end);
    ```

41. **Pour ajouter un ou plusieurs éléments à la fin d'un tableau.**
    ```javascript
    array.push(element1, ..., elementN);
    ```

42. **Pour ajouter un ou plusieurs éléments au début d'un tableau.**
    ```javascript
    array.unshift(element1, ..., elementN);
    ```

43. **Pour supprimer et retourner le dernier élément d'un tableau.**
    ```javascript
    array.pop();
    ```

44. **Pour supprimer et retourner le premier élément d'un tableau.**
    ```javascript
    array.shift();
    ```

45. **Pour trier un tableau.**
    ```javascript
    array.sort();
    ```

46. **Pour renverser l'ordre des éléments d'un tableau.**
    ```javascript
    array.reverse();
    ```

47. **Pour vérifier si un tableau contient un élément.**
    ```javascript
    array.includes(element);
    ```

48. **Pour fusionner deux ou plusieurs tableaux.**
    ```javascript
    array1.concat(array2, ..., arrayN);
    ```

49. **Pour itérer sur chaque élément d'un tableau.**
    ```javascript
    array.forEach(callback);
    ```

50. **Pour transformer chaque élément d'un tableau et retourner un nouveau tableau.**
    ```javascript
    array.map(callback);
    ```

51. **Pour filtrer les éléments d'un tableau et retourner un nouveau tableau.**
    ```javascript
    array.filter(callback);
    ```

52. **Pour réduire un tableau à une seule valeur.**
    ```javascript
    array.reduce(callback, initialValue);
    ```

53. **Pour vérifier si tous les éléments d'un tableau satisfont une condition.**
    ```javascript
    array.every(callback);
    ```

54. **Pour vérifier si au moins un élément d'un tableau satisfait une condition.**
    ```javascript
    array.some(callback);
    ```

55. **Pour trouver le premier élément d'un tableau qui satisfait une condition.**
    ```javascript
    array.find(callback);
    ```

56. **Pour trouver l'index du premier élément d'un tableau qui satisfait une condition.**
    ```javascript
    array.findIndex(callback);
    ```

57. **Pour vérifier si une chaîne contient une sous-chaîne.**
    ```javascript
    string.includes(substring);
    ```

58. **Pour diviser une chaîne en un tableau de sous-chaînes.**
    ```javascript
    string.split(separator);
    ```

59. **Pour joindre tous les éléments d'un tableau en une chaîne.**
    ```javascript
    array.join(separator);
    ```

60. **Pour supprimer les espaces au début et à la fin d'une chaîne.**
    ```javascript
    string.trim();
    ```

#### Moins utilisées

61. **Pour répéter une chaîne un certain nombre de fois.**
    ```javascript
    string.repeat(count);
    ```

62. **Pour obtenir la valeur absolue d'un nombre.**
    ```javascript
    Math.abs(number);
    ```

63. **Pour obtenir la valeur maximale d'un ensemble de nombres.**
    ```javascript
    Math.max(value1, value2, ..., valueN);
    ```

64. **Pour obtenir la valeur minimale d'un ensemble de nombres.**
    ```javascript
    Math.min(value1, value2, ..., valueN);
    ```

65. **Pour arrondir un nombre au nombre entier le plus proche.**
    ```javascript
    Math.round(number);
    ```

66. **Pour arrondir un nombre à l'entier inférieur le plus proche.**
    ```javascript
    Math.floor(number);
    ```

67. **Pour arrondir un nombre à l'entier supérieur le plus proche.**
    ```javascript
    Math.ceil(number);
    ```

68. **Pour obtenir un nombre aléatoire entre 0 (inclus) et 1 (exclus).**
    ```javascript
    Math.random();
    ```

69. **Pour élever un nombre à une certaine puissance.**
    ```javascript
    Math.pow(base, exponent);
    ```

70. **Pour calculer la racine carrée d'un nombre.**
    ```javascript
    Math.sqrt(number);
    ```

71. **Pour obtenir le logarithme naturel d'un nombre.**
    ```javascript
    Math.log(number);
    ```

