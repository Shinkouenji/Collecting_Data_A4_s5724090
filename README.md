## Annotation of Dutch party programs for the 2023 elections.

### The corpus

The corpus I collected consists of 10 party programs of Dutch political parties. The programs are from the elections in 2023. The corpus contains the programs of 10 political parties. I will elaborate in the data collection process on which parties and why those are included in the corpus.

### The target audience

The target audience is researchers who want to do textual analysis of Dutch political party programs. This corpus contains some of the major political parties’ programs, from left-wing to right-wing. As will be elaborated on in the metadata, the current amount of seats in the House of Representatives, or Tweede Kamer in Dutch, and the percentage of votes in the national election of 2023 are included in the metadata. This information was taken from [here](https://nl.wikipedia.org/wiki/Tweede_Kamerverkiezingen_2023).

### Text selection criteria

To be able to research left-wing and right-wing differences I wanted to include as many parties from both ideologies as possible. One challenge I found here is that even though parties identified themselves as left-wing, they would showcase some very right-wing traits such as DENK, which is pro-castration of pedophiles even though self-identifying as left-wing. Another challenge was trying to equally represent left-wing and right-wing. Left-wing and right-wing are not exact measure criteria. What is considered left-wing and right-wing will have different connotations per country and thus my identification of left-wing or right-wing is up for discussion as well. 

### The data collection process

I copied the party programs excluding the introductions and epilogue as only to retain the political plans of the party. I used [this](https://www.zokiesje.nl/nieuws/?item=285&nieuws=Overzicht_partijprogrammas) website which contains all party programs. I pasted the text into a text file and created a directory in my computer with the 10 programs. The metadata was gathered from [here](https://nl.wikipedia.org/wiki/Tweede_Kamerverkiezingen_2023). I included the metadata of current seats in the House of Representatives and percentage of votes because it might help in research about what prominent parties are saying, regardless of them being left-wing or right-wing.

### Metadata

| metadata | description |
| ------ | ----------- |
| file_name | the filename in the directory |
| party_name |The full name of the party in Dutch |
| left_right | Whether the party is left-wing or right-wing |
|current_seats_hop | The amount of seats won in the elections of 2023 in the House of Representatives ('Tweede Kamer' in Dutch ) |
| percent_votes | Percentage of votes the party earned in the elections of 2023 |



### Annotations
For Creating Annotations, I used SpaCy in python in a jupyter notebook. I created annotations for the Lemmas, Part-Of-Speech and Named Entities.

### File format

The party programs are all txt format and the metadata and text with SpaCy tags are csv files. 
The SpaCy-tagged csv file includes the metadata. Here follow the columns and their descriptions.

### Description of csv file
| metadata | description |
| ------ | ----------- |
| file_name | The filename |
| party_name | The full name of the party in Dutch|
| left_right | Whether the party is left-wing or right-wing |
|current_seats_hop | The amount of seats won in the elections of 2023 in the House of Representatives ('Tweede Kamer' in Dutch ) |
| percent_votes | Percentage of votes the party earned in the elections of 2023 |
| Text | The party program |
| Tokens | The tokenized party program |
| Lemmas | The lemmas in the party program |
| POS | The Part-Of-Speech tags |
| Named_Entities | The entities identified in the party program |
| NE_Words | The words that were identified as entities in the party program |



### Important to mention

This corpus does have some limitations that are important to be aware of when working with it. For one thing, I separated the parties into left-wing and right-wing but one might also use other labels such as ‘centre’, ‘centre-left’ and so on. Another limitation is that the texts are not sampled. Program size varied vastly and sampling would have made the visualisations one can create with this corpus more accurate. The last limitation is that I could not include all party programs that are currently holding seats in the second chamber. However, this was out of an attempt to keep the corpus size limited and to have somewhat of an equal number of left-wing and right-wing parties. 

### Sources
+ Website with party programs : https://www.zokiesje.nl/nieuws/?item=285&nieuws=Overzicht_partijprogrammas
+ Wikipedia about the 2023 elections in the Netherlands : https://nl.wikipedia.org/wiki/Tweede_Kamerverkiezingen_2023

