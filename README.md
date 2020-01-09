
<!DOCTYPE HTML>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Formulaire</title>
        <link rel="stylesheet" href="formulaire.css">
    </head>
<body>
    <form method="get">
        <label for="pseudo">Pseudo*</label>
        <input id="pseudo" type="text" name="pseudo" required placeholder="Pseudo">
        <hr>
        <label for="MOT DE PASSE">Mot de passe</label>
        <input type="password" name="mdp" id="motdepasse" required>
        <hr>
        <label for="Email">Votre Email</label>
        <input type="email" id="email" name="email">
        <hr>
        <label for="pays">Pays</label>
        <select id="pays" name="pays" required title="Choix de pays">
            <option disabled selected>Votre Pays</option>

            <optgroup label="Europe">
                <option value="fr">France</option>
                <option value="pl">Portugal</option>
                <option value="gr">Grece</option>
            </optgroup>
            <optgroup label="Asie">
                    <option>Chine</option>
                    <option>Vietnam</option>
                    <option>Japon</option>
                    <option>Malaisie</option>
                </optgroup>
            <optgroup label="Amérique">
                </option value="fr">USA</option>
                <option value="es">Brazil</option>
                <option value="gp">Argentine</option>
                <option value="it">Mexique</option>
                <option value="it">Guadeloupe</option>
            </optgroup>    
        </select>
        <hr>
        <label>Quels sont vos fruits préférés ?</label>
        <input type="checkbox" name="choix">Orange
        <input type="checkbox" name="choix">Frambroise
        <input type="checkbox" name="choix">Fraise
        <hr>
        <label>Civilité</label>
        <input type="radio" name="civilite" value="f">Femme
        <input type="radio" name="civilite" value="h">Homme
        <input type="radio" name="civilité" value="m">Mademoiselle
        <hr>
        <label for="adresse">Votre adresse</label>
     
        <textarea id="adresse" name="adresse" rows="10" cols="25"></textarea>
        <hr>
        <label for="ville">Ville</label>
        <input type="text" id="ville" name="ville" list="France">
        <datalist id="France">
            <option>Paris</option>
            <option>Nice</option>
            <option>Marseille</option>
            <option>Lyon</option>
        </datalist>
        <hr>
        <label for="cp">Code Postal</label>
        <input type="text" id="cp" name="cp" maxlength="5" pattern="[0-9]{5}"> 
        <!-- injput submit : qui valide le formulaire-->
        <input type="submit" value="Inscription" name="inscription">
        <hr>
        <section>
                <h2>Informations de paiement</h2>
                <p>
                  <label for="card">
                    <span>Type de carte :</span>
                  </label>
                  <select id="card" name="usercard">
                    <option value="visa">Visa</option>
                    <option value="mc">Mastercard</option>
                    <option value="amex">American Express</option>
                  </select>
                </p>
                <p>
                  <label for="number">
                    <span>Numéro de carte :</span>
                    <strong><abbr title="required">*</abbr></strong>
                  </label>
                  <input type="text" id="number" name="cardnumber">
                </p>
                <p>
                  <label for="date">
                    <span>Validité :</span>
                    <strong><abbr title="required">*</abbr></strong>
                    <em>format mm/aa</em>
                  </label>
                  <input type="text" id="date" name="expiration">
                </p>
            </section>
      
    </form>
</body>
</html>
