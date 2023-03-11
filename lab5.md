# Command: `find`
## 4 *find* command options
### 1. `find <file-path> -name <text>`
  - **What:** This command option finds the file with the specific name.
  - **Why:** This is useful when you are looking for a file with the exact name.
  - *Source: https://www.geeksforgeeks.org/find-command-in-linux-with-examples/*

#### - ***Example 1***
```console
[cs15lwi23aoa@ieng6-202]:berlitz1:590$ find . -name IntroEgypt.txt
./IntroEgypt.txt
```
  
  - **What:** This command searched for files with the title `IntroEgypt.txt`. 
  - **Why:** The command is useful since it found files with the specified name. 



#### - ***Example 2***
```console
[cs15lwi23aoa@ieng6-202]:berlitz1:514$ find . -name HistoryJamaica.txt
./HistoryJamaica.txt
```
  - **What:** This command searched for files with the title `HistoryJamaica.txt`. 
  - **Why:** The command is useful since it found files with the specified name. 

----

### 2. `find <file-path> -type <file-type>`
  - **What:** This command option finds the file with the specified type.
  - **Why:** This is useful when you are looking for files of a specific type. 
  - *Source: https://www.geeksforgeeks.org/find-command-in-linux-with-examples/*

#### - ***Example 1***
```console
[cs15lwi23aoa@ieng6-202]:skill-demo1-data:579$ find written_2 -type d
written_2
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Castro
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Rybczynski
written_2/travel_guides
written_2/travel_guides/berlitz1
written_2/travel_guides/berlitz2
```
  - **What:** This command searched for all the directories in the directory. 
  - **Why:** The command is useful since it is able to show which directories are in a directory.


