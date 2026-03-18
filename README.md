# lab4

<img width="835" height="437" alt="Capture d&#39;écran 2026-03-18 002940" src="https://github.com/user-attachments/assets/508f6979-0822-4f62-9fe0-c15cee409333" />
Ce screenshot montre l’ouverture de l’application UnCrackable-Level1.apk dans l’outil JADX-GUI.
JADX permet de décompiler une application Android afin d’obtenir un code Java lisible à partir du fichier classes.dex.
Dans la partie centrale, le code de la classe sg.vantagepoint.a.a est affiché.
Cette classe contient une fonction de déchiffrement AES qui sera utilisée plus tard pour vérifier la clé.


<img width="833" height="459" alt="Capture d&#39;écran 2026-03-18 002544" src="https://github.com/user-attachments/assets/a51ca8b4-3dc4-46e6-9c29-2ec243414ee0" />

<img width="830" height="458" alt="Capture d&#39;écran 2026-03-18 002947" src="https://github.com/user-attachments/assets/01d58320-97b2-4863-904c-b45696a733ab" />

Ce code contient la fonction utilisée pour déchiffrer les données avec AES.
Les étapes sont :
Création d’une clé secrète avec : SecretKeySpec
Initialisation du chiffrement : Cipher.getInstance("AES")
Initialisation du mode décryption (mode 2).
Déchiffrement avec : cipher.doFinal()
Cette fonction retourne les données déchiffrées qui contiennent la vraie clé.

<img width="832" height="437" alt="Capture d&#39;écran 2026-03-18 003000" src="https://github.com/user-attachments/assets/7810f2cf-6331-4a2e-969f-9685050216bf" />

ici on a regrouper le code afin de déchifrer la clé.

<img width="817" height="106" alt="Capture d&#39;écran 2026-03-18 003011" src="https://github.com/user-attachments/assets/942bf71c-ca10-44d8-8a59-365e360842c5" />

résultats; la clé chiffré est "I want to believe";
