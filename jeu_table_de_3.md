var saisie = -1;
var nbTentatives = 0;


while ((saisie % 3 !== 0) && (nbTentatives < 5)) {
    nbTentatives++;
    saisie = Number(prompt("Entrez un chiffre multiple de 3 entre 100 et 200 : "));
    
    if (saisie < 100) {
        alert("Le nombre saisi est inférieur à 100 !");
    }
    
    else if (saisie > 200) {
        alert("Le nombre saisi est supérieur à 200 !");
    }
}

if (saisie % 3 === 0) {
    alert("Bravo, le nombre saisi est bien un multiple de 3 ! Vous avez trouvé en " + nbTentatives + " essai(s)");
}
else {
    alert("Perdu !");
}