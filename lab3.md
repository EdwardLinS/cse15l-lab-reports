# Command: `grep`
## 4 *grep* command options
### 1. `grep -i` / `grep --ignore-case`
  - **What:** This command option matches without matching case.
  - **Why:** This is useful when you are purely looking for the pattern and not caring about specific case of the pattern.
  - *Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/*

- ***Example 1***
```console
[cs15lwi23aoa@ieng6-201]:skill-demo1-data:501$ grep -i "lotus" ./written_2/travel_guides/berlitz1/*.txt 
./written_2/travel_guides/berlitz1/IntroIndia.txt:        whose navel a lotus grew bearing Brahma whose task it was to create the
./written_2/travel_guides/berlitz1/IntroIndia.txt:        world. Vishnu, a four-armed god with mace, conch, discus, and lotus,
./written_2/travel_guides/berlitz1/IntroIndia.txt:        white elephant holding a lotus flower in his trunk had entered her
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        highlights the emperor’s aesthetic, in the lotus calyx on the gateway’s
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        gardens growing melons, tomatoes, cucumbers, and lotus root in a mesh
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        resting on the inverted lotus that once connected it to the pillar.
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        as well as plentiful trickling streams, lotus ponds, and lakes covered
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        the arcaded Golden Lotus Tank and the temple’s bathing-place. At the
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        lotus-covered bathing tank.
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        arms”) wielding bells, wheels, and lotus flowers. However,
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        a ring of giant lotus leaves, is Nara’s celebrated Daibutsu, or Great
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        white lotus blossoms. The myth-shrouded lakes are said to be the home
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        settlement beneath the surface. Outside lotus-blossom season, the lakes
```
  - **What:** This command searched for files with the word `lotus` regardless of case. 
  - **Why:** The command is useful since it found files not only with `lotus` but with `Lotus` as well. 

  - ***Example 2***
```console
[cs15lwi23aoa@ieng6-201]:skill-demo1-data:515$ grep --ignore-case "pride" ./written_2/travel_guides/berlitz1/*.txt
./written_2/travel_guides/berlitz1/HistoryEgypt.txt:        national pride by wresting the Suez Canal out of British hands he
./written_2/travel_guides/berlitz1/HistoryEgypt.txt:        Limited success in 1973 restored some national pride when the Sinai was
./written_2/travel_guides/berlitz1/HistoryFWI.txt:        France in 1946 — a source of great pride to many. 
More importantly, it
./written_2/travel_guides/berlitz1/HistoryFrance.txt:        national pride sufficiently to oust the English from France 20 years
./written_2/travel_guides/berlitz1/HistoryFrance.txt:        the pride of the Louvre. A new opulent architecture blossomed with the
./written_2/travel_guides/berlitz1/HistoryFrance.txt:        pride found its perfect expression in the Eiffel Tower, thrust into the
./written_2/travel_guides/berlitz1/HistoryFrance.txt:        power in the national capital. By allowing the 
local pride of such
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt:        treasures with great pride. Edinburgh Castle is a treasure in
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt:        1707. The sense of an impending new era can be discerned in the pride,
./written_2/travel_guides/berlitz1/IntroFrance.txt:        pride, the nation’s cultural wealth is just as important. Philosophy
./written_2/travel_guides/berlitz1/IntroFrance.txt:        high technology and is happy to share its pride in these advances. With
./written_2/travel_guides/berlitz1/IntroItaly.txt:        sustains a solid and pugnacious local pride from historic division into
./written_2/travel_guides/berlitz1/IntroJamaica.txt:        within, working on a principle of pride in oneself and in one’s roots.
./written_2/travel_guides/berlitz1/WhatToJamaica.txt:        themselves and their culture with national pride.
./written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:        year. Family pride mixes with economics at these events. Farming can be
./written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:        for visitors and of pride to the farmers who breed and train them. Each
./written_2/travel_guides/berlitz1/WhatToLasVegas.txt:        pride.
./written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:        pride and designed as a mini-Parthenon, in deference to the
./written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:        take pride of place — the zoo has the world’s largest group in
./written_2/travel_guides/berlitz1/WhereToEgypt.txt:        Memphis and constitutes the largest royal graveyard in Egypt. Pride of
./written_2/travel_guides/berlitz1/WhereToEgypt.txt:        A splendid Red granite sarcophagus has pride of 
place in
./written_2/travel_guides/berlitz1/WhereToFrance.txt:        metropolis. Renewed pride in France’s provincial cities is reducing
./written_2/travel_guides/berlitz1/WhereToFrance.txt:        pride.
./written_2/travel_guides/berlitz1/WhereToFrance.txt:        dialect, architecture, cuisine, and local prid 
 — the best of both
./written_2/travel_guides/berlitz1/WhereToFrance.txt:        centuries. But the museum’s pride and joy is its great ceramics
./written_2/travel_guides/berlitz1/WhereToFrance.txt:        textile, and industrial center with a bouncy pride, a taste for the
./written_2/travel_guides/berlitz1/WhereToGreek.txt:        visit. Pride of place goes to a 15th-century icon of the prophet
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        symbol of power and pride, was an understandable choice as the emblem
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        pride is a 200-year-old banyan tree, the Ficus bengalensis, or
./written_2/travel_guides/berlitz1/WhereToIsrael.txt:        long climb to swell national pride, and army recruits are sworn in here
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        proclaims the inordinate but certainly justified civic pride of the
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        restaurants and boutiques, a vibrant local prid 
 nurtured by economic
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        chamber of the Nine Patricians), the full force 
of Siena’s civic pride
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        Annunciation and Madonna with Angels. But Umbria’s pride and joy is the
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        inspired Shakespeare. In Emilia-Romagna, the pride and creativity of
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        With an inherent pride so justifiably timeless, 
the
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        government to Rome, Milan prides itself on being the country’s
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        Titian, Correggio, and Tintoretto, pride of place — and a room to
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        The pride of Turin, as in so many Italian cities, is not
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        Brooklynese. Ignore the proprieties — or offend 
the pride of an
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        waterfront itself is Nippon-maru Memorial Park, 
where pride of place
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        sprawling rival to the east. Osakans pride themselves on being warmer,
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        The pride and joy of the neighborhood is the Meganebashi,
./written_2/travel_guides/berlitz1/WhereToJerusalem.txt:        and became the pride of the Jewish community in Palestine under British
./written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt:        restored. Pride of place goes to SL Dolly, the oldest mechanically
./written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:        Pride Celebration, a lively two-day festival and parade which has grown
./written_2/travel_guides/berlitz1/WhereToMadrid.txt:        Madrid’s pride, the Prado museum, is indisputably the
./written_2/travel_guides/berlitz1/WhereToMadrid.txt:        museum’s greatest pride, spotlighted in its own niche on the ground
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        Plant life. The pride of the mountain is its 
1,500
```
  - **What:** This command searched for files with the word `pride` regardless of case. 
  - **Why:** The command is useful since it found files not only with `pride` but with `Pride` as well. 

----

### 2. `grep -c` / `grep --count`
  - **What:** This command option prints out count of matching lines instead of normal grep output.
  - **Why:** This is useful when the count of files is necessary and not file path or content.
  - *Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/*

  - ***Example 1***
```console
[cs15lwi23aoa@ieng6-203]:skill-demo1-data:501$ grep -c "lotus" ./written_2/travel_guides/berlitz1/*.txt     
./written_2/travel_guides/berlitz1/HandRHawaii.txt:0
./written_2/travel_guides/berlitz1/HandRHongKong.txt:0
./written_2/travel_guides/berlitz1/HandRIbiza.txt:0
./written_2/travel_guides/berlitz1/HandRIsrael.txt:0
./written_2/travel_guides/berlitz1/HandRIstanbul.txt:0
./written_2/travel_guides/berlitz1/HandRJamaica.txt:0
./written_2/travel_guides/berlitz1/HandRJerusalem.txt:0
./written_2/travel_guides/berlitz1/HandRLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/HandRLasVegas.txt:0
./written_2/travel_guides/berlitz1/HandRLisbon.txt:0
./written_2/travel_guides/berlitz1/HandRLosAngeles.txt:0
./written_2/travel_guides/berlitz1/HandRMadeira.txt:0
./written_2/travel_guides/berlitz1/HandRMadrid.txt:0
./written_2/travel_guides/berlitz1/HandRMallorca.txt:0
./written_2/travel_guides/berlitz1/HistoryDublin.txt:0
./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt:0
./written_2/travel_guides/berlitz1/HistoryEgypt.txt:0
./written_2/travel_guides/berlitz1/HistoryFWI.txt:0
./written_2/travel_guides/berlitz1/HistoryFrance.txt:0
./written_2/travel_guides/berlitz1/HistoryGreek.txt:0
./written_2/travel_guides/berlitz1/HistoryHawaii.txt:0
./written_2/travel_guides/berlitz1/HistoryHongKong.txt:0
./written_2/travel_guides/berlitz1/HistoryIbiza.txt:0
./written_2/travel_guides/berlitz1/HistoryIndia.txt:0
./written_2/travel_guides/berlitz1/HistoryIsrael.txt:0
./written_2/travel_guides/berlitz1/HistoryIstanbul.txt:0
./written_2/travel_guides/berlitz1/HistoryItaly.txt:0
./written_2/travel_guides/berlitz1/HistoryJamaica.txt:0
./written_2/travel_guides/berlitz1/HistoryJapan.txt:0
./written_2/travel_guides/berlitz1/HistoryJerusalem.txt:0
./written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/HistoryLasVegas.txt:0
./written_2/travel_guides/berlitz1/HistoryMadeira.txt:0
./written_2/travel_guides/berlitz1/HistoryMadrid.txt:0
./written_2/travel_guides/berlitz1/HistoryMalaysia.txt:0
./written_2/travel_guides/berlitz1/HistoryMallorca.txt:0
./written_2/travel_guides/berlitz1/IntroDublin.txt:0
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt:0
./written_2/travel_guides/berlitz1/IntroEgypt.txt:0
./written_2/travel_guides/berlitz1/IntroFWI.txt:0
./written_2/travel_guides/berlitz1/IntroFrance.txt:0
./written_2/travel_guides/berlitz1/IntroGreek.txt:0
./written_2/travel_guides/berlitz1/IntroHongKong.txt:0
./written_2/travel_guides/berlitz1/IntroIbiza.txt:0
./written_2/travel_guides/berlitz1/IntroIndia.txt:3
./written_2/travel_guides/berlitz1/IntroIsrael.txt:0
./written_2/travel_guides/berlitz1/IntroIstanbul.txt:0
./written_2/travel_guides/berlitz1/IntroItaly.txt:0
./written_2/travel_guides/berlitz1/IntroJamaica.txt:0
./written_2/travel_guides/berlitz1/IntroJapan.txt:0
./written_2/travel_guides/berlitz1/IntroJerusalem.txt:0
./written_2/travel_guides/berlitz1/IntroLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/IntroLasVegas.txt:0
./written_2/travel_guides/berlitz1/IntroLosAngeles.txt:0
./written_2/travel_guides/berlitz1/IntroMadeira.txt:0
./written_2/travel_guides/berlitz1/IntroMadrid.txt:0
./written_2/travel_guides/berlitz1/IntroMalaysia.txt:0
./written_2/travel_guides/berlitz1/IntroMallorca.txt:0
./written_2/travel_guides/berlitz1/JungleMalaysia.txt:0
./written_2/travel_guides/berlitz1/WhatToDublin.txt:0
./written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:0
./written_2/travel_guides/berlitz1/WhatToEgypt.txt:0
./written_2/travel_guides/berlitz1/WhatToFWI.txt:0
./written_2/travel_guides/berlitz1/WhatToFrance.txt:0
./written_2/travel_guides/berlitz1/WhatToGreek.txt:0
./written_2/travel_guides/berlitz1/WhatToHawaii.txt:0
./written_2/travel_guides/berlitz1/WhatToHongKong.txt:0
./written_2/travel_guides/berlitz1/WhatToIbiza.txt:0
./written_2/travel_guides/berlitz1/WhatToIndia.txt:0
./written_2/travel_guides/berlitz1/WhatToIsrael.txt:0
./written_2/travel_guides/berlitz1/WhatToIstanbul.txt:0
./written_2/travel_guides/berlitz1/WhatToItaly.txt:0
./written_2/travel_guides/berlitz1/WhatToJamaica.txt:0
./written_2/travel_guides/berlitz1/WhatToJapan.txt:0
./written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/WhatToLasVegas.txt:0
./written_2/travel_guides/berlitz1/WhatToLosAngeles.txt:0
./written_2/travel_guides/berlitz1/WhatToMadeira.txt:0
./written_2/travel_guides/berlitz1/WhatToMalaysia.txt:0
./written_2/travel_guides/berlitz1/WhatToMallorca.txt:0
./written_2/travel_guides/berlitz1/WhereToDublin.txt:0
./written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:0
./written_2/travel_guides/berlitz1/WhereToEgypt.txt:0
./written_2/travel_guides/berlitz1/WhereToFWI.txt:0
./written_2/travel_guides/berlitz1/WhereToFrance.txt:0
./written_2/travel_guides/berlitz1/WhereToGreek.txt:0
./written_2/travel_guides/berlitz1/WhereToHawaii.txt:0
./written_2/travel_guides/berlitz1/WhereToHongKong.txt:0
./written_2/travel_guides/berlitz1/WhereToIbiza.txt:0
./written_2/travel_guides/berlitz1/WhereToIndia.txt:5
./written_2/travel_guides/berlitz1/WhereToIsrael.txt:0
./written_2/travel_guides/berlitz1/WhereToIstanbul.txt:0
./written_2/travel_guides/berlitz1/WhereToItaly.txt:0
./written_2/travel_guides/berlitz1/WhereToJapan.txt:2
./written_2/travel_guides/berlitz1/WhereToJerusalem.txt:0
./written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:0
./written_2/travel_guides/berlitz1/WhereToMadeira.txt:0
./written_2/travel_guides/berlitz1/WhereToMadrid.txt:0
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt:2
./written_2/travel_guides/berlitz1/WhereToMallorca.txt:0
```
  - **What:** This command searched for how many times the word `lotus` appeared in the all the txt files in the directory. 
  - **Why:** The command is useful since it is able to show which files have the word `lotus` and how many times the word appears in the files that do have the word.

  - ***Example 2***
```console
[cs15lwi23aoa@ieng6-203]:skill-demo1-data:504$ grep --count "pride" ./written_2/travel_guides/berlitz1/*.txt
./written_2/travel_guides/berlitz1/HandRHawaii.txt:0
./written_2/travel_guides/berlitz1/HandRHongKong.txt:0
./written_2/travel_guides/berlitz1/HandRIbiza.txt:0
./written_2/travel_guides/berlitz1/HandRIsrael.txt:0
./written_2/travel_guides/berlitz1/HandRIstanbul.txt:0
./written_2/travel_guides/berlitz1/HandRJamaica.txt:0
./written_2/travel_guides/berlitz1/HandRJerusalem.txt:0
./written_2/travel_guides/berlitz1/HandRLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/HandRLasVegas.txt:0
./written_2/travel_guides/berlitz1/HandRLisbon.txt:0
./written_2/travel_guides/berlitz1/HandRLosAngeles.txt:0
./written_2/travel_guides/berlitz1/HandRMadeira.txt:0
./written_2/travel_guides/berlitz1/HandRMadrid.txt:0
./written_2/travel_guides/berlitz1/HandRMallorca.txt:0
./written_2/travel_guides/berlitz1/HistoryDublin.txt:0
./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt:0
./written_2/travel_guides/berlitz1/HistoryEgypt.txt:2
./written_2/travel_guides/berlitz1/HistoryFWI.txt:1
./written_2/travel_guides/berlitz1/HistoryFrance.txt:4
./written_2/travel_guides/berlitz1/HistoryGreek.txt:0
./written_2/travel_guides/berlitz1/HistoryHawaii.txt:0
./written_2/travel_guides/berlitz1/HistoryHongKong.txt:0
./written_2/travel_guides/berlitz1/HistoryIbiza.txt:0
./written_2/travel_guides/berlitz1/HistoryIndia.txt:0
./written_2/travel_guides/berlitz1/HistoryIsrael.txt:0
./written_2/travel_guides/berlitz1/HistoryIstanbul.txt:0
./written_2/travel_guides/berlitz1/HistoryItaly.txt:0
./written_2/travel_guides/berlitz1/HistoryJamaica.txt:0
./written_2/travel_guides/berlitz1/HistoryJapan.txt:0
./written_2/travel_guides/berlitz1/HistoryJerusalem.txt:0
./written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/HistoryLasVegas.txt:0
./written_2/travel_guides/berlitz1/HistoryMadeira.txt:0
./written_2/travel_guides/berlitz1/HistoryMadrid.txt:0
./written_2/travel_guides/berlitz1/HistoryMalaysia.txt:0
./written_2/travel_guides/berlitz1/HistoryMallorca.txt:0
./written_2/travel_guides/berlitz1/IntroDublin.txt:0
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt:2
./written_2/travel_guides/berlitz1/IntroEgypt.txt:0
./written_2/travel_guides/berlitz1/IntroFWI.txt:0
./written_2/travel_guides/berlitz1/IntroFrance.txt:2
./written_2/travel_guides/berlitz1/IntroGreek.txt:0
./written_2/travel_guides/berlitz1/IntroHongKong.txt:0
./written_2/travel_guides/berlitz1/IntroIbiza.txt:0
./written_2/travel_guides/berlitz1/IntroIndia.txt:0
./written_2/travel_guides/berlitz1/IntroIsrael.txt:0
./written_2/travel_guides/berlitz1/IntroIstanbul.txt:0
./written_2/travel_guides/berlitz1/IntroItaly.txt:1
./written_2/travel_guides/berlitz1/IntroJamaica.txt:1
./written_2/travel_guides/berlitz1/IntroJapan.txt:0
./written_2/travel_guides/berlitz1/IntroJerusalem.txt:0
./written_2/travel_guides/berlitz1/IntroLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/IntroLasVegas.txt:0
./written_2/travel_guides/berlitz1/IntroLosAngeles.txt:0
./written_2/travel_guides/berlitz1/IntroMadeira.txt:0
./written_2/travel_guides/berlitz1/IntroMadrid.txt:0
./written_2/travel_guides/berlitz1/IntroMalaysia.txt:0
./written_2/travel_guides/berlitz1/IntroMallorca.txt:0
./written_2/travel_guides/berlitz1/JungleMalaysia.txt:0
./written_2/travel_guides/berlitz1/WhatToDublin.txt:0
./written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:0
./written_2/travel_guides/berlitz1/WhatToEgypt.txt:0
./written_2/travel_guides/berlitz1/WhatToFWI.txt:0
./written_2/travel_guides/berlitz1/WhatToFrance.txt:0
./written_2/travel_guides/berlitz1/WhatToGreek.txt:0
./written_2/travel_guides/berlitz1/WhatToHawaii.txt:0
./written_2/travel_guides/berlitz1/WhatToHongKong.txt:0
./written_2/travel_guides/berlitz1/WhatToIbiza.txt:0
./written_2/travel_guides/berlitz1/WhatToIndia.txt:0
./written_2/travel_guides/berlitz1/WhatToIsrael.txt:0
./written_2/travel_guides/berlitz1/WhatToIstanbul.txt:0
./written_2/travel_guides/berlitz1/WhatToItaly.txt:0
./written_2/travel_guides/berlitz1/WhatToJamaica.txt:1
./written_2/travel_guides/berlitz1/WhatToJapan.txt:0
./written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:2
./written_2/travel_guides/berlitz1/WhatToLasVegas.txt:1
./written_2/travel_guides/berlitz1/WhatToLosAngeles.txt:0
./written_2/travel_guides/berlitz1/WhatToMadeira.txt:0
./written_2/travel_guides/berlitz1/WhatToMalaysia.txt:0
./written_2/travel_guides/berlitz1/WhatToMallorca.txt:0
./written_2/travel_guides/berlitz1/WhereToDublin.txt:0
./written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:2
./written_2/travel_guides/berlitz1/WhereToEgypt.txt:1
./written_2/travel_guides/berlitz1/WhereToFWI.txt:0
./written_2/travel_guides/berlitz1/WhereToFrance.txt:5
./written_2/travel_guides/berlitz1/WhereToGreek.txt:0
./written_2/travel_guides/berlitz1/WhereToHawaii.txt:0
./written_2/travel_guides/berlitz1/WhereToHongKong.txt:0
./written_2/travel_guides/berlitz1/WhereToIbiza.txt:0
./written_2/travel_guides/berlitz1/WhereToIndia.txt:2
./written_2/travel_guides/berlitz1/WhereToIsrael.txt:1
./written_2/travel_guides/berlitz1/WhereToIstanbul.txt:0
./written_2/travel_guides/berlitz1/WhereToItaly.txt:9
./written_2/travel_guides/berlitz1/WhereToJapan.txt:4
./written_2/travel_guides/berlitz1/WhereToJerusalem.txt:1
./written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:0
./written_2/travel_guides/berlitz1/WhereToMadeira.txt:0
./written_2/travel_guides/berlitz1/WhereToMadrid.txt:2
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt:1
./written_2/travel_guides/berlitz1/WhereToMallorca.txt:0
```
  - **What:** This command searched for how many times the word `pride` appeared in the all the txt files in the directory. 
  - **Why:** The command is useful since it is able to show which files have the word `pride` and how many times the word appears in the files that do have the word.
----

### 3. `grep -r` / `grep --recursive`
  - **What:** This command option greps all files in each directory recursively
  - **Why:** This is useful to grep all the files inside a directory with many different directories inside it, removing the need to go through each directory individually.
  - *Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/*

  - ***Example 1***
```console
[cs15lwi23aoa@ieng6-201]:skill-demo1-data:518$ grep -r "lotus" ./written_2/travel_guides          
./written_2/travel_guides/berlitz1/IntroIndia.txt:        whose navel a lotus grew bearing Brahma whose task it was to create the
./written_2/travel_guides/berlitz1/IntroIndia.txt:        world. Vishnu, a four-armed god with mace, conch, 
discus, and lotus,
./written_2/travel_guides/berlitz1/IntroIndia.txt:        white elephant holding a lotus flower in his trunk had entered her
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        highlights the emperor’s aesthetic, in the lotu 
 calyx on the gateway’s
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        gardens growing melons, tomatoes, cucumbers, and lotus root in a mesh
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        resting on the inverted lotus that once connected it to the pillar.
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        as well as plentiful trickling streams, lotus ponds, and lakes covered
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        lotus-covered bathing tank.
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        arms”) wielding bells, wheels, and lotus flowers. However,
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        a ring of giant lotus leaves, is Nara’s celebrated Daibutsu, or Great
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        white lotus blossoms. The myth-shrouded lakes are said to be the home
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        settlement beneath the surface. Outside lotu 
-blossom season, the lakes
./written_2/travel_guides/berlitz2/Bali-WhereToGo.txt:Museum Puri Lukisan is reached by a gateway across the road from the tourist office on Jalan Raya. In lush gardens, a fine hall has been built to house the works 
from the collection of the Dutch painter, Rudolf Bonnet, who helped guide the Pita Maha art movement in the 
1930s, and from the collection of his patron, Cokorda Gde Agung Sukawati, who governed Ubud for many decades. Look for the work of I Gusti Nyoman Lempad, one of the first artists to adopt Western techniques and bring the flat wayang figures of traditional painting to life. Remarkably, he was probably over 50 years old when he met Walter Spies and Bonnet (see page 53). Even he did not know his exact age. The museum’s estimate that he died in 1978 at the age of 115 may be an exaggeration. I Gusti Nyoman Lempad was chief architect and sculptor to the ruling Sukawati family of Ubud, and designed the Pura Saraswati temple, with its beautiful lotus pond and water garden, on Jalan Raya.
./written_2/travel_guides/berlitz2/China-WhereToGo.txt:The landscape beyond the palace compound features many of the romantic elements of Chinese tradition: interconnected lakes and lotus ponds, forests, causeways and arched bridges, ornate pavilions, and towering pagodas. The Tower of Mist and Rain (Yanyulou), a two-story lakeside pavilion in the southern style, was favored by emperors for its foggy views resembling those of an old Chinese painting. Tourists can cross the lakes in hand-poled ferryboats or drift at their own pace in a rowing boat. North of the lakes there are hiking trails in the Garden of Ten Thousand Trees (Wanahuyuan), where Emperor Qianlong gave an audience in 1793 to the first British ambassador to set foot in China, Lord Macartney. The meeting did not go well.
./written_2/travel_guides/berlitz2/China-WhereToGo.txt:One of the country’s best-known Buddhist monasteries, Hangzhou’s Lingyin Temple (“Spirits’ Retreat”), west of West Lake, attracts crowds of Chinese tourists and 
believers. The monks — for this is a working monastery — are kept busy supplying joss (incense) sticks to devout or merely fun-loving visitors. The main hall contains a statue of the Buddha seated on a lotus leaf. Carved of camphorwood, it is 191⁄2 m (64 ft) high and thought to be the largest such sculpture in China. Nearby, the “Peak That Flew from Afar” (Feilaifeng) shelters 380 Buddhist stone carvings created during the Yuan 
Dynasty and four sacred caves. The most famous sculpture is of the Laughing Buddha with a bulging belly, an 
animated figure fashioned about a thousand years ago.
./written_2/travel_guides/berlitz2/China-WhereToGo.txt:The subtleties of Tang-Dynasty art can be seen in the Qianqi cave temple, begun in the year 641, and in the Fengxian cave temple, constructed a few years later. 
The Fengxian cave shelters a 17-m (56-ft) Buddha, seated atop a thousand-petaled lotus and accompanied by lesser but equally brilliant statues of his disciples. The fierce, heavenly guard trampling a devil underfoot 
is thought to bring good luck to those who put their arms around his ankle, but an iron fence keeps most onlookers at bay.
./written_2/travel_guides/berlitz2/China-WhereToGo.txt:Yueyang (Yoyang), Hunan Province. Flamboyant upswept 
roofs surmount Yueyang Tower, a Tang landmark that has been rebuilt in Song Dynasty style. This three-tiered tower overlooks Lake Dongting, one of China’s biggest lakes. In summer months huge lotus flowers rise above the surface of the water. Junshan, an island in the lake endowed with many hills (and numerous legends), produces the rare and fragrant “silver needle” tea.
./written_2/travel_guides/berlitz2/Nepal-History.txt:Legend holds that the Kathmandu Valley was once a vast 
lake, upon which floated a giant lotus flower, from which emanated the light of Swayambhu, the primordial Buddha. When the Tibetan god Manjushri came to view this light, he was unable to get close enough for a good look, so he took his great sword and slashed through the mountains surrounding the valley to release the waters of the lake. (That is the myth. The fact, according to geologists, is that the Kathmandu Valley was indeed once a lake, though the valley’s waters now drain through the narrow cleft of Chobar Gorge, which was most likely created by a large earthquake.)
./written_2/travel_guides/berlitz2/Nepal-History.txt:In Nepal, both Hindu and Buddhist temples may take the 
pagoda form, but all the Indian-style stone shikara tower temples are Hindu and all the white dome-like stupas are Buddhist. The small trail-side shrines in the high mountains, called chortens, are also Buddhist, and often surrounded by stones carved with the Om mani padme hum incantation —  “Hail, jewel in the flower of the lotus.” Small stupas found around Buddhist and Hindu temples and known as chaityas are erected to hold relics or in memory of individuals.
./written_2/travel_guides/berlitz2/Nepal-History.txt:Vishnu, for example, can be Narayan, floating on the primeval ocean or lying on a bed of snakes. He is also Rama, the model prince and star of the Ramayana epic, and Krishna, a lusty hero who is the central figure of the Bhagavad Gita, a section of the Mahabharata epic. 
As Rama, he usually carries a bow and arrows. As Krishna, he is usually depicted with a blue face, an after-effect of swallowing a poison that threatened the world, and is often represented playing a flute or sporting with the milkmaids he seduced. As himself Vishnu is shown with four arms, holding a lotus, a club, a conch shell, and a disk, often seated on a snake, symbolizing eternity. Vishnu may appear in art as a fish, a tortoise, a boar, a man-lion, or a dwarf, the first five of his nine avatars. The ninth, according to some Hindus, was the Buddha. His tenth incarnation, to rescue the world from evil by destroying it and beginning a new cycle, is due about 540,000 years from now.
./written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt:The road north from Kathmandu leads 8 km (5 miles) to Budhanilkantha, and a giant statue of Vishnu reclining on a bed of snakes. Carved from one black stone and 
set in a sunken tank of water, the 5-m (16-ft) image dates from the seventh century. Legend has it that as Vishnu floated partly submerged in the primeval ocean, a lotus grew out of his navel, issuing Brahma, whose sole task was to create the world. The king cannot visit this shrine, as to look upon what is considered to be an image of himself, an incarnation of Vishnu, would be a forecast of death. On festival days worshippers 
blanket the statue with flowers. Beyond is Shivapuri Watershed and Wildlife Preserve, good place for a day hike.
```

  - **What:** This command option greps all files in directories within `./written_2/travel_guides` recursively for the word `lotus`.
  - **Why:** This is useful since it is able to look through all the txt files for `lotus` as long as they are within `travel_guides` or a sub-directory of `travel_guides`.

  - ***Example 2***
```console
[cs15lwi23aoa@ieng6-201]:skill-demo1-data:519$ grep --recursive "pride" ./written_2/travel_guides
./written_2/travel_guides/berlitz1/HistoryEgypt.txt:        national pride by wresting the Suez Canal out of British hands he
./written_2/travel_guides/berlitz1/HistoryEgypt.txt:        Limited success in 1973 restored some national pride when the Sinai was
./written_2/travel_guides/berlitz1/HistoryFWI.txt:        France in 1946 — a source of great pride to many. 
More importantly, it
./written_2/travel_guides/berlitz1/HistoryFrance.txt:        national pride sufficiently to oust the English from France 20 years
./written_2/travel_guides/berlitz1/HistoryFrance.txt:        the pride of the Louvre. A new opulent architecture blossomed with the
./written_2/travel_guides/berlitz1/HistoryFrance.txt:        pride found its perfect expression in the Eiffel Tower, thrust into the
./written_2/travel_guides/berlitz1/HistoryFrance.txt:        power in the national capital. By allowing the 
local pride of such
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt:        treasures with great pride. Edinburgh Castle is a treasure in
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt:        1707. The sense of an impending new era can be discerned in the pride,
./written_2/travel_guides/berlitz1/IntroFrance.txt:        pride, the nation’s cultural wealth is just as important. Philosophy
./written_2/travel_guides/berlitz1/IntroFrance.txt:        high technology and is happy to share its pride in these advances. With
./written_2/travel_guides/berlitz1/IntroItaly.txt:        sustains a solid and pugnacious local pride from historic division into
./written_2/travel_guides/berlitz1/IntroJamaica.txt:        within, working on a principle of pride in oneself and in one’s roots.
./written_2/travel_guides/berlitz1/WhatToJamaica.txt:        themselves and their culture with national pride.
./written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:        year. Family pride mixes with economics at these events. Farming can be
./written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:        for visitors and of pride to the farmers who breed and train them. Each
./written_2/travel_guides/berlitz1/WhatToLasVegas.txt:        pride.
./written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:        pride and designed as a mini-Parthenon, in deference to the
./written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:        take pride of place — the zoo has the world’s largest group in
./written_2/travel_guides/berlitz1/WhereToEgypt.txt:        A splendid Red granite sarcophagus has pride of 
place in
./written_2/travel_guides/berlitz1/WhereToFrance.txt:        metropolis. Renewed pride in France’s provincial cities is reducing
./written_2/travel_guides/berlitz1/WhereToFrance.txt:        pride.
./written_2/travel_guides/berlitz1/WhereToFrance.txt:        dialect, architecture, cuisine, and local prid 
 — the best of both
./written_2/travel_guides/berlitz1/WhereToFrance.txt:        centuries. But the museum’s pride and joy is its great ceramics
./written_2/travel_guides/berlitz1/WhereToFrance.txt:        textile, and industrial center with a bouncy pride, a taste for the
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        symbol of power and pride, was an understandable choice as the emblem
./written_2/travel_guides/berlitz1/WhereToIndia.txt:        pride is a 200-year-old banyan tree, the Ficus bengalensis, or
./written_2/travel_guides/berlitz1/WhereToIsrael.txt:        long climb to swell national pride, and army recruits are sworn in here
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        proclaims the inordinate but certainly justified civic pride of the
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        restaurants and boutiques, a vibrant local prid 
 nurtured by economic
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        chamber of the Nine Patricians), the full force 
of Siena’s civic pride
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        Annunciation and Madonna with Angels. But Umbria’s pride and joy is the
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        inspired Shakespeare. In Emilia-Romagna, the pride and creativity of
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        With an inherent pride so justifiably timeless, 
the
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        government to Rome, Milan prides itself on being the country’s
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        Titian, Correggio, and Tintoretto, pride of place — and a room to
./written_2/travel_guides/berlitz1/WhereToItaly.txt:        The pride of Turin, as in so many Italian cities, is not
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        Brooklynese. Ignore the proprieties — or offend 
the pride of an
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        waterfront itself is Nippon-maru Memorial Park, 
where pride of place
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        sprawling rival to the east. Osakans pride themselves on being warmer,
./written_2/travel_guides/berlitz1/WhereToJapan.txt:        The pride and joy of the neighborhood is the Meganebashi,
./written_2/travel_guides/berlitz1/WhereToJerusalem.txt:        and became the pride of the Jewish community in Palestine under British
./written_2/travel_guides/berlitz1/WhereToMadrid.txt:        Madrid’s pride, the Prado museum, is indisputably the
./written_2/travel_guides/berlitz1/WhereToMadrid.txt:        museum’s greatest pride, spotlighted in its own niche on the ground
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        Plant life. The pride of the mountain is its 
1,500
./written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt:An easy half-day outing is to Queluz, 14 km (8 miles) west of Lisbon on the way to Sintra (see below), home to the pretty pink palace commissioned by Pedro III. The sumptuous summer home was built in the second half of the 18th century and thrived during the reign of Maria I (1777–1799). The interior is a model of only slightly tattered splendor, but the exquisite Palace Gardens are the pride of Queluz, with imaginative fountains, and armies of statues.
./written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:The Dutch Royal barge (last used in 1962) is also kept in air-conditioned splendor, but perhaps pride of place — and certainly what brings 18th-century seafaring to life — is the re-creation of a Dutch East India ship The Amsterdam which sits in the dock outside. She is the life-size replica of a real ship completed in 1748, but more than this, The Amsterdam has a “press-ganged” crew to man her. As you explore her decks, the captain will illustrate his course with charts of the time, the doctor will explain his rather primitive treatments, and the ordinary seamen will be happy to sing you a Dutch sea shanty.
./written_2/travel_guides/berlitz2/Athens-Intro.txt:The Orthodox Church — for so long the one thing that united the Hellenic Diaspora — still has a strong influence on the population. Everyone from suited businessmen to young soldiers on national service make a regular visit to Athens Cathedral or a small local church to light a candle. People stop in on the way home from work or in their lunch breaks; it’s such a normal part of everyday life here. The Greek language also unifies the congregation with the clergy and Greeks around the 
world, though its use gives the capital a decidedly exotic air as visitors struggle to make sense of these “foreign” letters. There’s also a sense of patriotism and national pride here even among the young — perhaps 
brought about by political upheavals in the late 20th century. Since Greek democracy was restored in 1975, after the military dictatorship, it is as though the population relish their country all the more.
./written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt:On the ground floor, pride of place is given to a detailed model of Somers’s ship, Sea Venture. Many American visitors are also fascinated by a replica of a machine commissioned by the Congress of the Confederate States that stamped a seal for all their official documents. There is also a short video presentation called “Bermuda: Centre of the Atlantic,” which tells the story of the founding and development of the island. Climb the stairs to the first floor, where the so-called 
Rogues and Runners Museum presents a detailed exposition of Bermuda’s role in the American Civil War. Bermuda had many ties with the southern states through both business and family bloodlines. Although Britain officially remained neutral, Bermudians favored the South, wanting to help their friends — and make a lot of money in the process. A series of short information boards brings to life different aspects of this intriguing time in Bermuda’s history. Sadly, it also documents the true story of the blockade-runner Fannie, which returned from one trip in June 1864 with two sick crew members. The yellow fever they carried soon spread across 
Bermuda, killing many hundreds of people. Graves in the Royal Naval Cemetery (near the dockyard at the other end of Bermuda) offer testimony to some of the individuals who succumbed to this dreadful disease.
./written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt:Despite a recent cultural invasion from the West, Hungary still has a very active folk-music scene; and where there is music, dancing is never very far behind. Hungarian folk-dancing is well worth watching, and takes you through the whole gamut of courtly wedding dances to high-energy, boot-slapping “Lad’s Dances” from the 18th century. As ever it’s best to catch it at local festivals, where performers are there for the love of dancing or local pride, as opposed to the tourist dollar. In the same vein, look out for the real gypsy dancers who have vivacity associated with the likes of 
Andalucian ﬂamenco performers.
./written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:Tour guides are quick to point out the Loreto Chapel (immediately to the left of the entrance), where a red marble statue of the Virgin takes pride of place. At the east end of the church is the entrance to the crypt and the museum, which holds a ﬁne collection of medieval stone carvings, sacred relics, historic vestments, and religious paintings. The museum rambles up and down old staircases around the church, offering at one spot an excellent view down onto the nave.
./written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:Just as Tower Bridge is the toast of London, the Golden Gate is the pride of San Francisco, and the Brooklyn Bridge is a symbol of New York, Budapest too has its landmark river crossings.
./written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:The architectural pride of the Great Boulevard has 
to be the Museum of Applied Arts (Iparmuvészeti Múzeum), just off Ferenc körút at 33-37 Ülloi út. The exterior is a splendid example of Art Nouveau, incorporating Hungarian folk art styles and using Hungarian majolica tiles. Great green cupolas, small spiky towers, a majolica lantern, and a bright green and gold roof top the ensemble. The architect of the museum, Ödön Lechner, is regarded as the greatest exponent of this native 
form of Art Nouveau style. The interior is, if anything, even more remarkable. The style itself may best be 
described as fantasy Hungarian with strong Moorish inﬂuences. Shimmering white Arabian Nights-type arches, balconies, and swirling staircases sweep up to a ﬁne Art Nouveau skylight. The main hall is covered by a great expanse of glass supported by an iron frame, and ferns and potted plants around the hall create an exotic 
ambience.
./written_2/travel_guides/berlitz2/California-History.txt:The Great Depression hit California hard. Income from agriculture dropped by 50 percent between 1929 and 1932, and one-fifth of the state’s population was on 
public relief. California managed to weather the downturn better than the rest of the country, however, and 
became a magnet for dispossessed refugees from the Dustbowl of the Midwest. “Okies,” as they were known, packed their families and belongings into rickety cars and trucks to make the epic voyage west to find work in 
the farms and orchards of California. Their tale of hardship, pride, bitterness, and exploitation is graphically recorded in the Pulitzer Prize–winning novel The Grapes of Wrath, by California writer John Steinbeck. 
./written_2/travel_guides/berlitz2/California-WhereToGo.txt:The city’s pride and joy is the iron-hulled square-rigger Star of India, built in the Isle of Man in 1863. The Star is the oldest sailing ship that is still seaworthy; she makes a celebratory cruise twice each summer. A brief walk along the waterfront leads to Seaport Village, a lively complex of shops, restaurants, and galleries overlooking the harbor.
./written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:East of Yonge Street along Front, the Hummingbird Centre for the Performing Arts is a less-than-graceful concrete bunker that is home to the National Ballet of 
Canada and the Canadian Opera Company. Next door, Canadian drama, both contemporary and classical, is given 
pride of place at the St. Lawrence Centre for the Performing Arts. A block away at Jarvis Street, the sprawling indoor-outdoor St. Lawrence Market is open Tuesdays to Saturdays, with the flea market setting up its stalls here on Sundays. Buskers turn it into something of a genteel English country fair on the weekend. Nearby St. Lawrence Hall, once host to the freaks and darlings of Victorian vaudeville, has been beautifully restored to its original pink and green to provide a second home for the National Ballet.
./written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:The AGO’s Walker Gallery exhibits sculpture by fellow Briton Barbara Hepworth, as well as Rodin, Dégas, and Maillol. The European collection of paintings includes important works by Tintoretto, Rembrandt, Van Dyck, Rubens, Frans Hals, Jan van Goyen, and Poussin. An Ontario collection gives a prominent place to British painters, including Hogarth, Raeburn, Reynolds, and Gainsborough. Among the Impressionists and their followers represented here are Renoir, Pissarro, Monet, Cézanne, and Van Gogh. “Moderns” include Matisse, Picasso, and Braque. The Canadian collection provides a comprehensive survey of 200 years of Canadian painting, pride of place going to Emily Carr, Tom Thomson, and members 
of the influential Group of Seven.
./written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:Situated in the heart of the peninsula, 130 km (78 miles) or 2 hours’ drive from Toronto, Stratford town is well worth a visit for its celebrated Stratford Festival spanning the whole tourist season, from May to November. Since Tyrone Guthrie opened the festival in a 
tent in 1953, Shakespeare and other English classics such as Sheridan and Marlowe have been given pride of place. Their home is now the apron-staged Festival Theatre, while the Avon Theatre and Third Stage put on alternative fare, offering jazz and chamber-music concerts as well as a chance to discover Canadian playwrights.
./written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:As you travel from bilingual Montréal to New France’s old capital Québec City and the resolutely French-speaking farm villages along the St. Lawrence and around the Gaspé Peninsula, have a thought for local patriotic sensibility. The Québécois can justly claim to be cofounders of the Canadian nation. Abandoned by what many still call the “damned French” (maudits français), 
they felt that they alone had earned the name of canadiens, and that their British conquerors usurped it. As a tribute to their own past courage, there is both pride and resentment in the Québécois motto “Je me souviens” (“I Remember”). It was they who made the first and hardiest effort to hew a modern living out of this hard land. Like colonials everywhere, their missionaries sometimes brought more religion, their traders more 
alcohol, and their soldiers more guns than the natives really needed. But the Québécois understood the importance of learning from the native peoples how best to handle the Canadian wilderness. Fur-trading coureurs de bois settled down with Indian wives, and today more than a few Québécois proudly trace their ancestry back to native peoples with a tell-tale birthmark on the hip, high cheekbones, or long sleek black hair.        
./written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:Outside Montréal, you can’t assume everyone speaks English. Many make it a point of pride not to, until you’ve at least paid them the courtesy of a “Bonjour.” By Québec provincial law, public signs are all in French, and so we will often give you here, beside the English names, the French version as it appears on maps and signposts.
./written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:Get away from the city center with an excursion out 
to Point Grey. You can relax on the pleasant beaches; Wreck Beach is reserved for nudists. The grounds of the University of British Columbia, one of the most beautiful college campuses in North America, are nearby; the terraced Sedgwick Library and the Faculty Club rose garden are two notable gems set against a superb sea 
and mountain backdrop. The university’s pride and joy is the great Museum of Anthropology, out on Marine Drive at Point Grey. Arthur Erickson designed this noble glass and concrete-beam structure in 1972 as an explicit homage to the post-and-beam longhouses of the Northwest Coast Indians. Gracing the lawns are a magnificent group of totem poles and two cedarwood houses of the Haida Indians, built in the 1930s and faithful to a centuries-old technique and form.
./written_2/travel_guides/berlitz2/China-WhereToGo.txt:Nanjing’s distinguished history as a political and cultural center accounts for its considerable local pride. One area in which rivalry is freely revealed is the realm of cooking. Nanjing claims its salted duck is superior to the more famous Peking duck. Nanjing ducks, it’s pointed out, are raised naturally on ponds, not force-fed like their less fortunate Beijing comrades. 
./written_2/travel_guides/berlitz2/Costa-WhereToGo.txt:A couple of kilometers (about a mile) inland and high above the sea lies the village of Benalmádena-Pueblo. Its Museo Arqueológico y de Arte Colombino is an institution of national importance. The museum takes pride in its collection of Pre-Columbian art (said to be the most important of its kind in Spain), with jewelry, statuary, and ceramics from all the major cultures. Also in the Benalmádena area is the Tívoli World amusement park, in the suburb of Arroyo de la Miel (see page 
91), the Sea Life aquarium in the Puerto Deportivo, and the Eagle Park at the Colomares Castle.
./written_2/travel_guides/berlitz2/Costa-WhereToGo.txt:Northeast of the mosque on the Plaza Jerónimo Paéz, the splendid Renaissance Palacio Paéz houses the Museo Arqueológico Provincial. The exhibits span the centuries from the Iberian era to the Visigothic period, but pride of place goes to objects from the 10th-century palace of Medina Azahara, like the bronze figure of a stag taken from a fountain presented by the Byzantine emperor Constantine VII.
./written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt:In the tablaos and on the stage, the women, their hair swept severely back, swirl in flounced and flowing tight-waisted dresses. The men perform in the Cordoban suit — slightly flared, high-waisted trousers, frilled shirt, and short jacket. These traditional costumes, and the fervent pride of the performers who wear them, make for a colourful spectacle without equal on 
the cabaret stage.
./written_2/travel_guides/berlitz2/Paris-WhatToDo.txt:Among spectator sports, pride of place goes to horse-racing. The summer meetings at Longchamp (venue of the Prix de l’Arc de Triomphe), Auteuil, and Chantilly are as elegant as Britain’s Ascot. The serious punter who wants to avoid the frills and Champagne can have a very good time at Vincennes and Enghien trotting races.
./written_2/travel_guides/berlitz2/Poland-History.txt:By the end of the 20th century, Poland had joined NATO, and a decision on EU membership was expected by 2003. Poland is thought by most experts to be among the few countries that will be allowed to join in the first round of decisions. In June 1999, Pope John Paul II visited his homeland for the eighth time as Pope, and he was again received by enormous crowds, proof once again that Poland’s committed Catholics and fervent patriots had survived the Communist years with their faith 
and pride intact.
./written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt:Just 14 km (8 miles) west of Lisbon is the Palacio Nacional de Queluz, home to the pretty pink palace commissioned by Pedro III. The sumptuous summer palace was built in the second half of the 18th century as an official working residence for the royal family. The Palace Gardens are the pride of Queluz, with clipped hedges in perfect geometric array, imaginative fountains, and armies of statues.
./written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt:San Juan “never closes,” they say, with pride. And they’re absolutely right. Even at sunrise, you’ll see bright-eyed people heading for an early breakfast after spending all night at a discotheque or nightclub that stays open until the last patron departs.
```

  - **What:** This command option greps all files in directories within `./written_2/travel_guides` recursively for the word `pride`.
  - **Why:** This is useful since it is able to look through all the txt files for `pride` as long as they are within `travel_guides` or a sub-directory of `travel_guides`.

----

4. `grep -l` / `grep --files-with-matches` 
  - **What:** This command option prints the name of the file that has the match
  - **Why:** This is useful when only the path or name of the file is needed and it is also easier to read since the text isn't shown.
  - *Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/*

  - ***Example 1***
```console
[cs15lwi23aoa@ieng6-201]:skill-demo1-data:527$ grep -l "lotus" ./written_2/travel_guides/berlitz1/*.txt     
./written_2/travel_guides/berlitz1/IntroIndia.txt
./written_2/travel_guides/berlitz1/WhereToIndia.txt
./written_2/travel_guides/berlitz1/WhereToJapan.txt
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt
```
  - **What:** This command option printed the name of the files had the word `lotus` in them.
  - **Why:** This is useful since it printed the file names that have `lotus` in them. 

  - ***Example 2***
```console
[cs15lwi23aoa@ieng6-203]:skill-demo1-data:504$ grep --files-with-matches "pride" ./written_2/travel_guides/berlitz1/*.txt
./written_2/travel_guides/berlitz1/HistoryEgypt.txt
./written_2/travel_guides/berlitz1/HistoryFWI.txt
./written_2/travel_guides/berlitz1/HistoryFrance.txt
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt
./written_2/travel_guides/berlitz1/IntroFrance.txt
./written_2/travel_guides/berlitz1/IntroItaly.txt
./written_2/travel_guides/berlitz1/IntroJamaica.txt
./written_2/travel_guides/berlitz1/WhatToJamaica.txt
./written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt
./written_2/travel_guides/berlitz1/WhatToLasVegas.txt
./written_2/travel_guides/berlitz1/WhereToEdinburgh.txt
./written_2/travel_guides/berlitz1/WhereToEgypt.txt
./written_2/travel_guides/berlitz1/WhereToFrance.txt
./written_2/travel_guides/berlitz1/WhereToIndia.txt
./written_2/travel_guides/berlitz1/WhereToIsrael.txt
./written_2/travel_guides/berlitz1/WhereToItaly.txt
./written_2/travel_guides/berlitz1/WhereToJapan.txt
./written_2/travel_guides/berlitz1/WhereToJerusalem.txt
./written_2/travel_guides/berlitz1/WhereToMadrid.txt
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt
```

  - **What:** This command option printed the name of the files had the word `pride` in them.
  - **Why:** This is useful since it printed the file names that have `lotus` in them. 
