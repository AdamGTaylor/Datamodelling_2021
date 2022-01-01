# Read Me: Datamodelling and Databases (2021) Project Repository
# Acquaintance Network of the Marvel Cinematic Universe

    Advisor : János Báskay
    Course Leader : Péter Pál Pollner

## --- Description ---

    The dataset provides information about the dialogues between Marvel characters,
    information about which movie has which character in it.

    -> data / characters.csv  # characters per film
    -> data / mcu.csv         # transcript
 
## --- Dataset ---

    https://www.kaggle.com/pdunton/marvel-cinematic-universe-dialogue


## --- Tools ---

    Jupyter Notebook (python3)
    SQL (mysql)


## --- NOTES --

    The MYSQL server is hosted locally and installed on a my machine.

    The table is created by:
        create table linklist (
            uuid1 varchar(255) NOT NULL,
            uuid2 varchar(255) NOT NULL
        );

    The way the .csv files is loaded is:
        load data infile 'data\_linklist.csv'
        into table linklist
        fields terminated by ','
        lines terminated by '\n'
        ignore 1 rows;
    
    The location of the file is:
        C:\ProgramData\MySQL\MySQL Server 8.0\Data\data