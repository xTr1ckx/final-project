# Izstrādes žurnāls

## 1. solis: Plānošana
Es personīgi nekad iepriekš nebiju veidojis konkrētu plānu par kādas programmas izveidi, tāpēc šis process bija nedaudz sarežģīts -
sanāca tā, ka vajadzēja jau domāt no skatu punkta, ka programma ir pabeigta un es to vienkārši aprakstu, kamēr realitātē programma
pat nebija iesākta. Man personīgi ir vieglāk iedomāties kādu ideju par noteiktu programmu un sākt ar kaut kāda vienkārša koda
rakstīšanu, kas arī laika gaitā iedvesmo citas idejas un no tā arī izriet pabeigtā programma. Es arī zināju, ka programmas
veidošanas laikā daudz kas mainīsies no sākuma plāna, tāpēc es personīgi neredzēju lielu iemeslu pašam sev veidot šo plānu.

## 2. solis: Datu slānis un pamata darbības
Principā vislielākā palīdzība koda rakstīšanā un UI elementu izvadē nāca no minēšanas spēles, ko taisījām trešajā un ceturtajā nedēļā. 
Balstoties uz iegūtajām zināšanām pildot iepriekšējo nedēļu mājasdarbus, bija relatīvi viegli iesākt programmas rakstīšanu. Protams 
bija arī jaunas lietas kuras vajadzēta izprast, lai efektīvi pielietotu tās programmas kodā (kā piemēram datetime un visas funkcijas 
saistītas ar to), bet laika gaitā viss sanāca kā iecerēts. 

## 3. solis: Filtrēšana, kopsavilkums un dzēšana
Izpētot kādas funkcijas būs vajadzīgas uzkodēt šajā solī, pamanīju, ka nebija nekādas funkcijas rediģēt jau pastāvošos izdevumus 
programmā. Man likās, ka tā ir svarīga funkcija, tāpēc bija vēlme pamēģināt pašam tikt galā ar šīs funkcijas izveidi, kas nebija 
vienkārši, toties es biju priecīgs par gala rezultātu, it īpaši jo funkcionāli tā strādāja uzreiz kā bija ieplānots. Neliela aizķeršanās
sanāca kad es pamanīju, ka tas izdevumus, kuru es izvēlējos rediģēt ne vienmēr bija tas kas tiešām tika rediģēts. Pašam testējot 
rediģēšanas funkciju vairākas reizes es sapratu, ka problēma bija tajā, ka es izdarīju tā, ka terminālī visi izdevumi tiek sakārtoti
pēc datumiem, tomēr pašā programmā izdevumi tika sakārtoti pēc to ierakstīšanas secības. Ar interneta palīdzību un ar mākslīgo intelektu
sanāca salabot šo funkciju. Veidojot programmu, padomāju par izdevuma aprakstu - tam nebija nekāda limita cik daudz var tajā rakstīt,
tāpēc loģiskais risinājums bija atgriezties pie trešās nedēļas mājasdarbu, kur bija izmantota truncate() funkcija tieši šim mērķim.
Lielāko problēmu tomēr sagādāja izdevumu saraksta formatēšana, jo es nekādīgi nevarēju dabūt "Datums, Summa, Kategorija, Apraksts" 
uzrakstus pareizās pozīcijās. Biju mēģinājis visādus risinājumus līdz maģiski sanāca kaut kāds ļoti primitīvs risinājums (kur es 
vienkārši saliku vairākas atstarpes starp Summa un Kategorija) un kaut kādā veidā, terminālī pareizi sāka rādīties šie tituli. Maniem
nolūkiem šis risinājums bija pietiekami labs un man bija bail to turpmāk aiztikt.

## 4. solis: CSV eksports un dokumentācija
Līdz šim solim viss gāja labi līdz brīdim kad es izlasīju mājasdarba aprakstā, ka >200 kodu rindiņām failā skaitās kā kļūda un atjēdzos, 
ka manā app.py programmā ir 381 rindiņas ar kodu. Sapratu, ka būs jātaisa refactoring, kas uzreiz nesa galvassāpes, jo vajadzēja sākt 
domāt kuros moduļos ies kods un kā es visu savilkšu kopā. Šajā solī it īpaši nāca palīgā trešās nedēļas uzdevums, kur mums vajadzēja 
refactorot jau izveidoto spēli. No šī man arī izrita secinājums, ka ir jāizveido ui.py modulis un te arī sapratu, ka es lielu daļu koda
loģikas rakstīju app.py nevis logic.py. Pagāja diezgan ilgs laiks līdz sanāca pārmest kodu uz citiem moduļiem nesalaužot programmas 
darbību. Protams visādi tārpi tā pat līda ārā, bet mākslīgais intelekts nāca palīgā izprast kāpēc kaut kas nestrādāja un kalpoja kā 
kolēģis, kas izcēla tavas kļūdas vai nepilnības kodā. Bija interesanti arī apskatīt bonusa funkcijas - it īpaši interesēja uzzināt kā
vispār var uztaisīt šādu meklēšanas funkciju.