# JAFF project | Master’s Thesis | 

## MA Digital Humanities | University of Groningen 
## Letizia Maria Marietti | S6052029 

### Project title: 
Mapping Present-Day Commercially Published Jane Austen Inspired Works: Exploring the Role of Author Multiculturalism in Publishing Practices and Reader Perception 
Research aims: This research’s primary aim lies in systematically mapping and investigating the landscape of commercially published Jane Austen derivative works (known by the acronym JAFF, Jane Austen Fan Fiction), a phenomenon that has received little quantitative attention in literary and fan studies. Leveraging three original datasets compiled from Goodreads and Amazon, including bibliographic, editorial, and reception metadata, the project documents and visualizes the diversity of the phenomenon, covering more than 8.000 titles and over 20.000 editions. Special focus is placed on how the multilingual and multicultural backgrounds of authors influence their opportunities with major publishing houses, the dissemination of their works (in terms of editions and translations), and their reception by readers (as measured by ratings and reviews). By adopting a descriptive and comparative methodology, this study aims to provide both a foundational resource and new insights for understanding diversity and inclusion in the contemporary publishing ecosystem. 

### Description of the corpus: 
The corpus comprises all commercially published works, with relative editions and translations, of Austenesque fiction by contemporary authors individuated on Goodreads up to December 2024, without any restriction of genre or language in order to obtain the widest possible sample. It is organized across three different datasets providing information at different levels: the Authors and Works datasets cover around 8.000 unique titles, with metadata providing information, respectively, on authors backgrounds and the works themselves. 

### Data collection process: 
The core data was scraped from Goodreads book and author profiles (including titles, genres, average ratings, publication years, and publisher information), with Amazon author pages, when existent, to compensate missing biographical data crucial for assessing multilingual and multicultural backgrounds.

### Ethical considerations: 
Author data was collected from publicly accessible Goodreads profiles, including self-reported biographies and basic metadata (e.g., names, birthplaces). Data collection complied with the Exception for Text and Data Mining (TDM) under Article 3 of Directive (EU) 2019/790 of April 2019, and personal data was processed solely for academic research purposes in accordance with the GDPR (articles 5 and 89). In some cases, additional author attributes such as gender, ethnicity, multilingualism, and cultural background were inferred based on publicly available biographical information. These inferences were made solely for enabling the identification of large-scale patterns relevant to the researched phenomenon. 

### Structure of the repository:
The repository contains separate folders for all key research components:
/codes: Python scripts for scraping (Goodreads/Amazon) and analysis.
/datasets: The three main datasets in CSV format (Authors_dataset.csv, Works_dataset.csv, Editions_dataset.csv).

### Datasets description: 
List of variables included in each dataset and their description. For a detailed definition, see paragraph 3.1.4 in the main text. 

- Authors_dataset.csv (8381 entries) comprises:

| Variable             | Description                                                                                                                                  |
|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
|Author ID             | Unique author identifier assigned by Goodreads                                                                                               |
|Author name           | The author of the book (either real names or pseudonyms)                                                                                     |
|Place of birth        | Author’s birthplace as available in the Goodreads biography of each author                                                                   |
|Biography             | Short information of author’s life or career, as available in the Goodreads biography section                                                |
|Genres                | Literary genre of the work, e.g. Mystery, Fiction, Historical, etc.                                                                          |
|URL authors           | The Goodreads webpage of each author, with information on their biography and their personal website (if available), and their body of work  |
|Title                 | The title of the book in its original language                                                                                               |
|URL books             | The direct web address (URL) to the specific page of each book on Goodreads                                                                  |
|Average Rating        | Average of ratings for each book on Goodreads as of May 2025                                                                                 |
|Year of publication   | The year in which each title was first published                                                                                             |
|Number of works       | The quantity of literary works published by each author (total of works, not necessarily Austen transformative work)                         |
|Multilingual          | Whether or not the author can be associated with this definition, according to the Goodreads biography of the latter                         |
|Monolingual           | Authors who have a Goodreads description and do not explicitly declare knowledge of more than one language or a multicultural background     |
|Man/woman             | Gender of the author as inferred from the Goodreads profiles                                                                                 |
|American/British/Other| An author living or born in the United States of America or the United Kingdom if explicitly mentioned in the Goodreads or Amazon profile.   | 
                       |  All other cases, including authors from different countries or profiles without this information, are grouped under “Other”                 |

- Works_dataset.csv (7.491 entries) includes: 

| Variable             | Description                                                                                                                                       |
|----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|
|Title                 | The title of the book in its original language                                                                                                    |
|Author ID             | Same as in Authors dataset                                                                                                                        |
|Author                | The author of the book                                                                                                                            |
|Average Rating        | Average of ratings for each book on Goodreads as of May 2025                                                                                      |
|Ratings Count         | Total number of ratings for each book on Goodreads as of May 2025                                                                                 |
|Reviews Count         | Total number of reviews for each book on Goodreads as of May 2025                                                                                 |
|Description           | Short overview of the book’s content                                                                                                              |
|Genres                | Literary genre of the work, e.g. Mystery, Fiction, etc.                                                                                           |
|Pages Format          | Number of pages of the book and format of the published book                                                                                      |
|Publication Info      | The date of publication of each title, in some cases with some additional information such as date of first publication or of expected publication|
|Ratings Histogram     | Numerical representation of a graphical representation (in form of a bar chart) of the ratings distribution for each book                         |

- Editions_dataset.csv (21989 entries): 

| Variable             | Description                                                                                                                                      |
|----------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
|Title                 | The title of the book in its original language (either original publication, reedition, or translation)                                          |
|Publication Date      | The date of publication of each title                                                                                                            |         
|Publisher             | Complete name of the edition’s publisher. The differentiation is made between ‘Big publishers’, ‘Small publishers’, and ‘Independently published’| 
|Format                | Format of the published book (hardcover, paperback, eBooks, Kindle)                                                                              |
|Page Count            | Number of pages of the book                                                                                                                      |
|Author                | The author of the book                                                                                                                           |
|Author ID             | Same as in previous datasets                                                                                                                     |
|ISBN                  | International Standard Book Number assigned by the publisher to each book edition                                                                |
|ASIN                  | Amazon Standard Identification Number assigned to each book edition                                                                              |
|Edition Language      | The language the specific book edition is written in                                                                                             |
|Average Rating        | Average number of ratings for each book on Goodreads as of May 2025                                                                              |
|Rating Count          | Total number of ratings for each book on Goodreads as of May 2025                                                                                |
|Book URL              | The direct web address (URL) to the specific edition page of each book on Goodreads                                                              |
|Publisher type        | Either ‘big publisher’, ‘small publisher’, ‘self-published’, or ‘unknown’                                                                        |

Contact: 
For questions about this thesis or related projects, please write to l.m.marietti@student.rug.nl

