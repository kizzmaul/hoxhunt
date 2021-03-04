# Summer Hunters Data Science project
See improvement proposals for things which I would have considered had I not had so little time. 

## Implemented features
- (domain age, was given in the task)
- report count (how many times a domain was reported in the PhishTank database)
- certificate details (if there is one and is it self-signed or issued by someone)
- word frequencies (my hypothesis is that malicious sites often use similar language to convey their intent, meaning that the most common words found on malicious sites could be used as features. specifically, counting the amount of words on some site, which are most certainly present on malicious sites.)

## Visualisation
I chose to do a wordcloud of words found on malicious sites. The size of a word in the image represents its occurence rate in the data. The reason I chose the wordcloud is that it enables the developer to get a glance of the language since that is something which is explicitly directed towards the person viewing the website. 

## Improvement proposals
- I prefer native Python data structures to dataframes but found out that most of my peers prefer dataframes. this needs to be consistent with what the team is using
- easier additions of new extractors into the pipeline. maybe use a function decorator to denote label and automatically save into the database.
- better text parsing: stemming, special character removal, compound word detection, language filtering (meaning only words of some specific language would be considered)
- enhanced descriptions for some functions, with proper type hints
- replacing global index variable with something else
- asynchronous domain scraping
- scraping could be done in different order to avoid multiple identical requests
- reduce the amount of words used as features