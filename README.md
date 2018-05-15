# Video Games Distribution Database

Problem Definition:
A company needs a database for selling video games and extra programs for these games. Company wants to record users, their games and communities about these games. The database should have also game companies, genres of the games and should show special offers of the games and other products.

Requirements:
This database system has to have following objects and their entrys to record information.
1)	User Information
-User name
-Password
-Games which have bought by this user (if exist)
-Communities which have subscribed and have been as admin (if exist)

2)	Games
-Name of the games
-Genre(s)
-Price
-age limit(if exist)
-Extra programs for developing(DLCs etc.) (if exist)

3)	Communities
-Community name
-Subscribers
-Group admin

4)	Game Companies
-Company name
-Games of the company

5)	Extra Programs
*Extra Programs are to make the games playing ,display or sounds better.
-Name of the Program
-Games which are related the program

6)	Special Offers(if exist)
-Offer rate(%50-40 etc.)

Constraints-Requirements:

A user can purchased many extra programs and an extra program can be purchased by many users, so there will be a many to many relationship between these entities. It will be the same for entitites which are user and game. 
A user can be admin of many communities also a community can be subscribed by many users, it should use many-to-many relationship between them. However a community cannot be exists if it hasn't any admin. So between this relation community entity must have total participation.
 An extra program must be related with a game, that's why it has a total participation. Because of that a game can have more than one extra program, there will be many-to-one relationship(program-game).
A game can be exist if and only if it is owned by a game company, so there is a total participation to game entity. A game can be owned by only one company, however a company can own many games. So it is many to one relationship(game-company).
Special offers can be exists if and only if a game or an extra program is in a special offer. So it is an total participation and many programs or games can be in same offer category. So it is the many to one relationship.

In E-R Diagram,
Primary keys are red.
Entities are blue.
Relationship Sets are purple.
Primary keys are red.
Derived Attributes are yellow and dashed.
Total participations are double lines.

Functionalities of the Database:
•	Users can show their owned games.
•	A user can check a specific company's games.
•	Users can check special offers.
•	Users can check on the games by genre, age limit etc.
•	People can subscribe as a user or an admin to communities.
•	Users can search games by price.
•	And many other operations can be handled by this system.
