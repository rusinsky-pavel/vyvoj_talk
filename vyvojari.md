# Jak komunikovat s vývojáři

- neexistuje jedna pravda, hledejte cesty ke svým vývojářům
- vše je jen má zkušenost

## Proč jsou vývojáři "jiní"?

"Problemy zpusobuji systemove alokace pameti primo pro kernel. To dale ma za pricinu nemoznost alokace dostecne pameti pro radice sitove karty (bnx2x) a tim padem jak drop spojeni z aplikace, tak i samotne zpomaleni databaze. Pamet se sice jevi jako volna, ale je zcela fragmentovana a nestaci se vcas uvolnovat a tim padem zpusobuje tyto problemy. Jako prvni krok navysuji volnou pamet pro kernel a zmenim nastaveni pro dirty pages."

"Funguje to, ale nejde to použít."


## Rozdíly mezi vývojáři

### Pracovní zaměření

- vyvojářských zaměření je spousta a zmíním jen ty "nejklasičtější"
- je potřeba pořádně vybrat vývojáře s ohledem na jeho zaměření
  - lépe pak pracuje a je šťastnější

#### Backend developer

- pracuje na "vnitřnostech" aplikace = to co nejde vidět
- má rád logické fungování věcí, rád se hrabe pod kapotou
- nemá rád barvičky
- často používané jazyky: C, C++, C#, Python, Java, PHP, aj.

#### Frontend developer

- vyrábí to, jak to vypadá -> UI/UX
- má rád barvičky, animace, "zajímá se o lidi"
- používané jazyky: JavaScript (+HTML, CSS)

#### Full-stack developer

- dělá všechno sám => nemá kompletní zaměření
- vhodný pro menší projekty, na kterých udělá všechno
- nevhodný na komplexní a velké projekty, kde je potřeba zaměření
- nikdo není naprostý full-stack

#### DevOps

- zaměřuje se na servery, infrastukuru
- řeší věci ještě o level níž než programátoři
- jazyky: Bash, Python

#### Tester

- zaměřuje se testování fungování aplikace
- často není programátor, ale může být!
- je pro něj důležité, že to fakt jede

#### AI guy

- často se zaměřuje na vývoj umělé inteligence a chytrých modelů
- má rád automatizaci všeho
  - stává se, že chce automatizovat až za "normální" hranici

#### Co si toho odnést

- je důležité vybrat si správný typ vývojáře na správnou pozici
  - když chcete nějaký spešl web, není špatné mít full-stack
  - když potřebujete někoho kdo bude řešit rychlost aplikace, zkuste sehnat DevOps/databázistu
  - atd

### Osobnostní typ

- spíš meme, každý vývojář je osobnost
- jsou určité stereotypy, se kterýma se pracuje jinak, ale není to tak vždycky!

#### Oldschool nerd

- klasický oldschool programátor
- schovaný ve tmě, pracující v noci
- silnější/rachitický, protože nemá dobrou výživu a pořád sedí u PC
- tento obrázek se často ukazuje, dneska to tak ale z větší části není

#### Be-fit

- sporťák, který je dynamický a nechce mít pupek ze sezení za stolem
- mívá velký drive, někdy až moc velký

#### Everyday normal guy

- všichni ostatní, normální lidé
- každý je svůj a je potřeba k němu přistupovat jednotlivě

## Jak nastavit komunikaci s vývojáři

- pokud nerozumíte "vývojářské hantýrce", nechte si to vysvětlit (a pořádně!)
- buďte otevření
- pochopte co konkrétní vývojáře baví na jejich práci
  - někdo se rád šťourá v detailech
  - někdo rád dělá nové věci
  - někdo chce hodně peněz
  - atd.
- je důležité stanovit si pravidla, přestože většina vývojářů nemá ráda byrokracii
  - můžou vám pomoci již vymyšlené metodiky (Kanban, Scrum, PRINCE2, aj)
- dva nejčastější typy komunikace, můžete mít nějaké mezistavy

### Interní tým

- v kanclu
  - poznejte, co je to za lidi a podle toho se s něma bavte (tohle je pravda, pro všechny zaměstnance)
  - chtějte, aby věděli na čem pracují a proč je to důležité
  - zapojte je do rozhodování
  - tvořte skupiny na konkrétní problém,
    - ale nechte každého říct svůj názor na technický problém, i když není v pracovní skupině
  - pravidelně se setkávejte, aby všichni byli v obraze
- remote
  - viz to předchozí
  - dejte větší důraz na reportování a transparentnost práce
  - pokud to jde, jednou za čas se vídejte real-life

### Externí pracovníci

