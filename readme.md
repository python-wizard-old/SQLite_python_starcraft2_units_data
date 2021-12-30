# SQLite python Starcraft 2

## English
This project shows the usage of SQLite with python. 

To create, modify and communicate with the SQLite database from within python I'll use the SQLite3 library that comes by default with python.

The content of the database I'll be working on will be statistics of the units from the Starcraft 2 game. Reason being that working with some mock data is not that interesting to me, so in order to keep it more interesting and not just create dummy 'customer' or 'celebrity' tables I will create a table where I INSERT few of the terran units with simplified stats.

Starcraft 2 is an RTS (Real Time Strategy) game, where the commander(player) controls various kinds of units. The goal of the game is to build attacking units to destroy all of the opponents buildings. To achieve that goal one can improve one's economy by creating more workers and expand to more bases. That's where statistics of the units come into play. The damage, speed, etc. of each unit has profound effect on the game and that's what I want to explore.

There are several jupyter notebooks that either do the actual SQL modifications or perform tasks that are needed for the SQL work (like spraping page of liquipedia using pandas and 'exporting' it to a SQLite database).

Here is the description of what do I actually do in each notebook.

#### [SQLite_basic_operations_SC2units.ipynb](SQLite_basic_operations_SC2units.ipynb)

Here I create some close to real data for Starcraft 2 terran units. I create a database and enter 4 rows each corresponding to one unit type, with 5 columns, including name and excluding rowid. In reality terran race in Starcraft 2 has about 23 units (depends on what you actually count as a unit or as a building) and each unit has close to 20 characterists, depending on race (which boil down to columns in a Starcraft 2 game). 

This mock data is saved in the data/sc2_basic_units.db file.

Here I want to show basic SQL skills that are most basic and most commonly used but the data is mock data (even though it's based on real data). In this notebook I'm not exploring or solving any real problem. Just basic SQL stuff :)



#### [units_sc2_scraping.ipynb](units_sc2_scraping.ipynb)

Here I scrape data from the Liquipedia website section with all the data about Starcraft 2 units. Liquipedia is one of the best encyclopedias about Starcraft franchise and other esport games. Below is the exact address of the scraped page:
https://liquipedia.net/starcraft2/Unit_Statistics_(Legacy_of_the_Void)

The data is saved in the sc2_data.db. Here the goal is just to get the data of the webpage and save it to the database. I'll actually work on the data in the next notebook.










## Polski


Starcraft 2 jest grą RTS (Strategia czasu rzeczywistego) gdzie gracz zarządza jedną z trzech ras. Celem gry jest wytrenowanie jednostek atakujących w celu zniczszenia budynków przeciwnika. Gracz może zwiększyć swoje zasoby poprzez tworzenie więcej jednostek zbierających zasoby i rozbudowania swojej bazy.
W tym zeszycie będę dodawał wiersze do tabeli terran_units odpowiadające uproszczonym statystykom 4 jednostek terrana.
