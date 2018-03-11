method
sort()//alphabetique







UTILISATION DU SORT AVEC PARAMETRE
var myArray = [3, 1, 5, 10, 4, 2];
myArray.sort(function(a, b) {
    if (a < b) {
        return -1;
    } else if (a > b) {
        return 1;
    } else {
        return 0;
    }
});
alert(myArray); // Affiche : 1,2,3,4,5,10






indexOf();
lastIndexOf();
reverse();






myArray.forEach(function(value, index, array) {
    alert(
        'Index : ' + index + '\n' +
        'Valeur : ' + value
    );
});





concat()
pour tester egalitE il faut passer par une variable 
slice() = substring
splice() efacer une partie  index d commencement et nombre d valeur a effacer
Array.isArray();





les piles et files


