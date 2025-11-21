# Verus_html
Cybersécurité 
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CyberGuardian</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>CyberGuardian</h1>
            <p>Le bouclier invisible de votre monde numérique</p>
        </div>
    </header>

    <main>
        <div class="container">
            <!-- Section Simulation d'Attaque -->
            <section class="card">
                <h2>Simuler une attaque</h2>
                <p>Choisissez un type d'attaque pour voir son impact :</p>
                <select id="attackType">
                    <option value="phishing">Phishing</option>
                    <option value="malware">Malware</option>
                    <option value="ransomware">Ransomware</option>
                </select>
                <button onclick="simulateAttack()">Lancer l'attaque</button>
                <div id="attackResult" class="result"></div>
            </section>

            <!-- Section Défense -->
            <section class="card">
                <h2>Module de défense</h2>
                <p>Activez les protections pour renforcer votre sécurité :</p>
                <label><input type="checkbox" id="strongPassword"> Mot de passe fort</label>
                <label><input type="checkbox" id="twoFactor"> Authentification à deux facteurs</label>
                <label><input type="checkbox" id="updateSoftware"> Mise à jour logicielle</label>
                <button onclick="checkDefense()">Tester la défense</button>
                <div id="defenseResult" class="result"></div>
            </section>

            <!-- Dashboard -->
            <section class="card">
                <h2>Dashboard de sécurité</h2>
                <div class="dashboard">
                    <div class="meter">
                        <div id="securityMeter" class="fill"></div>
                    </div>
                    <p>Niveau de sécurité : <span id="securityLevel">50%</span></p>
                </div>
            </section>
        </div>
    </main>

    <footer>
        <p>© 2025 CyberGuardian. Tous droits réservés.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
