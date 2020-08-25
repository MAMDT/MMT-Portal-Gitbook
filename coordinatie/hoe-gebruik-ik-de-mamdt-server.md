# Hoe gebruik ik de school server?

Als MAMDT-student krijg je toegang tot je eigen online "plekje". Je ontvangt daarvoor een bericht per mail na de introductieles van MMT. Mocht je dat bericht niet hebben gekregen, stuur dan even een Slack bericht naar je docent.

{% hint style="danger" %}
Niet alle studenten hebben reeds een account op de MAMDT server. Wil je graag toegevoegd worden? Stuur een mailtje naar [vincent.sijben@zuyd.nl](mailto:vincent.sijben@zuyd.nl). Vergeet niet je studentnummer te vermelden.
{% endhint %}

In dit artikel leer je een verbinding te leggen tussen jouw lokale bestanden en de omgeving die aan jou is toegekend op de MAMDT-server. We gaan daartoe werken met een [ftp-client](https://en.wikipedia.org/wiki/Comparison_of_FTP_client_software); software waarmee een ftp-verbinding tot stand kan worden gebracht. **In de voorbeelden wordt gebruikt gemaakt van FileZilla.** [**Download FileZilla hier**](https://filezilla-project.org/download.php?show_all=1)**.**

{% embed url="https://filezilla-project.org/download.php?show\_all=1" caption="download FileZilla" %}

Om verbinding te kunnen maken dien je over de ftp-gegevens te beschikken die je ontvangen hebt per mail \(afzender is reselzuyd\).

{% embed url="https://vimeo.com/287886848/a48a06ba1b" %}

{% hint style="warning" %}
Bij het installeren van FileZilla vraagt de _installer_ additieve software te mogen installeren. FileZilla noemt dit ['bundled' software](https://www.bleepingcomputer.com/news/security/filezillas-use-of-bundled-offers-sparks-outrage-from-users/). **Installeer deze extra software echter niet, we zien dat als** [**bloatware**](https://www.techopedia.com/definition/4237/bloatware)**.** Het heeft verder geen toevoeging op FileZilla.
{% endhint %}

### Aan de slag <a id="aan-de-slag"></a>

De `.html`-pagina's die je hebt gemaakt zijn tot nu toe alleen zichtbaar op je eigen apparaat \(lokaal\). Om een site online \(live\) te plaatsen \(en dus zichtbaar voor iedereen\) dien je de bestanden te uploaden naar een ruimte op een [_server_](https://www.lifewire.com/servers-in-computer-networking-817380). Vaak wordt serverruimte gekocht via _hosting providers_ zoals [Transip](https://www.transip.nl/), [Hostnet](http://www.hostnet.nl/), [mijnDomein](https://www.mijndomein.nl/), [Hostgator](https://www.hostgator.com/) en vele andere. Je kunt ook je eigen computer inrichten als server. De _domeinnaam_ verwijst je door naar de betreffende ruimte op de server.

Je kunt op allerlei manieren verbindingen maken met een server. Met reguliere webservers kun je doorgaans verbinden door middel van [FTP](https://www.digitaltrends.com/computing/what-is-ftp-and-how-do-i-use-it/) \(_File Transfer Protocol_\). Met de unieke ftp-gegevens kun je een verbinding maken met je unieke ruimte op de server. Zo kun je de bestanden op de server bekijken, downloaden of andere bestanden uploaden. Ftp-gegevens bestaan doorgaans uit 3 onderdelen:

1. Het ftp-adres. Ook wel eens _host_, of _server_ genoemd. Voorbeeld: _`ftp.website.com`_
2. _Gebruikersnaam_
3. _Wachtwoord_

Het kan zijn dat er additionele informatie nodig is voor het tot stand komen van de verbinding. Soms dien je aan te geven dat er een specifieke _poort_ of _encryptie_ moet worden gebruikt. Dit wordt meestal bij het ontvangen van de ftp-gegevens aangegeven. Om verbinding te kunnen maken via ftp gebruiken we een _ftp-client_. Software die de verbinding tot stand brengt en de bestanden weergeeft.

* [ ] \*\*\*\*[**Download FileZilla**](https://filezilla-project.org/)\*\*\*\*
* [ ] In dit voorbeeld maken we een ftp-verbinding met de server van MAMDT. **Pak de ftp-gegevens erbij die je hebt ontvangen in je mail**

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LBKz5kbVKsfWEBCyX1y%2F-LC8x5e2cahapETxtrWW%2F-LC96A0heyslS_naHy4d%2FScreen%20Shot%202018-05-10%20at%2014.52.38.png?alt=media&token=5e768079-0649-493e-9684-0a3df570fca3)

In de meeste _ftp-clients_ kun je de ftp-gegevens opslaan. Zo kun je gemakkelijke meerdere ftp-gegevens tegelijkertijd managen.

* [ ] **Open in FileZilla de Site manager.** Ga naar _file -&gt; Site manager_

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LBKz5kbVKsfWEBCyX1y%2F-LC8x5e2cahapETxtrWW%2F-LC97CaAx7fPOpmO2bmb%2FScreen%20Shot%202018-05-10%20at%2014.57.19.png?alt=media&token=0cf1cdcc-8dae-4bfa-82b9-c5a43bb01e82)

* [ ] **Maak een nieuwe site in de** _**Site manager. Klik op 'new site'.**_
* [ ] **Vul hier de ftp-gegevens zoals ontvangen in de e-mail.** Zodra je op '_connect_' verbindt je met de server.

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LBKz5kbVKsfWEBCyX1y%2F-LC8x5e2cahapETxtrWW%2F-LC97sPpQOlCWo1xrujS%2FScreen%20Shot%202018-05-10%20at%2015.00.21.png?alt=media&token=6274802d-b080-494f-bc08-d5f09b60f5f4)

* [ ] In het volgende venster kun je het certificaat vertrouwen door het vinkje te plaatsen en op OK te drukken:

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LBKz5kbVKsfWEBCyX1y%2F-LCUmgVSrbXQyOKOanOg%2F-LCUmwrr55bPrH6iifvJ%2Ftrust.jpg?alt=media&token=96a3fff1-6728-4c21-b143-1b366639ec5e)

