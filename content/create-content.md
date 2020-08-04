---
layout: default
title: Creating Content
permalink: /create-content/
parent: Part 1 - The basics
nav_order: 8
---

# Add Content To Your Site

## Posts and Pages

Before we add content to our site, lets go over the two basic types of content documents: posts and pages.

### Posts

Posts are the dynamic content that makes up your site. Often these are articles, tutorials, or some newsworthy event, but can take the form of whatever you want. Posts are published with a date – which affects their timing, relevancy, and longevity.

Posts should always be written in a markup language such as Markdown or HTML, and always follow the naming convention: **YYYY-MM-DD-title-of-post**.markdown

Navigate to your Jekyll site directory on your computer, and open the **_posts** folder. Inside you should see your "welcome-to-jekyll" Markdown file. **Open that file in your code editor**.


#### Front Matter

Your post and page is divided into two main sections. The "front matter" and the content. The front matter of your post provides Jekyll with basic information about the document - such as the layout, title, author, date, and other things. Some of these front matter elements, like information about the layout, are defined elsewhere in your Jekyll directory. Your front matter should look something like this:

```
---
layout: post
title:  "Welcome to Jekyll!"
date:   2020-02-05 08:49:10 -0800
categories: jekyll update
---
```

For this workshop, we're going to leave the default front in our post the way they are. Instead, let's edit the content below with some Lorem Markdownum (via [jaspervdj.be/lorem-markdownum/](https://jaspervdj.be/lorem-markdownum/){:target="_blank"}). Copy the text below, and replace the content below your front matter.

```
## Certis quem vincla at triste Surrentino placuisse

Fulsit *Phoce* hiscere incustoditae terra Achillem offensaque fratri enim
desunt. Duorum mutabit [nec](http://crines.io/phoebeiusumeris.php).

1. Micant inanes datura
2. In vela consorte precesque perdiderant molle pendebant
3. Auditis lateat ursi mundi
4. Rogus et victus pharetras experiensque silvas sim

Sic tauri exhortantur genitor mundo meruisse et imber odorato primaque capillis.
Et pio regem per saepe adspice, alto. Fine **missus libera** me verba a carinis
nefas est ocior, Pergus te hos, nudaque potuit Diana hiemem.

    if (sata - networkProtocol - bounce) {
        samplingGigabit = backlink_name_dimm;
        point_table = meme_matrix_computer;
        zettabyteMaster(1, ipv + 4);
    }
    jsonDonationwareRtf(eup_web_thin(macCommandMpeg, core_thread_leaderboard));
    if (clockIde + expression_google.server_exif_frequency.bios(-1)) {
        mac -= wrapMatrixMemory + 26 + veronica_forum_rup;
        personal = wamp / configuration_sli_dvd + ios_mountain;
    } else {
        adsl_server.jpegMainframeData += 4;
        oasis_dongle.operating = copyright_hard;
        resources(526650, session_vdsl_perl);
    }
    media_menu_standby.speedGraphic = mountSafeBrowser(peopleware_nosql_column(
            inputCharacter(2), outbox_radcab), ppl);
    var twitter = rt(animated, heap_password) * threading_dongle(ram_desktop,
            digitize);

Imumque nam [parabat visa](http://bracchia.net/), corpus vix perenni vires tibi
formamque velate lucem in quem. Achivos cana artisque veste inquit aristas
divesque laeso.
```

Now save your document, and refresh your browser to see the changes live.

### Pages

Pages are used for the static content on your site such as an About, Contact, or CV page. The easiest method for adding a page is to create a <code>.md</code> document in the main (root) folder of your site.

Let's create a new file called <code>contact.md</code> and add the following text.

```
---
layout: page
title: Contact Us
permalink: /contact/
---

## In erat Dircen

Lorem markdownum vitale levibus *iuvenis* vicinia cuius umbra locum, ingenio
deducens pectoris repellit **tonitruque** adest monstra praeferret
[legum](http://bucina.io/est). Sua induitur sanguine [cibis et
lassaque](http://www.ortus.io/) quamvis vertitur inpensaque praecipue litora?
Oculos invidiam poscimus resupinus in summa; erat pleno sparsae. Adsueta referam
Quo leve arvo Bacche ora cruentum densa: ite pavet.

1. Epulis tumultus solidis
2. Tenues ab ut tale iuste tellusque superest
3. Differt tabuit pinum
4. Gente mendacia mutaverat habitus
5. Liquescunt o quoque

*Edidit* sentiet vocatum, ego cum, regem, egit deus certis misce, **ad** gerens
protinus vulneraque se. Rhoetus quoque permulcetque sonant pepulere nymphae ait.
Partes magna fert per, peteret, fulminis [profuso](http://tergo.io/non.php) ad
cuspidis Sicaniam. Domum ausa foramina; mox rumpit, macies nec murmure adhuc
delendaque. [Et](http://erat.org/vocatusriguo.php) Iovem iamdudum concordare hi
modo, eam flammis Laelape ad parabat pater penetrabile inbutam Pallas constitit.

> Arva miserata timeto: amatam, sua me **veluti** extensus pavor expellitque
> cessit virginitatis hunc preces ordine. Est nulloque raptos. Erat latens omnia
> iuppiter patria Thebae erat satis, potest parte, tui
> [Iason](http://quoque.net/in-pugnando) patria salutant Othrys faveatque; duri.
> Ora Boreas Iovis: [temptavit](http://telum-pinum.net/) heros et facit fuisse,
> ex ipsa parte freta. Gemitus vitae.
```

Now save your file and refresh your site's homepage.

Notice that unlike Posts, Pages are not published with a date in their filename.