#### - ***Example 2***
```console
[cs15lwi23aoa@ieng6-202]:skill-demo1-data:582$ find written_2 -type f  
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written_2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch3.txt
written_2/non-fiction/OUP/Abernathy/ch6.txt
written_2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/ch9.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch7.txt
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chC.txt
written_2/non-fiction/OUP/Castro/chL.txt
written_2/non-fiction/OUP/Castro/chM.txt
written_2/non-fiction/OUP/Castro/chN.txt
written_2/non-fiction/OUP/Castro/chO.txt
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/chQ.txt
written_2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chV.txt
written_2/non-fiction/OUP/Castro/chW.txt
written_2/non-fiction/OUP/Castro/chY.txt
written_2/non-fiction/OUP/Castro/chZ.txt
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch10.txt
written_2/non-fiction/OUP/Fletcher/ch2.txt
written_2/non-fiction/OUP/Fletcher/ch5.txt
written_2/non-fiction/OUP/Fletcher/ch6.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch10.txt
written_2/non-fiction/OUP/Kauffman/ch3.txt
written_2/non-fiction/OUP/Kauffman/ch4.txt
written_2/non-fiction/OUP/Kauffman/ch5.txt
written_2/non-fiction/OUP/Kauffman/ch6.txt
written_2/non-fiction/OUP/Kauffman/ch7.txt
written_2/non-fiction/OUP/Kauffman/ch8.txt
written_2/non-fiction/OUP/Kauffman/ch9.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch3.txt
written_2/travel_guides/berlitz1/HandRHawaii.txt
written_2/travel_guides/berlitz1/HandRHongKong.txt
written_2/travel_guides/berlitz1/HandRIbiza.txt
written_2/travel_guides/berlitz1/HandRIsrael.txt
written_2/travel_guides/berlitz1/HandRIstanbul.txt
written_2/travel_guides/berlitz1/HandRJamaica.txt
written_2/travel_guides/berlitz1/HandRJerusalem.txt
written_2/travel_guides/berlitz1/HandRLakeDistrict.txt
written_2/travel_guides/berlitz1/HandRLasVegas.txt
written_2/travel_guides/berlitz1/HandRLisbon.txt
written_2/travel_guides/berlitz1/HandRLosAngeles.txt
written_2/travel_guides/berlitz1/HandRMadeira.txt
written_2/travel_guides/berlitz1/HandRMadrid.txt
written_2/travel_guides/berlitz1/HandRMallorca.txt
written_2/travel_guides/berlitz1/HistoryDublin.txt
written_2/travel_guides/berlitz1/HistoryEdinburgh.txt
written_2/travel_guides/berlitz1/HistoryEgypt.txt
written_2/travel_guides/berlitz1/HistoryFWI.txt
written_2/travel_guides/berlitz1/HistoryFrance.txt
written_2/travel_guides/berlitz1/HistoryGreek.txt
written_2/travel_guides/berlitz1/HistoryHawaii.txt
written_2/travel_guides/berlitz1/HistoryHongKong.txt
written_2/travel_guides/berlitz1/HistoryIbiza.txt
written_2/travel_guides/berlitz1/HistoryIndia.txt
written_2/travel_guides/berlitz1/HistoryIsrael.txt
written_2/travel_guides/berlitz1/HistoryIstanbul.txt
written_2/travel_guides/berlitz1/HistoryItaly.txt
written_2/travel_guides/berlitz1/HistoryJamaica.txt
written_2/travel_guides/berlitz1/HistoryJapan.txt
written_2/travel_guides/berlitz1/HistoryJerusalem.txt
written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt
written_2/travel_guides/berlitz1/HistoryLasVegas.txt
written_2/travel_guides/berlitz1/HistoryMadeira.txt
written_2/travel_guides/berlitz1/HistoryMadrid.txt
written_2/travel_guides/berlitz1/HistoryMalaysia.txt
written_2/travel_guides/berlitz1/HistoryMallorca.txt
written_2/travel_guides/berlitz1/IntroDublin.txt
written_2/travel_guides/berlitz1/IntroEdinburgh.txt
written_2/travel_guides/berlitz1/IntroEgypt.txt
written_2/travel_guides/berlitz1/IntroFWI.txt
written_2/travel_guides/berlitz1/IntroFrance.txt
written_2/travel_guides/berlitz1/IntroGreek.txt
written_2/travel_guides/berlitz1/IntroHongKong.txt
written_2/travel_guides/berlitz1/IntroIbiza.txt
written_2/travel_guides/berlitz1/IntroIndia.txt
written_2/travel_guides/berlitz1/IntroIsrael.txt
written_2/travel_guides/berlitz1/IntroIstanbul.txt
written_2/travel_guides/berlitz1/IntroItaly.txt
written_2/travel_guides/berlitz1/IntroJamaica.txt
written_2/travel_guides/berlitz1/IntroJapan.txt
written_2/travel_guides/berlitz1/IntroJerusalem.txt
written_2/travel_guides/berlitz1/IntroLakeDistrict.txt
written_2/travel_guides/berlitz1/IntroLasVegas.txt
written_2/travel_guides/berlitz1/IntroLosAngeles.txt
written_2/travel_guides/berlitz1/IntroMadeira.txt
written_2/travel_guides/berlitz1/IntroMadrid.txt
written_2/travel_guides/berlitz1/IntroMalaysia.txt
written_2/travel_guides/berlitz1/IntroMallorca.txt
written_2/travel_guides/berlitz1/JungleMalaysia.txt
written_2/travel_guides/berlitz1/WhatToDublin.txt
written_2/travel_guides/berlitz1/WhatToEdinburgh.txt
written_2/travel_guides/berlitz1/WhatToEgypt.txt
written_2/travel_guides/berlitz1/WhatToFWI.txt
written_2/travel_guides/berlitz1/WhatToFrance.txt
written_2/travel_guides/berlitz1/WhatToGreek.txt
written_2/travel_guides/berlitz1/WhatToHawaii.txt
written_2/travel_guides/berlitz1/WhatToHongKong.txt
written_2/travel_guides/berlitz1/WhatToIbiza.txt
written_2/travel_guides/berlitz1/WhatToIndia.txt
written_2/travel_guides/berlitz1/WhatToIsrael.txt
written_2/travel_guides/berlitz1/WhatToIstanbul.txt
written_2/travel_guides/berlitz1/WhatToItaly.txt
written_2/travel_guides/berlitz1/WhatToJamaica.txt
written_2/travel_guides/berlitz1/WhatToJapan.txt
written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt
written_2/travel_guides/berlitz1/WhatToLasVegas.txt
written_2/travel_guides/berlitz1/WhatToLosAngeles.txt
written_2/travel_guides/berlitz1/WhatToMadeira.txt
written_2/travel_guides/berlitz1/WhatToMalaysia.txt
written_2/travel_guides/berlitz1/WhatToMallorca.txt
written_2/travel_guides/berlitz1/WhereToDublin.txt
written_2/travel_guides/berlitz1/WhereToEdinburgh.txt
written_2/travel_guides/berlitz1/WhereToEgypt.txt
written_2/travel_guides/berlitz1/WhereToFWI.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz1/WhereToGreek.txt
written_2/travel_guides/berlitz1/WhereToHawaii.txt
written_2/travel_guides/berlitz1/WhereToHongKong.txt
written_2/travel_guides/berlitz1/WhereToIbiza.txt
written_2/travel_guides/berlitz1/WhereToIndia.txt
written_2/travel_guides/berlitz1/WhereToIsrael.txt
written_2/travel_guides/berlitz1/WhereToIstanbul.txt
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToJapan.txt
written_2/travel_guides/berlitz1/WhereToJerusalem.txt
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt
written_2/travel_guides/berlitz1/WhereToMadeira.txt
written_2/travel_guides/berlitz1/WhereToMadrid.txt
written_2/travel_guides/berlitz1/WhereToMalaysia.txt
written_2/travel_guides/berlitz1/WhereToMallorca.txt
written_2/travel_guides/berlitz2/Algarve-History.txt
written_2/travel_guides/berlitz2/Algarve-Intro.txt
written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt
written_2/travel_guides/berlitz2/Amsterdam-History.txt
written_2/travel_guides/berlitz2/Amsterdam-Intro.txt
written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt
written_2/travel_guides/berlitz2/Athens-History.txt
written_2/travel_guides/berlitz2/Athens-Intro.txt
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
written_2/travel_guides/berlitz2/Bahamas-History.txt
written_2/travel_guides/berlitz2/Bahamas-Intro.txt
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
written_2/travel_guides/berlitz2/Bali-History.txt
written_2/travel_guides/berlitz2/Bali-WhatToDo.txt
written_2/travel_guides/berlitz2/Bali-WhereToGo.txt
written_2/travel_guides/berlitz2/Barcelona-History.txt
written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt
written_2/travel_guides/berlitz2/Beijing-History.txt
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt
written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt
written_2/travel_guides/berlitz2/Berlin-History.txt
written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt
written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt
written_2/travel_guides/berlitz2/Bermuda-history.txt
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt
written_2/travel_guides/berlitz2/Budapest-History.txt
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt
written_2/travel_guides/berlitz2/California-History.txt
written_2/travel_guides/berlitz2/California-WhatToDo.txt
written_2/travel_guides/berlitz2/California-WhereToGo.txt
written_2/travel_guides/berlitz2/Canada-History.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/CanaryIslands-History.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
written_2/travel_guides/berlitz2/Cancun-History.txt
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt
written_2/travel_guides/berlitz2/China-History.txt
written_2/travel_guides/berlitz2/China-WhatToDo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
written_2/travel_guides/berlitz2/Costa-History.txt
written_2/travel_guides/berlitz2/Costa-WhatToDo.txt
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt
written_2/travel_guides/berlitz2/CostaBlanca-History.txt
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
written_2/travel_guides/berlitz2/Crete-History.txt
written_2/travel_guides/berlitz2/Crete-WhatToDo.txt
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
written_2/travel_guides/berlitz2/Cuba-History.txt
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
written_2/travel_guides/berlitz2/Nepal-History.txt
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt
written_2/travel_guides/berlitz2/NewOrleans-History.txt
written_2/travel_guides/berlitz2/Paris-WhatToDo.txt
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
written_2/travel_guides/berlitz2/Poland-History.txt
written_2/travel_guides/berlitz2/Poland-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-History.txt
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
written_2/travel_guides/berlitz2/PuertoRico-History.txt
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt
written_2/travel_guides/berlitz2/Vallarta-History.txt
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt
```
  - **What:** This command searched for all the files in the directory. 
  - **Why:** The command is useful since it is able to show which files are in a directory.

----

### 3. `find <path> -atime <days>`
  - **What:** This command option finds all files in the path that have been accessed back certain days
  - **Why:** This is useful to find which files have been accessed most recently in a directory.
  - *Source: https://www.tecmint.com/35-practical-examples-of-linux-find-command/*

- ***Example 1***
```console
[cs15lwi23aoa@ieng6-202]:berlitz1:609$ find . -atime 0
.
./HistoryIsrael.txt
```

  - **What:** This command option finds all files in directories within `./written_2/travel_guides/berlitz1` for files accessed back 0 days. Since I opened HistoryIsrael.txt recently, it prints that.
  - **Why:** This is useful since it is able to see which files have been accessed recently or until a certain day. It can keep a history on the files.

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

### 4. `grep -l` / `grep --files-with-matches` 
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
  - **Why:** This is useful since it printed the file names that have `pride` in them. 