- dbejte na reportování a transparentnost práce
- stanovte přesná a striktní pravidla spolupráce
- dělejte zápisy z každého jednání
- nebojte se rozvázat spolupráci
  - ano vývojářů je málo, ale je opravdu špatné dělat s někým nekompetentním

## Jak zadávat a trackovat práci

- důležité pro každý tým/spolupráci

### Kompletní zadání vs. Barely enough

| Kompletní zadání               | Barely enough                                     |
|--------------------------------|---------------------------------------------------|
| Vhodné pro externí spolupráci  | Vhodné pro interní tým                            |
| Opravdu popsat všechno         | Popsat to tak, aby to šlo udělt                   |
| Náročné pro přípravu           | Sniží se náročnost pro product ownery/projekťáky  |
| Nikdy to není kompletní        | Počítá se s tím, že se něco dodělá potom          |
| Menší chybovost                | Větší počet neočekávaných/nerozmyšlených věcí     |
| Vzniká micromanagement         | Vychováváte si spolehlivé vývojáře                |

[Kompletní zadání](https://github.com/rusinsky-pavel/vyvoj_talk/issues/2) vs.
[Barely enough](https://github.com/rusinsky-pavel/vyvoj_talk/issues/1)


### Jak zadávat

#### Ústně

- vyhněte se tomu co nejvíc = co není na papíře se neudělá
- možnost pouze v interním týmu
- pokud spolupracujete s někým externím, vždy to musí být nakonec zaevidované!

#### Online

- různé aplikace (github/jira atd.)
  - nachystané nástroje lidma, kteří mají zkušenost
  - nebojte se je trochu ohnout pro vaše účely a vaše workflow (pokud už trochu víte co děláte)
    - lepší je začít s něčím nachystaným a pak iterativně upravovat ke svým účelům
- maily
  - špatně se zajišťuje transparentnost práce a vzniká trochu chaos
- slack aj.
  - je to možnost, ale lepší je napsat si, že je problém a ten pak zadat jako task
  - špatně se dohledává, kdo co napsal a tak


### Trackování

- pokud potřebujete trackovat hodiny, používejte nějaký nástroj (př. toggle)
- z mé zkušenosti lepší domluvit si odměnu za určitý task
  - je důležité rozplánování předem

## Money, money, money

- vyvojáři jsou drazí
  - specializace, která jde do budoucnosti a je tak nastavený trh = počítejte s tím
  - ne každý vývojář si ty peníze zaslouží = pokud ne, nedávejte mu je jen proto, že je to vývojář
  - odměňujte dobré vývojáře, je o ně nouze
- jestli chcete dělat software, nachystejte si peníze (a postupně hodně peněz)
- pokud někdo jde do IT, protože je tam velká výplata, tak z něj nebude pravděpodobně dobrý vývojář (ale jsou i výjimky)

## Nabírání vývojářů

- pokud je to možné, věnujte se nějaké IT komunitě => jdete vidět mezi ostatníma

### Pohovory

- vystavte inzerát a pohovorujte
  - dejte si pozor na CV, papír snese všechno
  - vývojáři (hlavně junioři) napíšou do CV, že umí uplně všechno = vypíšou technolgie o kterých slyšeli/jednou viděli ve škole
- nedejte jen na školu, spousta self-tought vývojářů opravdu umí
  - škola má výhodu v širším rozhledu v IT (nemusí býr pravda!)
- pokud pořádně nerozumíte IT, vemte si s sebou někoho kdo IT rozumí
- ptejte se na věci z oboru, ale i na věci jiné
  - technicky dobrých programátorů je hodně, ale do týmu/na spolupráci potřebujete někoho "normálního"
    - s vývojáři je někdy těžké se domluvit => lepší normální člověk, který se naučí
  - hledejte hlavně "drive" se učit a dělat nové věci!
- pokud si nejste jistí skillem, zadejte úkol k vypracování

### Drafting/scouting

- draftovat vývojáře se vyplatí
  - viz výše, shánějte super lidi do týmu + "drive"
- nemarněte tím moc času a nemějte to jako hlavní způsob nabírání
- výhodné pro externí spolupráce = "na doporučení"
- zkuste pohovorovat/draftovat na školních systémech (př. VUT v Brně to má cool)

### Agentury

- slibují, že najdou vývojáře
  - často ale jen možná "shoda" s potřenými znalostmi
- velmi agilní a drsný trh
  - scoutují linkedin a facebook extrémně rychle
  - 10 min po zveřejnění "Hledám práci" na LinkedInu 3 agentury
- nezpomeňte, že je to drahé

## Slova, která se naučíte akceptovat

...nic jiného vám nezbývá...

Debugging
- kachnička?
Release
Testování
Refactoring
Bug
Estimate
Hot-fix
Workaround
Hack
Produkce
Fíčr
Implementační detail
a spousta dalších....

