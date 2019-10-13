Results of Danish General Elections 1953-2019
---

### Description

Results of Danish General Elections 1953-2019 including number of votes and number of seats in parliament. Election results from Greenland and the Faroe Islands are not included.

### Parties

|       | Party name in Danish         | Party name in English |
| ----- | ---------------------------- | --------------------------------- |
| S     | Socialdemokratiet            | The Social Democratic Party |
| RV    | Det Radikale Venstre         | The Social Liberal Party |
| K     | Det Konservative Folkeparti  | The Conservative People's Party |
| CD    | Centrum-Demokraterne         | The Centre Democrats |
| Rfb   | Retsforbundet                | The Justice Party |
| SF    | Socialistisk Folkeparti      | Socialist People's Party |
| DKP   | Danmarks Kommunistiske Parti | Communist Party of Denmark |
| DF    | Dansk Folkparti              | Danish People's Party |
| FK    | Fælles Kurs                  | Common Course |
| LC    | Liberalt Centrum             | Liberal Centre |
| KD    | Kristendemokraterne          | The Christian Democrats |
| SP    | Slesvigsk Parti              | Schleswig Party |
| U     | De Uafhængige                | The Independents |
| V     | Venstre                      | The Liberal Party |
| VS    | Venstresocialisterne         | The Left Socialists |
| FP    | Fremskridtspartiet           | The Progress Party |
| EL    | Enhedslisten                 | The Red-Green Alliance |
| LA    | Liberal Alliance             | Liberal Alliance |
| Alt   | Alternativet                 | The Alternativ |
| NB    | Nye Borgerlige               | The New Right |
| KRP   | Klaus Riskær Pedersen        | Klaus Riskær Pedersen |
| SK    | Stram Kurs                   | Hard Line Party |


### Repository content

The `votes.csv` data file consists of the following variables:

- `year` = The year of the election
- `party_s` = Number of votes for the Social Democratic Party
- `party_rv` = Number of votes for the Social Liberal Party
- `party_k` = Number of votes for the Conservative People's Party
- `party_cd` = Number of votes for the Centre Democrats
- `party_rfb` = Number of votes for the Justice Party
- `party_sf` = Number of votes for the Socialist People's Party
- `party_dkp` = Number of votes for the Communist Party of Denmark
- `party_df` = Number of votes for the Danish People's Party
- `party_fk` = Number of votes for Common Course
- `party_lc` = Number of votes for Liberal Centre
- `party_kd` = Number of votes for the Christian Democrats
- `party_sp` = Number of votes for the Schleswig Party
- `party_u` = Number of votes for the Independents
- `party_v` = Number of votes for the Liberal Party
- `party_vs` = Number of votes for the Left Socialists
- `party_fp` = Number of votes for the Progress Party 
- `party_el` = Number of votes for the Red-Green Alliance
- `party_la` = Number of votes for the Liberal Alliance
- `party_alt` = Number of votes for the Alternative
- `party_nb` = Number of votes for the New Right
- `party_krp` = Number of votes for Klaus Riskær Pedersen
- `party_sk` = Number of votes for the Hard Line Party
- `other_valid` = Number of votes for other parties and independents
- `total_valid` = Total number of valid votes
- `blank` = Number of blank votes
- `other_invalid` = Number of invalide votes besides blank votes
- `total_invalid` = Total number of invalid votes
- `total_votes` = Total number of votes cast
- `electorate` = Size of electorate

The `seats.csv` data file consists of the following variables:

- `year` = The year of the election
- `party_s` = Number of seats won by for the Social Democratic Party
- `party_rv` = Number of seats won by for the Social Liberal Party
- `party_k` = Number of seats won by for the Conservative People's Party
- `party_cd` = Number of seats won by for the Centre Democrats
- `party_rfb` = Number of seats won by for the Justice Party
- `party_sf` = Number of seats won by for the Socialist People's Party
- `party_dkp` = Number of seats won by for the Communist Party of Denmark
- `party_df` = Number of seats won by for the Danish People's Party
- `party_fk` = Number of seats won by for Common Course
- `party_lc` = Number of seats won by for Liberal Centre
- `party_kd` = Number of seats won by for the Christian Democrats
- `party_sp` = Number of seats won by for the Schleswig Party
- `party_u` = Number of seats won by for the Independents
- `party_v` = Number of seats won by for the Liberal Party
- `party_vs` = Number of seats won by for the Left Socialists
- `party_fp` = Number of seats won by for the Progress Party 
- `party_el` = Number of seats won by for the Red-Green Alliance
- `party_la` = Number of seats won by for the Liberal Alliance
- `party_alt` = Number of seats won by for the Alternative
- `party_nb` = Number of seats won by the New Right
- `party_krp` = Number of seats won by Klaus Riskær Pedersen
- `party_sk` = Number of seats won by the Hard Line Party
- `other` = Number of seats won by other parties and independents
- `total` = Total number of seats in parliament

The following commands will load the data into R:
``` R
# seats dataset
read.csv(text=RCurl::getURL("https://raw.githubusercontent.com/Straubinger/folketingsvalg/master/seats.csv"))
# votes dataset
read.csv(text=RCurl::getURL("https://raw.githubusercontent.com/Straubinger/folketingsvalg/master/votes.csv"))
```

### Sources

- <a href="http://www.dst.dk/da/Statistik/Publikationer/VisPub?pid=1696">Danmarks Statistik Publikationer 1953-2007</a>
- <a href="http://www.dst.dk/da/Statistik/Publikationer/VisPub?pid=1532">Danmarks Statistik Publikationer 2011-2015</a>
- <a href="https://www.dst.dk/valg/index.htm">Danmarks Statistik Valghjemmeside 2011-2019</a>
