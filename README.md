# lab-9-

Lab_9_MobileSecurity
Objectif
Examiner rapidement une application Android vulnérable en utilisant Drozer.



Étape 2 – Connexion depuis le PC
drozer console connect
Vérifiez la connexion :dz> device
Listez les modules :dz> list
Affichez la version Android :dz> run information.device
Console Drozer connectée

Étape 3 – Cartographie des composants exposés


- Résumez dans le tableau :

| Type      | Nom                 | Exporté | Protection |
|-----------|--------------------|---------|------------|
| Activity  | LoginActivity      | Oui     | Aucun      |
| Activity  | UserProfileActivity| Oui     | Permission |
| Service   | DataSyncService    | Oui     | Aucun      |
| Receiver  | BootReceiver       | Oui     | Aucun      |
| Provider  | UserDataProvider   | Oui     | Lecture/Écriture |

![Cartographie des composants](screenshots/Screenshot%202026-05-25%20163914.png)

---

## Étape 4 – Vérifier les protections

![Analyse des protections](screenshots/Screenshot%202026-05-25%20163931.png)

---

## Étape 5 – Rassembler les preuves
Créez la structure :
preuves/ activities/ services/ receivers/ providers/ manifest/

Enregistrez les listes, les tableaux et les captures d’écran.