​

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LBKz5kbVKsfWEBCyX1y%2F-LC8x5e2cahapETxtrWW%2F-LC98CTCqOD6zqt2quZM%2FScreen%20Shot%202018-05-10%20at%2015.01.19.png?alt=media&token=96b84bb6-74a8-4e54-9c64-fb5332bb3202)

Alle gegevens goed ingevuld? FileZilla laat aan de linkerzijde je _lokale_ _bestanden_ zien, aan de rechterzijde zie je de _live_ _bestanden_. Je bent succesvol verbonden wanneer de _status_ dit aangeeft en de bestanden aan de rechterzijde zichtbaar zijn.

Doorgaans bevat je server meer dan één folder. Wellicht staan er al bestanden op die wilt overschrijven. **Daarentegen dient maar één folder als** _**rootfolder**_ **voor je website.** Overige folders zijn wellicht in gebruik voor andere toepassingen zoals mail of databases. Laat de mappen in de root van je server met rust. **Vaak is de map** _**`public_html`**_ **\(ook wel eens** _**public**_ **of** _**html**_ **genoemd\) de map waarin de bestanden van je website moeten worden geplaatst.** De nieuwe _root_ van je site.

* [ ] **Sleep de inhoud van je lokale rootfolder naar de** _**`public_html`**_ **folder op de server.** Je bestanden worden gekopieerd van _local_ naar _live_.

_**`public_html`**_ **is je nieuwe rootfolder. Zet dus niet de volledige folder, maar de bestanden ín jouw lokale rootfolder naar de nieuwe live folder.**

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LBKz5kbVKsfWEBCyX1y%2F-LC8x5e2cahapETxtrWW%2F-LC9AYoDCaRyUwsmHY-a%2FScreen%20Shot%202018-05-10%20at%2015.11.56.png?alt=media&token=3b0f5a6e-35dc-4df3-9e31-b57f90e6f072)

Je bestanden staan nu live! Bezoek je site op je domeinnaam \(staat ook in de mail met de ftp-gegevens\). Je domeinnaam is het gedeelte zónder `:2222`.

Wil je meerdere projecten op deze test-server plaatsen? Maak simpelweg een aantal sub folders in _`public_html`_. Iedere subfolder kan dienen als nieuwe rootfolder; de URL wordt dan wel: `student-123456sijb.mamdt.com/nieuwefoldernaam/`.

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LBKz5kbVKsfWEBCyX1y%2F-LCDGVtMUrXgy2MR2bc7%2F-LCDGh0LyjzSVHei6CLj%2FScreen%20Shot%202018-05-11%20at%2010.12.05.png?alt=media&token=dbbfe475-6a8e-4d4a-a8ac-f94d1194f81a)



