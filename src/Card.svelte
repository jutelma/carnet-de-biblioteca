<script>
    function showInformation(fullUserName) {

        var nom = "";
        var cognoms = "";
        fullUserName = fullUserName.trim();
        var words = fullUserName.split("");
        nom = words [0];

        if (words.length > 1) {
            cognoms = words.slice(1).join("");
        }

        return {
            nom: nom,
            cognoms: cognoms
        };
    }

    var fullUserName = "Pepa Fuentes Martinez";
    var result = showInformation(fullUserName);

    console.log("nom: " + result.nom);
    console.log("cognoms: " + result.cognoms);

</script>

<div>
    <p>Nom: </p>
    <p>Conoms: </p>
</div>

<div>
    <p>Nom: </p>
    <p>Congnoms</p>
</div>

<style>
    div {
        margin: 45px;
        padding:45px;
        border: 2px solid gold;
        text-align: center;
        margin-left: 225px;
        display: table;

    }
</style>

