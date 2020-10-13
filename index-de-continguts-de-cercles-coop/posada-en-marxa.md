# 3. Manual per crear una reunió societària virtual

{% hint style="info" %}
Assumint que ja teniu disponible una [instància de Decidim](../#com-puc-utilitzar-cercles-coop) i un [sistema de emissió de vídeo](necessitats-tecniques-per-organitzar-i-celebrar-reunions-virtuals.md#1-emissio-de-video-en-directe) seleccionat. 
{% endhint %}

{% hint style="info" %}
Podeu consultar documentació més amplia sobre Decidim a [https://docs.decidim.org](https://docs.decidim.org) No obstant si voleu fer servir les funcionalitats que CooCat ha validat us recomanem seguir únicament aquesta guia. 
{% endhint %}

Si has sol·licitat la creació d'un Decidim i ets el primer administrador hauràs rebut un correu per registra-te, en cas que aquest correu no t'hagi arribat pots recordar la contrasenya. Fent clic a l'enllaç de dalt a la dreta **Entra**

![](../.gitbook/assets/screenshot_2020-08-17-iniciar-sessio-prova-assemblea.png)

També la primera vegada que s'accedeix a **/pages/terms-and-conditions** s'han d'acceptar els termes i condicions del servei abans de poder realitzar accions a la administració.

Un cop fet ja podem accedir al panell d'administració, al menú de dalt a la dreta t'apareixerà la opció "Taulell de administració"

![](../.gitbook/assets/screenshot_2020-08-17-prova-assemblea.png)

### Preparació

{% hint style="info" %}
Si fas servir el servei ofert per cercles.coop ja tindràs creades Pàgines, Àmbits pots saltar a la creació de la [Consulta](posada-en-marxa.md#consultes)
{% endhint %}

#### Pàgines informatives

En la administració en la secció **Pàgines** podem editar els continguts de les pàgines, podem crear/editar/suprimir diversos Temes i Pàgines explicatives, però obligatoriament hem de tenir les següents pàgines: 

* FAQ \(preguntes freqüents\) **pages/faq**
* Termes i condicions **pages/terms-and-conditions**
* Accessibilitat **pages/accessibility**

#### **Àmbits**

Abans de crear una consulta necessitem crear un àmbit, si no esperem tenir diversitat d'àmbits en que és realitzen les consultes podem crear sols un anomenat "reunió societària" per qualsevol reunió i després un àmbit concret per les preguntes tipus "assemblea general"

A la administració, secció **Configuració &gt; Àmbits** fem clic a dalt a la dreta **Afegir**

* **Nom:** reunió societària
* **Codi:** reunio-societaria

Un cop creada fem clic a sobre **reunió societària** i dins podrem **Afegir** un "sub àmbit" que anomenarem 

* **Nom:** assemblea general
* **Codi:** assemblea-general

#### Consultes

El mòdul de consultes és el que farem servir per organitzar les votacions a una determinada reunió, si anem a la secció **Consultes** en el menú de administració podrem crear una nova consulta fent clic al botó de dalt a la dreta **Nova consulta**

![](../.gitbook/assets/screenshot_2020-08-18-prova-assemblea.png)

Hem d'omplir els següents camps:

* Títol
* Subtítol
* Descripció \(afegir tota la informació relativa a com participar en la assemblea\)
* Comença la votació: Data de la assemblea
* La votació finalitza: Data de la assemblea
* Abast destacat: Reunió Societària
* Nom curt d'URL \(sense espais per exemple assemblea-general-2020\)

Altres camps recomanats: 

* Imatge del banner
* URL de vídeo introductori \(pot ser un video explicatiu o bé el video del broadcasting\)

{% hint style="info" %}
Si emetem el video a través d'un sistema de broadcasting, com youtube, el podem afegir al camp **URL de vídeo introductori** [tal com s'explica aquí](../video-de-la-assemblea/videoconferencia/mode-broadcasting.md#mostrar-el-video-de-youtube-a-decidim).
{% endhint %}

{% hint style="danger" %}
Fins que no fem clic a **Publicar** la consulta no serà visible pels visitants.
{% endhint %}

{% hint style="info" %}
Si la votació està tancada per data però pública permetrem que les sòcies entrin a consultar les preguntes i la documentació relativa però sense poder votar. 

Quan vulguem obrir la votació canviarem la data de **Comença la votació** a un dia anterior a avui, quan vulguem tancar la votació mourem la data de **La votació finalitza** a un dia anterior a avui.
{% endhint %}

#### Preguntes de la consulta

Dins de la Consulta creada podrem crear totes les preguntes i respostes possibles per cada una d'ella. Fem clic a **Preguntes** al menú lateral esquerra i després **Nova Pregunta** fent clic al botó de dalt a la dreta.

Hem d'omplir els següents camps:

* Títol
* Subtítol
* Grup promotor
* Àmbit participatiu
* Què es decideix
* Àrea municipal: Assemblea General
* Nom curt d'URL \(sense espais per exemple pregunta-1\)

Fent clic a la pregunta creada veurem que al menú lateral esquerra se'ns despleguen més opcions, **recomanem sols fer ús de les dues següents**: 

* Respostes \(podem crear totes les respostes que necessitem, habitualment: _A favor, En contra, En blanc_\)
* Adjunts \(documents de consulta que acompanyen la pregunta\)

{% hint style="info" %}
Per poder publicar una pregunta cal que sempre es creïn les respostes possibles
{% endhint %}

{% hint style="danger" %}
Per tal de mantenir la compatibitat amb la delegació de vot no tocarem la configuració de les preguntes.
{% endhint %}

![](../.gitbook/assets/screenshot_2020-10-13-cooperativa-proves.png)

Abans de publicar la pregunta ens assegurem que es requereixen les verificacions de identitat que considerem, fent clic sobre la icona amb forma de clau. 

{% hint style="info" %}
A cercles.coop recomanem que estiguin marcades per totes les preguntes:  Verificació directa i SMS \(el que significa que sols poden contestar les preguntes de la assemblea les persones que hem convidat pel cens \(verificació directa\) i que a més han validat que tenen accés al seu telèfon mòbil\)
{% endhint %}

Un cop configurats els permisos d'accès a la pregunta podem fer clic sobre la icona amb forma de llapís i al final del formulari de configuració de la pregunta ens apareixerà la funció de publicar. 

#### Importació de les participants

Format document CSV  
Primera linea capçalera, separant columnes amb comes i sense espais:

```text
email,nom,membership_phone,membership_type,membership_weight
```

Següents línies de dades, separant columnes amb comes i sense espais:

```text
email,nom,membership_phone,membership_type,membership_weight
joana@example.com,joana garcia,76318371,treballadora,3
miqul@example.com,miquel,653565765,treballadora,2
[...]
```

**membership\_type** i **membership\_weight** representen tipologia de sòcies, i ponderació del vot, respectivament aquesta dada es farà servir per mostrar resultats agrupant sòcies amb la mateixa tipologia i poderació de vot. Per tant en el exemple si hem fet servir tipologia sòcia "treballadora" és important que fem servir exactament el mateix text per totes les sòcies de tipus "treballadora".

#### Delegacions

Si necessitem realitzar delegacions de vots ho podem fer com administradores a **Participants &gt; Delegacions**

![](../.gitbook/assets/screenshot_2020-10-13-cooperativa-proves-1-.png)

Podrem realitzar delefacions per diferentes consultes \(diferentes reunions\). Fent clic a **Nova delegació** crearem la configuració per la consulta que dessitgem, podem especificar **Consulta**, **Màxim nombre de delegacions que pot rebre una sòcia.**

### Reunió

#### Votacions

#### Visualització de resultats

### 

