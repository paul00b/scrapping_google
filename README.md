# Scrappe donc moi tout ça

Projet scrapping de mairie et bot twitter par Théo Duranti, Maxime Elkael, Marianne Chaumeil, Du Halgouet Melec, Paul Broussolle et Anis Bougrab

### Spreadsheet link
<a href="https://docs.google.com/spreadsheets/d/1N7--OE8i6xGaAO2AA8cxe9Ry1xm2GSdGULdlyJL7-iE/edit?usp=sharing"> C'est par ici pour voir la spreadsheet google ;) </a>

### IMPORTANT

Le bot twitter fonctionne parfaitement, mais étant donné qu'il y a beaucoup de requêtes, twitter bloque la connexion :( :(
Preuve d'envoie des mails en photo <a href= "https://drive.google.com/file/d/10SOpUL7pVn9H74gopYpmMje9aJF7_N65/view?usp=sharing">91 pages, 1116 Emails :D </a>
### What's the point ?

This programm is taking all the e-mails from all the townhall of 3 departement in France, and send them a message. Then, it follows all the townhall on their twitter acount. Isn't it wonderful ? (Si ça l'est)

### Installing

Use bundle install to install all of the dependencies.
```
bundle install

```
This programm require the following gems :
```
twitter ==> For the twitter bot
google_drive ==> To store all the e-mail on a beautiful spreadsheet
Gmail ==> To send the message to every towns
```
### How to use ? ###
- Changer les identifiants google mail dans le fichier <b>get_mail_and_city</b>
- Modifier le <b>config.json</b> pour connecter son API Google Drive
- Modifier <b>BotTwitter.rb</b>  pour rentrer ses clefs d'API Twitter
### What have we done ?

1116 Townhall have received the following e-mail : <br>
<br>
Bonjour, <br>
Je m'appelle Hugo, je suis élève à The Hacking Project, une formation au code gratuite, sans locaux, sans sélection, sans restriction géographique. La pédagogie de notre école est celle du peer-learning, où nous travaillons par petits groupes sur des projets concrets qui font apprendre le code. Le projet du jour est d'envoyer (avec du codage) des emails aux mairies pour qu'ils nous aident à faire de The Hacking Project un nouveau format d'éducation pour tous.<br>
Déjà 300 personnes sont passées par The Hacking Project. Est-ce que la mairie de #{array_city[index].capitalize} veut changer le monde avec nous ?<br>
Charles, co-fondateur de The Hacking Project pourra répondre à toutes vos questions : 06.95.46.60.80 <br>

And they've always been followed by the lovely-dovely account twitter : <a href="https://twitter.com/Tt_thp">TT Twitter</a> <br>

### Files
- The programm "<b>scrapping.rb</b>" scrapped the mails and name of all the townhall of 3 departement.

- The programm "<b>get_mail_and_name.rb</b>" is used to get the name or the email of the town scrapped in the spreadsheets, by using two methods : get_mails() and get_names()

- The programm "<b>townhall_mailer.rb</b>" can be used to send an email to every townhall listed by get_mail_and_name()

- The programm "<b>BotTwitter.rb</b>" follow every townhall and gathered their ID in the spreadsheet, section "ID"

### Acknowledgments

MERKI TOU LE MOND
