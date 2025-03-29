# Apple Music Text Hints Guidelines

## Introduction
In this document we will explain how to evaluate Music Text Hints for Apple Music. You will use the BaseLine tool to make these judgments. The purpose of this evaluation is to evaluate the relevance of a Text Hint suggestion for a given string, aka prefix. We want to ensure that the Text Hints suggestions add value to the users in their search journey. Use your best judgment when considering the popularity, relevance and recency of a suggestion. Take into account the length of the prefix and how strong the intent is.

## Music Suggestions
Music Suggestions are hints that are provided as a user types their query in the Apple Music search box. The role of the music suggestions is to help the user find the specific content they are looking for quickly and easily. Additionally, suggestions can also provide inspiration for new searches, leading users to discover new and relevant content they might not have otherwise found.

Apple Music provides two types of music suggestions, as illustrated in the screenshot below:
- **Text Hints**: Suggestions that the search engine is offering to the user as they start typing their query. The text hints are not search results, they are queries by themselves.
  - i.e. “the weeknd essentials”, “the weekend”, “the weeknd” in screenshot below.
- **Top Hits**: Search results suggested to the user as they start typing their query.
  - i.e. “The Weeknd” (Artist), “The Weekend” (Song), “The Weeknd Essentials" (Playlist), etc. in screenshot below.

The focus of this evaluation is to evaluate the relevance of the Text Hint.

## The importance of your work as a Rater
The data we receive from you in the form of high quality relevance judgments will be used to build and improve artificial intelligence systems such as search algorithms and machine learned rankers that power the user experience for Apple Music users.
Author: Speed <speedonedirection@gmail.com>
Date:   Sat Mar 29 12:47:50 2025 +0000

    Aggiornato guidelines.md con nuovi esempi di valutazione

[1mdiff --git a/guidelines.md b/guidelines.md[m
[1mindex 3bc20a2..eb95e84 100644[m
[1m--- a/guidelines.md[m
[1m+++ b/guidelines.md[m
[36m@@ -184,4 +184,28 @@[m [mA secondary intent is less likely intent compared to a primary one. A secondary[m
 [m
 #### Query [workout][m
 - **Text Hint:** workout songs => **Acceptable**  [m
[31m-  Questo suggerimento potrebbe sembrare ridondante poiché contiene un linguaggio ovvio nel nostro contesto; tuttavia, potresti incontrare casi in cui un Text Hint contiene un genere, un mood, un’attività + le stringhe "music" o "songs". Poiché questi sono troppo specifici ma comunque utili, la valutazione migliore è **Acceptable**. Inoltre, il simbolo open box alla fine rappresenta uno spazio che l’utente ha inserito dopo il termine di ricerca, implicando che l’intento sia un’entità composta da due o più parole. Non ho visto lo spazio dopo la query. [m
\ No newline at end of file[m
[32m+[m[32m  Questo suggerimento potrebbe sembrare ridondante poiché contiene un linguaggio ovvio nel nostro contesto; tuttavia, potresti incontrare casi in cui un Text Hint contiene un genere, un mood, un’attività + le stringhe "music" o "songs". Poiché questi sono troppo specifici ma comunque utili, la valutazione migliore è **Acceptable**. Inoltre, il simbolo open box alla fine rappresenta uno spazio che l’utente ha inserito dopo il termine di ricerca, implicando che l’intento sia un’entità composta da due o più parole. Non ho visto lo spazio dopo la query.[m[41m [m
[32m+[m[32m  ## Valutazione dei Suggerimenti[m
[32m+[m
[32m+[m[32m### Classificazione dei Suggerimenti[m
[32m+[m
[32m+[m[32m188. **Perfect**: Un suggerimento che molto probabilmente soddisfa un'intenzione primaria comune dell'input. I suggerimenti che completano il prefisso e sono fortemente correlati al prefisso, sono mainstream popolari, aggiungono valore e "hanno senso" data la lunghezza della stringa. Solo le canzoni/albums più popolari e le playlist di alta qualità contenenti solo musica dell'artista dovrebbero essere classificate come Perfect.[m
[32m+[m
[32m+[m[32m189. **Good**: Un suggerimento che probabilmente soddisfa un'intenzione secondaria del prefisso. Un'intenzione secondaria è meno probabile rispetto a un'intenzione primaria. Questo è rilevante per il prefisso e popolare, ma potrebbe non essere la prima scelta dell'utente.[m
[32m+[m
[32m+[m[32m### Esempi di Valutazione[m
[32m+[m
[32m+[m[32m190. **Esempio 1: Query [dua]**[m
[32m+[m[32m- **Suggerimento:** dua lipa madonna[m
[32m+[m[32m- **Classificazione:** Good[m
[32m+[m[32m  - **Motivazione:** Questo suggerimento contiene "dua lipa", che è molto rilevante per la query "dua". Tuttavia, l'aggiunta di "madonna" potrebbe rendere il suggerimento meno diretto. Nonostante ciò, poiché entrambi gli artisti sono molto popolari, il suggerimento può ancora essere considerato utile per l'utente.[m
[32m+[m
[32m+[m[32m191. **Esempio 2: Query [be]**[m
[32m+[m[32m- **Suggerimento:** betty wright[m
[32m+[m[32m- **Classificazione:** Good[m
[32m+[m[32m  - **Motivazione:** Questo suggerimento porta a un'artista con 725K ascoltatori mensili su Spotify e 258K iscritti su YouTube; tuttavia, Wright non ha rilasciato musica da un po' di tempo e il suo periodo di massimo successo è stato negli anni '70. Poiché questo è un artista meno conosciuto/abbastanza popolare (ma non il meno popolare), possono essere considerati come un'intenzione secondaria. Per una query così ampia, solo le entità più popolari possono essere classificate come Perfect.[m
[32m+[m
[32m+[m[32m192. **Esempio 3: Query [kylie m]**[m
[32m+[m[32m- **Suggerimento:** kylie minogue the one[m
[32m+[m[32m- **Classificazione:** Good[m
[32m+[m[32m  - **Motivazione:** Questo suggerimento porta a una canzone dell'artista inteso, ma non è una delle più popolari. Solo le canzoni/albums più popolari e le playlist di alta qualità contenenti solo musica dell'artista dovrebbero essere classificate come Perfect.[m
\ No newline at end of file[m

[33mcommit c95932d1b54f05b41e608f624caee9d2d13265d4[m
Author: Speed <speedonedirection@gmail.com>
Date:   Fri Mar 28 01:14:32 2025 +0000

    Aggiornato guidelines.md con esempio Query [workout]

[1mdiff --git a/guidelines.md b/guidelines.md[m
[1mindex b435b6e..3bc20a2 100644[m
[1m--- a/guidelines.md[m
[1m+++ b/guidelines.md[m
[36m@@ -179,4 +179,9 @@[m [mA secondary intent is less likely intent compared to a primary one. A secondary[m
   - Another example of less popular suggestion is “bad habits remix” for the prefix “bad habi”. The primary intent is likely the song “Bad Habits” by Ed Sheeran and the hints points to the remix of intended song.[m
 - **Less recent**: Hints that points to a less recent content. [m
   - A less recent suggestion might be “good life” for the prefix “good”. The primary intent is likely the song “good 4 u” by Olivia Rodrigo and the hints points to the less recent song “Good Life” by OneRepublic (released in 2009). [m
[31m-- **Slightly Specific**: Hint that points to content relevant to a smaller group of users than for the primary intent or that restricts the intent.[m
\ No newline at end of file[m
[32m+[m[32m- **Slightly Specific**: Hint that points to content relevant to a smaller group of users than for the primary intent or that restricts the intent.[m
[32m+[m[32m### Query: Esempi[m
[32m+[m
[32m+[m[32m#### Query [workout][m
[32m+[m[32m- **Text Hint:** workout songs => **Acceptable**[m[41m  [m
[32m+[m[32m  Questo suggerimento potrebbe sembrare ridondante poiché contiene un linguaggio ovvio nel nostro contesto; tuttavia, potresti incontrare casi in cui un Text Hint contiene un genere, un mood, un’attività + le stringhe "music" o "songs". Poiché questi sono troppo specifici ma comunque utili, la valutazione migliore è **Acceptable**. Inoltre, il simbolo open box alla fine rappresenta uno spazio che l’utente ha inserito dopo il termine di ricerca, implicando che l’intento sia un’entità composta da due o più parole. Non ho visto lo spazio dopo la query.[m[41m [m
\ No newline at end of file[m

[33mcommit 02c6fe3d1552a056dcb942cddb45895b7b0c054f[m
Author: SpeedOned <speedonedirection@gmail.com>
Date:   Thu Mar 27 20:59:31 2025 +0100

    ## Esempi
    
    ## Esempi
    
    ### Query: [mi]
    **Suggerimento:** miley cyrus flowers
    - **Classificazione:** Accettabile
    - **Motivazione:** Sebbene sia pertinente per un possibile intento, non è l'unico risultato rilevante per la query "mi". Pertanto, secondo le linee guida, un suggerimento che soddisfa un intento secondario o meno comune dovrebbe essere classificato come accettabile.
    
    ### Query: [workout]
    **Suggerimento:** workout songs
    - **Classificazione:** Accettabile
    - **Motivazione:** Questo suggerimento potrebbe sembrare ridondante in quanto contiene un linguaggio ovvio nel nostro contesto; tuttavia, potrebbe essere utile in casi dove una Text Hint contiene una combinazione di Genere/Umore/Attività + le stringhe "music" o "songs". Poiché questi sono troppo specifici ma comunque di valore, la classificazione migliore è accettabile. Inoltre, il simbolo di open box alla fine rappresenta uno spazio inserito dall'utente dopo il termine di ricerca, implicando che l'intento dell'utente è una frase di due parole (o più).
    
    ### Esempi addizionali
    
    #### Query: [workout]
    **Suggerimento:** workout music
    - **Classificazione:** Accettabile
    - **Motivazione:** Simile al caso di "workout songs", il suggerimento "workout music" è pertinente ma potrebbe sembrare ridondante. Tuttavia, rimane di valore per gli utenti interessati a musica specifica per l'allenamento.
    
    #### Query: [workout playlist]
    **Suggerimento:** best workout playlist
    - **Classificazione:** Perfetto
    - **Motivazione:** Il suggerimento "best workout playlist" è altamente rilevante e di valore diretto per utenti che cercano playlist specifiche per l'allenamento, aggiungendo valore alla query originale.
    
    ### Note
    - Assicurati di considerare l'intento dell'utente e la specificità della query quando classifichi i suggerimenti.
    - I suggerimenti che sembrano ovvi o ridondanti nel contesto possono comunque essere accettabili se aggiungono valore in modo specifico.

[1mdiff --git a/guidelines.md b/guidelines.md[m
[1mnew file mode 100644[m
[1mindex 0000000..b435b6e[m
[1m--- /dev/null[m
[1m+++ b/guidelines.md[m
[36m@@ -0,0 +1,182 @@[m
[32m+[m[32m# Apple Music Text Hints Guidelines[m
[32m+[m
[32m+[m[32m## Introduction[m
[32m+[m[32mIn this document we will explain how to evaluate Music Text Hints for Apple Music. You will use the BaseLine tool to make these judgments. The purpose of this evaluation is to evaluate the relevance of a Text Hint suggestion for a given string, aka prefix. We want to ensure that the Text Hints suggestions add value to the users in their search journey. Use your best judgment when considering the popularity, relevance and recency of a suggestion. Take into account the length of the prefix and how strong the intent is.[m
[32m+[m
[32m+[m[32m## Music Suggestions[m
[32m+[m[32mMusic Suggestions are hints that are provided as a user types their query in the Apple Music search box. The role of the music suggestions is to help the user find the specific content they are looking for quickly and easily. Additionally, suggestions can also provide inspiration for new searches, leading users to discover new and relevant content they might not have otherwise found.[m
[32m+[m
[32m+[m[32mApple Music provides two types of music suggestions, as illustrated in the screenshot below:[m
[32m+[m[32m- **Text Hints**: Suggestions that the search engine is offering to the user as they start typing their query. The text hints are not search results, they are queries by themselves.[m
[32m+[m[32m  - i.e. “the weeknd essentials”, “the weekend”, “the weeknd” in screenshot below.[m
[32m+[m[32m- **Top Hits**: Search results suggested to the user as they start typing their query.[m
[32m+[m[32m  - i.e. “The Weeknd” (Artist), “The Weekend” (Song), “The Weeknd Essentials" (Playlist), etc. in screenshot below.[m
[32m+[m
[32m+[m[32mThe focus of this evaluation is to evaluate the relevance of the Text Hint.[m
[32m+[m
[32m+[m[32m## The importance of your work as a Rater[m
[32m+[m[32mThe data we receive from you in the form of high quality relevance judgments will be used to build and improve artificial intelligence systems such as search algorithms and machine learned rankers that power the user experience for Apple Music users.[m[41m [m
[32m+[m[32mOur ultimate goal is to surprise and delight our customers by improving search quality and enhancing customer satisfaction, and you play an important role in this.[m
[32m+[m
[32m+[m[32mYour attention to detail, research and language skills as well as your cultural knowledge of the market are all critical to the success of our projects. Please keep in mind that your tasks will be spot-checked for quality, and measured against those of your peers. If your accuracy rate is consistently high enough, you may be qualified to work as an auditor who gives feedback to your peers.[m
[32m+[m
[32m+[m[32m## Rating Overview[m
[32m+[m[32m### Rating Scale[m
[32m+[m[32mThe grades on the relevance scale are as follows:[m
[32m+[m
[32m+[m[32m- Perfect[m
[32m+[m[32m- Good[m
[32m+[m[32m- Acceptable[m
[32m+[m[32m- Unacceptable: Concerns[m
[32m+[m[32m- Unacceptable: Spelling[m
[32m+[m[32m- Unacceptable: Other[m
[32m+[m[32m- Problem: Other[m
[32m+[m
[32m+[m[32m### When choosing your rating take into consideration the following:[m
[32m+[m[32m- Intent of the user[m
[32m+[m[32m- Relevance to the prefix[m
[32m+[m[32m- Popularity/Recency of the music content hinted[m
[32m+[m[32m- Availability on the Apple Music Catalog[m
[32m+[m
[32m+[m[32m#### Intent of the user[m
[32m+[m[32mEach user that navigates to search in Apple Music is looking for a specific piece of content or content in a specific genre/mood. When evaluating the suggestions, keep in mind that user typing the same prefix might have a different intent. Because of this, it is important to understand what is the most frequent and common intent for a specific prefix, also known as primary intent.[m[41m [m
[32m+[m
[32m+[m[32m##### Primary and Secondary Intent[m
[32m+[m[32mThe primary intent of a prefix is the most frequent and common intent based on relevance, recency, and popularity in the market you’re evaluating i.e. the intent of most users who enter that prefix on Apple Music. By taking in account the length of the prefix, you should adjust your popularity/recency judgement according to the set of content which is available given an input.[m
[32m+[m[32mMost of the queries that you will evaluate are incomplete (reason why the inputs is called prefixes). Prefixes can have multiple likely primary intents while others point to a specific content.[m
[32m+[m[32mFor example, for the prefix “lil”, the primary intent could be “Lil Wayne”, “Lil Baby” or “Lil Nas X” (all very popular artists) while for the prefix “pop sm”, the primary intent is clearly the artist “Pop Smoke”.[m
[32m+[m
[32m+[m[32mA secondary intent, on the other hand, is less likely, or is a less popular/common intent compared to a primary one. A secondary intent could be:[m
[32m+[m[32mcontent relevant to a smaller group of users[m
[32m+[m[32mlesser known content such as unpopular covers, remixes from unknown artists.[m
[32m+[m[32mFor example, for the prefix “lil”, a secondary intent could be “Lily Rose”, or “Lily Allen” while for the prefix “pop sm”, a secondary intent could be “Pop Smoke (Instrumental Version) by Lil Cragiu”.[m
[32m+[m
[32m+[m[32m##### Researching Query Intent[m
[32m+[m[32mTo help you understand the likely intents of the prefix, use your local market knowledge in addition to online sources such as Google, YouTube, social media, and other streaming platform. Please, consider how you would search for content as a user of a music streaming platform to navigate to a specific content, or as a means to browse a larger catalogue of music content.[m
[32m+[m
[32m+[m[32m#### Relevance[m
[32m+[m[32mRelevance captures the relationship between the literal text of the prefix and the text hint. The role of the Text Hints is to help the user easily complete their query and make the search faster. Therefore, when assessing the degree of relevance of a suggestion, think about all the different ways that a specific prefix can be completed and how useful each completion can be to the users.[m
[32m+[m
[32m+[m[32mWhen assessing the relevance of the suggestions high emphasis should be given to the user submitted string, aka prefix. For example, for the prefix ‘2000s r’, the Text Hints ‘2000s r&b’ and ‘2000s rock’ are both highly relevant. For the prefix ‘2000s ro’, the previous relevant Text Hint ‘2000s r&b’ is no longer relevant.[m
[32m+[m
[32m+[m[32mNote: Content that does not exist in Apple Music should not be suggested as Text Hint. If a Text Hint points to content that is not available on the platform, it should be rated as Unacceptable: Other.[m
[32m+[m
[32m+[m[32m#### Popularity/Recency[m
[32m+[m[32mIt is important to understand the popularity and recency of the content that the Text Hints point to. Popularity and recency help us understand how many users would likely click on the Text Hints to complete their search. In other words, more popular and/or more recent content is usually relevant to a larger group of users, so the result is more likely to satisfy the intent.[m
[32m+[m
[32m+[m[32mThere are multiple resources you can check to understand popularity of content in your storefront: Bing, Google, Yahoo, YouTube, Genius, Apple Music. Please make sure you use at least two resources before making your decision.[m[41m [m
[32m+[m
[32m+[m[32m##### Seasonal Popularity[m
[32m+[m[32mWhen rating, you could encounter seasonal results which have additional relevance and popularity at specific times of year, for example Christmas songs are very popular at the end of the year. Please consider the seasonal popularity when rating results and consider increasing the rating due to seasonal popularity. E.g. The Text Hint 'christmas jazz' should be rated higher for a prefix [jazz] around Christmas time.[m
[32m+[m
[32m+[m[32m#### Complex Hints[m
[32m+[m[32mYou may encounter hints that are longer and more complex than the standard search hints.[m
[32m+[m
[32m+[m[32mFor these hints, relevance should still be assessed as outlined above. However, it might be more difficult to assess popularity of the exact hint. While the absolute popularity of the intent of the hint be low, it can still lead users to interesting results and invite them to explore. In these situations, please also consider how likely a hint sparks the interest of the user.[m
[32m+[m
[32m+[m[32mSuch complex hints should not be rated Perfect.[m
[32m+[m[32mThe only ratings available for these are Good, Acceptable and Unacceptable. The examples of ratings are below.[m
[32m+[m
[32m+[m[32mGood: Hints that are relevant to the query, popular and would lead users to explore new content.[m
[32m+[m
[32m+[m[32mA complex hint should only be rated Good if the additional words in the text hint add a dimension that will change the results of that music search significantly. This applies especially to artist queries with additional text for decades, genres or remixes.[m[41m [m
[32m+[m[32mFor example, when specifying genre, the query [selena gomez] and the query [selena gomez pop songs] will produce mostly the same results, since the dominant part of the catalog of the artist is all pop music. In contrast, the queries [new order] and [alternative songs by new order] would lead to different results, since the latter actually narrows down the catalog of the band significantly.[m[41m [m
[32m+[m[32mSimilarly with decades, if the artist's work spans over multiple decades and has popular content in multiple, the dominant decade that most people would prefer to search for, would be rated Good. For example, AC/DC has albums from 1970 to 2020. So, specifying the decade [ac/dc songs from 80s] adds relevant dimension and therefore should be considered Good. In contrast, the text hints [the beatles] vs [the beatles albums from 1960s] would lead to very similar results, therefore, that latter hint is only Acceptable.[m[41m [m
[32m+[m
[32m+[m[32m- calm –> calm relaxing music to help me fall asleep (highly relevant to the prefix and would help the user)[m
[32m+[m[32m- art –> artist similar to The Weeknd / artist with a similar sound to The Weeknd (relevant and interesting prefix that would allow user to explore more content)[m
[32m+[m[32m- 70s –> 70s classic rock with shredding guitar solos (relevant to the primary intent and invites exploration to new content)[m
[32m+[m[32m- cardi –> artists similar to cardi b (invites users to explore new content)[m
[32m+[m[32m- cardi –> songs featuring cardi b (intent is clear and this hint invites users to explore content by other artists featuring cardi b)[m
[32m+[m[32m- new ord –> alternative songs by new order (narrows down the catalog of the artist and adds a new dimension)[m
[32m+[m
[32m+[m[32mAcceptable: Hints that are relevant to the query but are less popular or lead to a more specific content.[m
[32m+[m[32mIf the complex hint for an artist includes additional words that do not narrow down the results of search, but the hint is still relevant/popular, this should be rated Acceptable. For example, the query [hip hop songs by moneybagg yo] can be rated Acceptable, since it doesn't add a lot of new information to search, compared to the plain text hint [moneybagg yo].[m
[32m+[m
[32m+[m[32m- 80s –> 80s blockbuster movie songs (relevant and invites exploration, but not very popular for such a broad prefix)[m
[32m+[m[32m- cardi –> new releases by cardi b (relevant to the intent and might be somewhat helpful, but doesn’t include additional details for exploration)[m
[32m+[m[32m- frank –> songs for a 2 hour dinner party featuring frank sinatra and similar artists (relevant to primary intent and interesting way of searching, but might be too specific)[m
[32m+[m[32m- moneyba –> hip hop songs by moneybagg yo (most of the artist's music is in general hip-hop, so this does not narrow down search results for the user)[m
[32m+[m[32m- selena –> selena gomez pop songs (most of the artist's catalog is in pop genre, so adding these extra words do not significantly change the intent of the query or search results)[m
[32m+[m
[32m+[m[32mUnacceptable: Hints that are irrelevant to the prefix and would not be useful to the user or hints pointing to non-existing content.[m
[32m+[m
[32m+[m[32m- adel → adele songs from the 80s (points to non-existing content)[m
[32m+[m[32m- ta → songs that I want to listen to when I take a break (very low relevance between the hint and the prefix)[m
[32m+[m[32m- boys –> find me songs by the beach boys (poorly relevant, not popular and includes unnecessary wording “find me songs”)[m
[32m+[m[32m- 2000s –> play some pop music from the 2000s (relevant and might be popular, but includes unnecessary wording “play some”)[m
[32m+[m[32m- country –> recommend me songs like “take me home, country roads” (relevant and interesting, but includes unnecessary wording “recommend me”)[m
[32m+[m[32m- his –> melody songs by ar rahman. dont forget to include his tamil songs (accidental matching that does not make the hint relevant)[m
[32m+[m[32m- bruno –> songs by bruno mars (relevant to the intent, but doesn’t include any additional value, since the intent of the primary hint is most likely just [bruno mars])[m
[32m+[m[32m- cardi –> songs by cardi b (no additional value since the primary intent is most likely just [cardi b])[m
[32m+[m
[32m+[m[32mUnacceptable: Spelling: A Text Hint that contains spelling errors, spacing errors, punctuation errors, missing accents etc.[m
[32m+[m[32m- kids –> kids songs that teach kids good behvaiour (the word “behaviour” is misspelled)[m
[32m+[m
[32m+[m[32mUnacceptable: Concerns[m
[32m+[m[32mSuggestions containing content related but not limited to the following topics that may be offensive or sensitive:[m
[32m+[m[32m- Bias[m
[32m+[m[32m- Discrimination[m
[32m+[m[32m- Hatred[m
[32m+[m[32m- Restricted or Regulated Content[m
[32m+[m[32m- Sexual Material[m
[32m+[m[32m- Self-Harm[m
[32m+[m[32m- Toxicity[m
[32m+[m[32m- Vulgarity/Obscenities[m
[32m+[m[32m- Violence[m
[32m+[m
[32m+[m[32mProblem: Other[m
[32m+[m[32mUse this rating when a problem or technical issue with the task in BaseLine that makes it impossible to judge relevance. Problem: Other rating should not be used if the content is unavailable in Apple Music but it is still possible to determine relevance between input and output based on the information provided in BaseLine, and by completing a side search on Google and/or on other streaming platforms such as Spotify, Deezer, etc. If a Text Hint points to content that is not available on the platform, it should be rated as Unacceptable: Other.[m
[32m+[m
[32m+[m[32mOpen box ␣[m[41m [m
[32m+[m[32mSome user queries in BaseLine end with the symbol known as open box: ␣[m
[32m+[m[32mThe open box ␣ symbol represents a space that the user entered after their search term(s). For example, if the user entered the word 'che' and then hit the space bar, that specific prefix would be displayed in BaseLine as [che␣]. If the user did not enter a space after, the prefix would be displayed as [che]. It's important to consider the likely and possible user intents with the added space when you see an open box ␣ in the prefix.[m[41m [m
[32m+[m
[32m+[m[32mMandatory Comment[m
[32m+[m[32mEach rating must be explained in the comment box [even if “optional” is indicated - rating comments are always mandatory]. The comment should be concise and must only explain why the rating chosen is the correct one in application of the guidelines.[m
[32m+[m
[32m+[m[32m## Rating Options and Examples[m
[32m+[m[32m### Perfect[m
[32m+[m[32mA suggestion that very likely satisfies a common primary intent of the input, aka prefix.[m
[32m+[m[32mPerfect Text Hints complete the prefix, are strongly related to the prefix, are mainstream popular, add value, and 'make sense' given the length of the string.[m
[32m+[m
[32m+[m[32mKeep in mid that incomplete queries can have more than one possible primary intent. All the hints that complete and/or are strongly related to the prefix and that point to possible primary intents should be rated as Perfect.[m[41m [m
[32m+[m[32mFor example, for the prefix “happ”, possible Text Hints that should be rated as Perfect are “happier than ever”, “happier”, “happy”.[m
[32m+[m
[32m+[m[32m#### Special cases[m
[32m+[m[32m- Queries where the primary intent is for an artist: Only Text Hints pointing to most popular songs or albums by the artist and high quality playlists containing only music by the intended artist (essentials playlists, next steps playlists,..) should be rated as Perfect.[m[41m [m
[32m+[m[32m  - For example, for the prefix "adel", the suggestions "adele 30", "adele essentials" and “adele hello" should be rated as Perfect but the suggestions "adele 19" or "adele daydreamer" should receive a lower rating.[m
[32m+[m[32m- Possible misspellings: When rating, take in consideration that the prefix might be misspelled. In cases where the primary intent of the prefix is clear also if the prefix is misspelled, a suggestion that points to the primary intent content should be rated as Perfect.[m[41m [m
[32m+[m[32m  - For example, for the prefix “beetles”, the suggestion “beatles essentials” should be rated as Perfect.[m
[32m+[m[32m- Lyrics matches: In cases where the suggestion matches the lyrics of a song, use popularity and recency to determine the correct ratings.[m[41m [m
[32m+[m[32m  - An example of a lyrics matching suggestion that should be rated as Perfect is “you want me, i want you, baby” for the prefix “you want m”. In this case, the primary intent is the song “Levitating” by Dua Lipa ft. DaBaby and the suggestion is part of the lyrics of the intended song.[m
[32m+[m[32m- Suggestion identical to the input: You may encounter cases where the hint is identical to the input. The rating for these cases should be Perfect if they point to popular content that likely satisfy a primary intent.[m[41m [m
[32m+[m[32m  - For example, the suggestion “best i ever had” for the prefix “best i ever had”. In this case, the suggestions points to a popular content that very likely satisfies a primary intent.[m
[32m+[m
[32m+[m[32m#### Examples of Perfect Text Hints[m
[32m+[m[32m- bts → bts, bts dynamite, or bts essentials (the band BTS is very likely the primary intent and these results are popular and very likely to satisfy the primary intent)[m
[32m+[m[32m- na → nav, or natanael cano (multiple likely primary intents and these results are popular and very likely to satisfy a primary intent)[m
[32m+[m[32m- t → taylor swift (popular and very likely to satisfy a primary intent)[m
[32m+[m[32m- tay → taylor swift lover (popular and recent album by a very likely primary intent artist)[m
[32m+[m[32m- big → big sean (popular and very likely to satisfy a primary intent)[m
[32m+[m[32m- bey → beyoncé, or beyoncé essentials (popular and very likely to satisfy a primary intent)[m
[32m+[m[32m- pink → p!nk (a very likely primary intent)[m
[32m+[m[32m- billie → billie eilish (a very likely primary intent)[m
[32m+[m[32m- bt → bts (a very likely primary intent)[m
[32m+[m[32m- dra → drake (a very likely primary intent)[m
[32m+[m[32m- yummy → yummy justin bieber (popular and very likely to satisfy a primary intent)[m
[32m+[m[32m- fro → frozen or frozen soundtrack (popular results likely to satisfy the primary intent)[m
[32m+[m[32m- sico → sicko mode (Sicko Mode by Travis Scott is a likely primary intent given that the prefix is very likely misspelled)[m
[32m+[m[32m- shau → shaun frank (a very likely primary intent of this prefix)[m
[32m+[m[32m- 50 cent → 50 cent essentials (high quality playlist that very likely satisfies a primary intent)[m
[32m+[m
[32m+[m[32m### Good[m
[32m+[m[32mA suggestion that likely satisfies a secondary intent of the prefix. Use your best judgment when considering the popularity of a suggestion and evaluating how strong the intent is.[m
[32m+[m
[32m+[m[32mA secondary intent is less likely intent compared to a primary one. A secondary intent hint could be:[m
[32m+[m[32m- **Less popular**: Text Hint that points to lesser known content.[m[41m [m
[32m+[m[32m  - A less popular suggestion might be “hello hello” for the prefix “hello”. The primary intent of the prefix is “Hello” by Adele and this suggestion points to a less popular content “Hello Hello” by Trixie Mattell.[m[41m [m
[32m+[m[32m  - Another example of less popular suggestion is “bad habits remix” for the prefix “bad habi”. The primary intent is likely the song “Bad Habits” by Ed Sheeran and the hints points to the remix of intended song.[m
[32m+[m[32m- **Less recent**: Hints that points to a less recent content.[m[41m [m
[32m+[m[32m  - A less recent suggestion might be “good life” for the prefix “good”. The primary intent is likely the song “good 4 u” by Olivia Rodrigo and the hints points to the less recent song “Good Life” by OneRepublic (released in 2009).[m[41m [m
[32m+[m[32m- **Slightly Specific**: Hint that points to content relevant to a smaller group of users than for the primary intent or that restricts the intent.[m
\ No newline at end of file[m
Our ultimate goal is to surprise and delight our customers by improving search quality and enhancing customer satisfaction, and you play an important role in this.

Your attention to detail, research and language skills as well as your cultural knowledge of the market are all critical to the success of our projects. Please keep in mind that your tasks will be spot-checked for quality, and measured against those of your peers. If your accuracy rate is consistently high enough, you may be qualified to work as an auditor who gives feedback to your peers.

## Rating Overview
### Rating Scale
The grades on the relevance scale are as follows:

- Perfect
- Good
- Acceptable
- Unacceptable: Concerns
- Unacceptable: Spelling
- Unacceptable: Other
- Problem: Other

### When choosing your rating take into consideration the following:
- Intent of the user
- Relevance to the prefix
- Popularity/Recency of the music content hinted
- Availability on the Apple Music Catalog

#### Intent of the user
Each user that navigates to search in Apple Music is looking for a specific piece of content or content in a specific genre/mood. When evaluating the suggestions, keep in mind that user typing the same prefix might have a different intent. Because of this, it is important to understand what is the most frequent and common intent for a specific prefix, also known as primary intent. 

##### Primary and Secondary Intent
The primary intent of a prefix is the most frequent and common intent based on relevance, recency, and popularity in the market you’re evaluating i.e. the intent of most users who enter that prefix on Apple Music. By taking in account the length of the prefix, you should adjust your popularity/recency judgement according to the set of content which is available given an input.
Most of the queries that you will evaluate are incomplete (reason why the inputs is called prefixes). Prefixes can have multiple likely primary intents while others point to a specific content.
For example, for the prefix “lil”, the primary intent could be “Lil Wayne”, “Lil Baby” or “Lil Nas X” (all very popular artists) while for the prefix “pop sm”, the primary intent is clearly the artist “Pop Smoke”.

A secondary intent, on the other hand, is less likely, or is a less popular/common intent compared to a primary one. A secondary intent could be:
content relevant to a smaller group of users
lesser known content such as unpopular covers, remixes from unknown artists.
For example, for the prefix “lil”, a secondary intent could be “Lily Rose”, or “Lily Allen” while for the prefix “pop sm”, a secondary intent could be “Pop Smoke (Instrumental Version) by Lil Cragiu”.

##### Researching Query Intent
To help you understand the likely intents of the prefix, use your local market knowledge in addition to online sources such as Google, YouTube, social media, and other streaming platform. Please, consider how you would search for content as a user of a music streaming platform to navigate to a specific content, or as a means to browse a larger catalogue of music content.

#### Relevance
Relevance captures the relationship between the literal text of the prefix and the text hint. The role of the Text Hints is to help the user easily complete their query and make the search faster. Therefore, when assessing the degree of relevance of a suggestion, think about all the different ways that a specific prefix can be completed and how useful each completion can be to the users.

When assessing the relevance of the suggestions high emphasis should be given to the user submitted string, aka prefix. For example, for the prefix ‘2000s r’, the Text Hints ‘2000s r&b’ and ‘2000s rock’ are both highly relevant. For the prefix ‘2000s ro’, the previous relevant Text Hint ‘2000s r&b’ is no longer relevant.

Note: Content that does not exist in Apple Music should not be suggested as Text Hint. If a Text Hint points to content that is not available on the platform, it should be rated as Unacceptable: Other.

#### Popularity/Recency
It is important to understand the popularity and recency of the content that the Text Hints point to. Popularity and recency help us understand how many users would likely click on the Text Hints to complete their search. In other words, more popular and/or more recent content is usually relevant to a larger group of users, so the result is more likely to satisfy the intent.

There are multiple resources you can check to understand popularity of content in your storefront: Bing, Google, Yahoo, YouTube, Genius, Apple Music. Please make sure you use at least two resources before making your decision. 

##### Seasonal Popularity
When rating, you could encounter seasonal results which have additional relevance and popularity at specific times of year, for example Christmas songs are very popular at the end of the year. Please consider the seasonal popularity when rating results and consider increasing the rating due to seasonal popularity. E.g. The Text Hint 'christmas jazz' should be rated higher for a prefix [jazz] around Christmas time.

#### Complex Hints
You may encounter hints that are longer and more complex than the standard search hints.

For these hints, relevance should still be assessed as outlined above. However, it might be more difficult to assess popularity of the exact hint. While the absolute popularity of the intent of the hint be low, it can still lead users to interesting results and invite them to explore. In these situations, please also consider how likely a hint sparks the interest of the user.

Such complex hints should not be rated Perfect.
The only ratings available for these are Good, Acceptable and Unacceptable. The examples of ratings are below.

Good: Hints that are relevant to the query, popular and would lead users to explore new content.

A complex hint should only be rated Good if the additional words in the text hint add a dimension that will change the results of that music search significantly. This applies especially to artist queries with additional text for decades, genres or remixes. 
For example, when specifying genre, the query [selena gomez] and the query [selena gomez pop songs] will produce mostly the same results, since the dominant part of the catalog of the artist is all pop music. In contrast, the queries [new order] and [alternative songs by new order] would lead to different results, since the latter actually narrows down the catalog of the band significantly. 
Similarly with decades, if the artist's work spans over multiple decades and has popular content in multiple, the dominant decade that most people would prefer to search for, would be rated Good. For example, AC/DC has albums from 1970 to 2020. So, specifying the decade [ac/dc songs from 80s] adds relevant dimension and therefore should be considered Good. In contrast, the text hints [the beatles] vs [the beatles albums from 1960s] would lead to very similar results, therefore, that latter hint is only Acceptable. 

- calm –> calm relaxing music to help me fall asleep (highly relevant to the prefix and would help the user)
- art –> artist similar to The Weeknd / artist with a similar sound to The Weeknd (relevant and interesting prefix that would allow user to explore more content)
- 70s –> 70s classic rock with shredding guitar solos (relevant to the primary intent and invites exploration to new content)
- cardi –> artists similar to cardi b (invites users to explore new content)
- cardi –> songs featuring cardi b (intent is clear and this hint invites users to explore content by other artists featuring cardi b)
- new ord –> alternative songs by new order (narrows down the catalog of the artist and adds a new dimension)

Acceptable: Hints that are relevant to the query but are less popular or lead to a more specific content.
If the complex hint for an artist includes additional words that do not narrow down the results of search, but the hint is still relevant/popular, this should be rated Acceptable. For example, the query [hip hop songs by moneybagg yo] can be rated Acceptable, since it doesn't add a lot of new information to search, compared to the plain text hint [moneybagg yo].

- 80s –> 80s blockbuster movie songs (relevant and invites exploration, but not very popular for such a broad prefix)
- cardi –> new releases by cardi b (relevant to the intent and might be somewhat helpful, but doesn’t include additional details for exploration)
- frank –> songs for a 2 hour dinner party featuring frank sinatra and similar artists (relevant to primary intent and interesting way of searching, but might be too specific)
- moneyba –> hip hop songs by moneybagg yo (most of the artist's music is in general hip-hop, so this does not narrow down search results for the user)
- selena –> selena gomez pop songs (most of the artist's catalog is in pop genre, so adding these extra words do not significantly change the intent of the query or search results)

Unacceptable: Hints that are irrelevant to the prefix and would not be useful to the user or hints pointing to non-existing content.

- adel → adele songs from the 80s (points to non-existing content)
- ta → songs that I want to listen to when I take a break (very low relevance between the hint and the prefix)
- boys –> find me songs by the beach boys (poorly relevant, not popular and includes unnecessary wording “find me songs”)
- 2000s –> play some pop music from the 2000s (relevant and might be popular, but includes unnecessary wording “play some”)
- country –> recommend me songs like “take me home, country roads” (relevant and interesting, but includes unnecessary wording “recommend me”)
- his –> melody songs by ar rahman. dont forget to include his tamil songs (accidental matching that does not make the hint relevant)
- bruno –> songs by bruno mars (relevant to the intent, but doesn’t include any additional value, since the intent of the primary hint is most likely just [bruno mars])
- cardi –> songs by cardi b (no additional value since the primary intent is most likely just [cardi b])

Unacceptable: Spelling: A Text Hint that contains spelling errors, spacing errors, punctuation errors, missing accents etc.
- kids –> kids songs that teach kids good behvaiour (the word “behaviour” is misspelled)

Unacceptable: Concerns
Suggestions containing content related but not limited to the following topics that may be offensive or sensitive:
- Bias
- Discrimination
- Hatred
- Restricted or Regulated Content
- Sexual Material
- Self-Harm
- Toxicity
- Vulgarity/Obscenities
- Violence

Problem: Other
Use this rating when a problem or technical issue with the task in BaseLine that makes it impossible to judge relevance. Problem: Other rating should not be used if the content is unavailable in Apple Music but it is still possible to determine relevance between input and output based on the information provided in BaseLine, and by completing a side search on Google and/or on other streaming platforms such as Spotify, Deezer, etc. If a Text Hint points to content that is not available on the platform, it should be rated as Unacceptable: Other.

Open box ␣ 
Some user queries in BaseLine end with the symbol known as open box: ␣
The open box ␣ symbol represents a space that the user entered after their search term(s). For example, if the user entered the word 'che' and then hit the space bar, that specific prefix would be displayed in BaseLine as [che␣]. If the user did not enter a space after, the prefix would be displayed as [che]. It's important to consider the likely and possible user intents with the added space when you see an open box ␣ in the prefix. 

Mandatory Comment
Each rating must be explained in the comment box [even if “optional” is indicated - rating comments are always mandatory]. The comment should be concise and must only explain why the rating chosen is the correct one in application of the guidelines.

## Rating Options and Examples
### Perfect
A suggestion that very likely satisfies a common primary intent of the input, aka prefix.
Perfect Text Hints complete the prefix, are strongly related to the prefix, are mainstream popular, add value, and 'make sense' given the length of the string.

Keep in mid that incomplete queries can have more than one possible primary intent. All the hints that complete and/or are strongly related to the prefix and that point to possible primary intents should be rated as Perfect. 
For example, for the prefix “happ”, possible Text Hints that should be rated as Perfect are “happier than ever”, “happier”, “happy”.

#### Special cases
- Queries where the primary intent is for an artist: Only Text Hints pointing to most popular songs or albums by the artist and high quality playlists containing only music by the intended artist (essentials playlists, next steps playlists,..) should be rated as Perfect. 
  - For example, for the prefix "adel", the suggestions "adele 30", "adele essentials" and “adele hello" should be rated as Perfect but the suggestions "adele 19" or "adele daydreamer" should receive a lower rating.
- Possible misspellings: When rating, take in consideration that the prefix might be misspelled. In cases where the primary intent of the prefix is clear also if the prefix is misspelled, a suggestion that points to the primary intent content should be rated as Perfect. 
  - For example, for the prefix “beetles”, the suggestion “beatles essentials” should be rated as Perfect.
- Lyrics matches: In cases where the suggestion matches the lyrics of a song, use popularity and recency to determine the correct ratings. 
  - An example of a lyrics matching suggestion that should be rated as Perfect is “you want me, i want you, baby” for the prefix “you want m”. In this case, the primary intent is the song “Levitating” by Dua Lipa ft. DaBaby and the suggestion is part of the lyrics of the intended song.
- Suggestion identical to the input: You may encounter cases where the hint is identical to the input. The rating for these cases should be Perfect if they point to popular content that likely satisfy a primary intent. 
  - For example, the suggestion “best i ever had” for the prefix “best i ever had”. In this case, the suggestions points to a popular content that very likely satisfies a primary intent.

#### Examples of Perfect Text Hints
- bts → bts, bts dynamite, or bts essentials (the band BTS is very likely the primary intent and these results are popular and very likely to satisfy the primary intent)
- na → nav, or natanael cano (multiple likely primary intents and these results are popular and very likely to satisfy a primary intent)
- t → taylor swift (popular and very likely to satisfy a primary intent)
- tay → taylor swift lover (popular and recent album by a very likely primary intent artist)
- big → big sean (popular and very likely to satisfy a primary intent)
- bey → beyoncé, or beyoncé essentials (popular and very likely to satisfy a primary intent)
- pink → p!nk (a very likely primary intent)
- billie → billie eilish (a very likely primary intent)
- bt → bts (a very likely primary intent)
- dra → drake (a very likely primary intent)
- yummy → yummy justin bieber (popular and very likely to satisfy a primary intent)
- fro → frozen or frozen soundtrack (popular results likely to satisfy the primary intent)
- sico → sicko mode (Sicko Mode by Travis Scott is a likely primary intent given that the prefix is very likely misspelled)
- shau → shaun frank (a very likely primary intent of this prefix)
- 50 cent → 50 cent essentials (high quality playlist that very likely satisfies a primary intent)

### Good
A suggestion that likely satisfies a secondary intent of the prefix. Use your best judgment when considering the popularity of a suggestion and evaluating how strong the intent is.

A secondary intent is less likely intent compared to a primary one. A secondary intent hint could be:
- **Less popular**: Text Hint that points to lesser known content. 
  - A less popular suggestion might be “hello hello” for the prefix “hello”. The primary intent of the prefix is “Hello” by Adele and this suggestion points to a less popular content “Hello Hello” by Trixie Mattell. 
  - Another example of less popular suggestion is “bad habits remix” for the prefix “bad habi”. The primary intent is likely the song “Bad Habits” by Ed Sheeran and the hints points to the remix of intended song.
- **Less recent**: Hints that points to a less recent content. 
  - A less recent suggestion might be “good life” for the prefix “good”. The primary intent is likely the song “good 4 u” by Olivia Rodrigo and the hints points to the less recent song “Good Life” by OneRepublic (released in 2009). 
- **Slightly Specific**: Hint that points to content relevant to a smaller group of users than for the primary intent or that restricts the intent.
### Query: Esempi

#### Query [workout]
- **Text Hint:** workout songs => **Acceptable**  
  Questo suggerimento potrebbe sembrare ridondante poiché contiene un linguaggio ovvio nel nostro contesto; tuttavia, potresti incontrare casi in cui un Text Hint contiene un genere, un mood, un’attività + le stringhe "music" o "songs". Poiché questi sono troppo specifici ma comunque utili, la valutazione migliore è **Acceptable**. Inoltre, il simbolo open box alla fine rappresenta uno spazio che l’utente ha inserito dopo il termine di ricerca, implicando che l’intento sia un’entità composta da due o più parole. Non ho visto lo spazio dopo la query. 
  ## Valutazione dei Suggerimenti

### Classificazione dei Suggerimenti

188. **Perfect**: Un suggerimento che molto probabilmente soddisfa un'intenzione primaria comune dell'input. I suggerimenti che completano il prefisso e sono fortemente correlati al prefisso, sono mainstream popolari, aggiungono valore e "hanno senso" data la lunghezza della stringa. Solo le canzoni/albums più popolari e le playlist di alta qualità contenenti solo musica dell'artista dovrebbero essere classificate come Perfect.

189. **Good**: Un suggerimento che probabilmente soddisfa un'intenzione secondaria del prefisso. Un'intenzione secondaria è meno probabile rispetto a un'intenzione primaria. Questo è rilevante per il prefisso e popolare, ma potrebbe non essere la prima scelta dell'utente.

### Esempi di Valutazione

190. **Esempio 1: Query [dua]**
- **Suggerimento:** dua lipa madonna
- **Classificazione:** Good
  - **Motivazione:** Questo suggerimento contiene "dua lipa", che è molto rilevante per la query "dua". Tuttavia, l'aggiunta di "madonna" potrebbe rendere il suggerimento meno diretto. Nonostante ciò, poiché entrambi gli artisti sono molto popolari, il suggerimento può ancora essere considerato utile per l'utente.

191. **Esempio 2: Query [be]**
- **Suggerimento:** betty wright
- **Classificazione:** Good
  - **Motivazione:** Questo suggerimento porta a un'artista con 725K ascoltatori mensili su Spotify e 258K iscritti su YouTube; tuttavia, Wright non ha rilasciato musica da un po' di tempo e il suo periodo di massimo successo è stato negli anni '70. Poiché questo è un artista meno conosciuto/abbastanza popolare (ma non il meno popolare), possono essere considerati come un'intenzione secondaria. Per una query così ampia, solo le entità più popolari possono essere classificate come Perfect.

192. **Esempio 3: Query [kylie m]**
- **Suggerimento:** kylie minogue the one
- **Classificazione:** Good
  - **Motivazione:** Questo suggerimento porta a una canzone dell'artista inteso, ma non è una delle più popolari. Solo le canzoni/albums più popolari e le playlist di alta qualità contenenti solo musica dell'artista dovrebbero essere classificate come Perfect.
  # Apple Music Text Hints Guidelines

## Introduction
In this document we will explain how to evaluate Music Text Hints for Apple Music. You will use the BaseLine tool to make these judgments. The purpose of this evaluation is to evaluate the relevance of the Text Hints.

## Music Suggestions
Music Suggestions are hints that are provided as a user types their query in the Apple Music search box. The role of the music suggestions is to help the user find the specific content they are looking for.

Apple Music provides two types of music suggestions, as illustrated in the screenshot below:
- **Text Hints**: Suggestions that the search engine is offering to the user as they start typing their query. The text hints are not search results, they are queries by themselves.
  - i.e. “the weeknd essentials”, “the weekend”, “the weeknd”.
- **Top Hits**: Search results suggested to the user as they start typing their query.
  - i.e. “The Weeknd” (Artist), “The Weekend” (Song), “The Weeknd Essentials" (Playlist).

The focus of this evaluation is to evaluate the relevance of the Text Hint.

## The importance of your work as a Rater
The data we receive from you in the form of high quality relevance judgments will be used to build and improve artificial intelligence systems such as search algorithms and machine learned rankers. Our ultimate goal is to surprise and delight our customers by improving search quality and enhancing customer satisfaction, and you play an important role in this.

Your attention to detail, research and language skills as well as your cultural knowledge of the market are all critical to the success of our projects. Please keep in mind that your tasks will be evaluated for quality.

## Rating Overview
### Rating Scale
The grades on the relevance scale are as follows:

- Perfect
- Good
- Acceptable
- Unacceptable: Concerns
- Unacceptable: Spelling
- Unacceptable: Other
- Problem: Other

### When choosing your rating take into consideration the following:
- Intent of the user
- Relevance to the prefix
- Popularity/Recency of the music content hinted
- Availability on the Apple Music Catalog

#### Intent of the user
Each user that navigates to search in Apple Music is looking for a specific piece of content or content in a specific genre/mood. When evaluating the suggestions, keep in mind that user typing the query has a specific intent.

##### Primary and Secondary Intent
The primary intent of a prefix is the most frequent and common intent based on relevance, recency, and popularity in the market you’re evaluating i.e. the intent of most users who enter that prefix. Most of the queries that you will evaluate are incomplete (reason why the inputs is called prefixes). Prefixes can have multiple likely primary intents while others point to a specific content. For example, for the prefix “lil”, the primary intent could be “Lil Wayne”, “Lil Baby” or “Lil Nas X” (all very popular artists) while for the prefix “pop sm”, the primary intent could be “Pop Smoke”.

A secondary intent, on the other hand, is less likely, or is a less popular/common intent compared to a primary one. A secondary intent could be:
content relevant to a smaller group of users
lesser known content such as unpopular covers, remixes from unknown artists.
For example, for the prefix “lil”, a secondary intent could be “Lily Rose”, or “Lily Allen” while for the prefix “pop sm”, a secondary intent could be “Pop Smoke (Instrumental Version)”.

##### Researching Query Intent
To help you understand the likely intents of the prefix, use your local market knowledge in addition to online sources such as Google, YouTube, social media, and other streaming platforms.

#### Relevance
Relevance captures the relationship between the literal text of the prefix and the text hint. The role of the Text Hints is to help the user easily complete their query and make the search faster.

When assessing the relevance of the suggestions high emphasis should be given to the user submitted string, aka prefix. For example, for the prefix ‘2000s r’, the Text Hints ‘2000s r&b’ and ‘2000s rock’ are highly relevant.

Note: Content that does not exist in Apple Music should not be suggested as Text Hint. If a Text Hint points to content that is not available on the platform, it should be rated as Unacceptable: Other.

#### Popularity/Recency
It is important to understand the popularity and recency of the content that the Text Hints point to. Popularity and recency help us understand how many users would likely click on the Text Hints.

There are multiple resources you can check to understand popularity of content in your storefront: Bing, Google, Yahoo, YouTube, Genius, Apple Music. Please make sure you use at least two resources.

##### Seasonal Popularity
When rating, you could encounter seasonal results which have additional relevance and popularity at specific times of year, for example Christmas songs are very popular at the end of the year. Please take this into account when evaluating such suggestions.

#### Complex Hints
You may encounter hints that are longer and more complex than the standard search hints.

For these hints, relevance should still be assessed as outlined above. However, it might be more difficult to assess popularity of the exact hint. While the absolute popularity of the intent of the hint may be low, the relative popularity within the context of the hint could be high.

Such complex hints should not be rated Perfect.
The only ratings available for these are Good, Acceptable and Unacceptable. The examples of ratings are below.

Good: Hints that are relevant to the query, popular and would lead users to explore new content.

A complex hint should only be rated Good if the additional words in the text hint add a dimension that will change the results of that music search significantly. This applies especially to artist names, genres, and time periods. For example, when specifying genre, the query [selena gomez] and the query [selena gomez pop songs] will produce mostly the same results, since the dominant part of the catalog of the artist is already pop. Similarly with decades, if the artist's work spans over multiple decades and has popular content in multiple, the dominant decade that most people would prefer to search for, would be rated Good.

- calm –> calm relaxing music to help me fall asleep (highly relevant to the prefix and would help the user)
- art –> artist similar to The Weeknd / artist with a similar sound to The Weeknd (relevant and interesting prefix that would allow user to explore more content)
- 70s –> 70s classic rock with shredding guitar solos (relevant to the primary intent and invites exploration to new content)
- cardi –> artists similar to cardi b (invites users to explore new content)
- cardi –> songs featuring cardi b (intent is clear and this hint invites users to explore content by other artists featuring cardi b)
- new ord –> alternative songs by new order (narrows down the catalog of the artist and adds a new dimension)

Acceptable: Hints that are relevant to the query but are less popular or lead to a more specific content.
If the complex hint for an artist includes additional words that do not narrow down the results of search, but the hint is still relevant/popular, this should be rated Acceptable. For example, the complex hint [selena gomez pop songs] is still relevant, but doesn't narrow down the search results significantly since most of the artist's catalog is in the pop genre.

- 80s –> 80s blockbuster movie songs (relevant and invites exploration, but not very popular for such a broad prefix)
- cardi –> new releases by cardi b (relevant to the intent and might be somewhat helpful, but doesn’t include additional details for exploration)
- frank –> songs for a 2 hour dinner party featuring frank sinatra and similar artists (relevant to primary intent and interesting way of searching, but might be too specific)
- moneyba –> hip hop songs by moneybagg yo (most of the artist's music is in general hip-hop, so this does not narrow down search results for the user)
- selena –> selena gomez pop songs (most of the artist's catalog is in pop genre, so adding these extra words do not significantly change the intent of the query or search results)

Unacceptable: Hints that are irrelevant to the prefix and would not be useful to the user or hints pointing to non-existing content.

- adel → adele songs from the 80s (points to non-existing content)
- ta → songs that I want to listen to when I take a break (very low relevance between the hint and the prefix)
- boys –> find me songs by the beach boys (poorly relevant, not popular and includes unnecessary wording “find me songs”)
- 2000s –> play some pop music from the 2000s (relevant and might be popular, but includes unnecessary wording “play some”)
- country –> recommend me songs like “take me home, country roads” (relevant and interesting, but includes unnecessary wording “recommend me”)
- his –> melody songs by ar rahman. dont forget to include his tamil songs (accidental matching that does not make the hint relevant)
- bruno –> songs by bruno mars (relevant to the intent, but doesn’t include any additional value, since the intent of the primary hint is most likely just [bruno mars])
- cardi –> songs by cardi b (no additional value since the primary intent is most likely just [cardi b])

Unacceptable: Spelling: A Text Hint that contains spelling errors, spacing errors, punctuation errors, missing accents etc.
- kids –> kids songs that teach kids good behvaiour (the word “behaviour” is misspelled)

Unacceptable: Concerns
Suggestions containing content related but not limited to the following topics that may be offensive or sensitive:
- Bias
- Discrimination
- Hatred
- Restricted or Regulated Content
- Sexual Material
- Self-Harm
- Toxicity
- Vulgarity/Obscenities
- Violence

Problem: Other
Use this rating when a problem or technical issue with the task in BaseLine that makes it impossible to judge relevance. Problem: Other rating should not be used if the content is unavailable in Apple Music.

Open box ␣ 
Some user queries in BaseLine end with the symbol known as open box: ␣
The open box ␣ symbol represents a space that the user entered after their search term(s). For example, if the user entered the word 'che' and then hit the space bar, that specific prefix would end with ‘che␣’.

Mandatory Comment
Each rating must be explained in the comment box [even if “optional” is indicated - rating comments are always mandatory]. The comment should be concise and must only explain why the rating choice was made.

## Rating Options and Examples
### Perfect
A suggestion that very likely satisfies a common primary intent of the input, aka prefix.
Perfect Text Hints complete the prefix, are strongly related to the prefix, are mainstream popular, add value, and 'make sense' given the length of the string.

Keep in mind that incomplete queries can have more than one possible primary intent. All the hints that complete and/or are strongly related to the prefix and that point to possible primary intents should be rated as Perfect. For example, for the prefix “happ”, possible Text Hints that should be rated as Perfect are “happier than ever”, “happier”, “happy”.

#### Special cases
- Queries where the primary intent is for an artist: Only Text Hints pointing to most popular songs or albums by the artist and high quality playlists containing only music by the intended artist should be rated as Perfect. 
  - For example, for the prefix "adel", the suggestions "adele 30", "adele essentials" and “adele hello" should be rated as Perfect but the suggestions "adele 19" or "adele daydreamer" should not.
- Possible misspellings: When rating, take in consideration that the prefix might be misspelled. In cases where the primary intent of the prefix is clear also if the prefix is misspelled, a suggestion pointing to the correct content should be rated as Perfect.
  - For example, for the prefix “beetles”, the suggestion “beatles essentials” should be rated as Perfect.
- Lyrics matches: In cases where the suggestion matches the lyrics of a song, use popularity and recency to determine the correct ratings. 
  - An example of a lyrics matching suggestion that should be rated as Perfect is “you want me, i want you, baby” for the prefix “you want m”. In this case, the primary intent is the song “Levitating” by Dua Lipa.
- Suggestion identical to the input: You may encounter cases where the hint is identical to the input. The rating for these cases should be Perfect if they point to popular content that likely satisfies a primary intent.
  - For example, the suggestion “best i ever had” for the prefix “best i ever had”. In this case, the suggestions points to a popular content that very likely satisfies a primary intent.

#### Examples of Perfect Text Hints
- bts → bts, bts dynamite, or bts essentials (the band BTS is very likely the primary intent and these results are popular and very likely to satisfy the primary intent)
- na → nav, or natanael cano (multiple likely primary intents and these results are popular and very likely to satisfy a primary intent)
- t → taylor swift (popular and very likely to satisfy a primary intent)
- tay → taylor swift lover (popular and recent album by a very likely primary intent artist)
- big → big sean (popular and very likely to satisfy a primary intent)
- bey → beyoncé, or beyoncé essentials (popular and very likely to satisfy a primary intent)
- pink → p!nk (a very likely primary intent)
- billie → billie eilish (a very likely primary intent)
- bt → bts (a very likely primary intent)
- dra → drake (a very likely primary intent)
- yummy → yummy justin bieber (popular and very likely to satisfy a primary intent)
- fro → frozen or frozen soundtrack (popular results likely to satisfy the primary intent)
- sico → sicko mode (Sicko Mode by Travis Scott is a likely primary intent given that the prefix is very likely misspelled)
- shau → shaun frank (a very likely primary intent of this prefix)
- 50 cent → 50 cent essentials (high quality playlist that very likely satisfies a primary intent)

### Good
A suggestion that likely satisfies a secondary intent of the prefix. Use your best judgment when considering the popularity of a suggestion and evaluating how strong the intent is.

A secondary intent is less likely intent compared to a primary one. A secondary intent hint could be:
- **Less popular**: Text Hint that points to lesser known content. 
  - A less popular suggestion might be “hello hello” for the prefix “hello”. The primary intent of the prefix is “Hello” by Adele and this suggestion points to a less popular content.
  - Another example of less popular suggestion is “bad habits remix” for the prefix “bad habi”. The primary intent is likely the song “Bad Habits” by Ed Sheeran and the hints points to a less popular remix.
- **Less recent**: Hints that points to a less recent content. 
  - A less recent suggestion might be “good life” for the prefix “good”. The primary intent is likely the song “good 4 u” by Olivia Rodrigo and the hints points to the less recent song “Good Life” by Kanye West.
- **Slightly Specific**: Hint that points to content relevant to a smaller group of users than for the primary intent or that restricts the intent.

### Query: Esempi

#### Query [workout]
- **Text Hint:** workout songs => **Acceptable**  
  Questo suggerimento potrebbe sembrare ridondante poiché contiene un linguaggio ovvio nel nostro contesto; tuttavia, potresti incontrare casi in cui un Text Hint contiene un genere, un mood, un artista specifico che potrebbe essere utile per l'utente.

## Valutazione dei Suggerimenti

### Classificazione dei Suggerimenti

188. **Perfect**: Un suggerimento che molto probabilmente soddisfa un'intenzione primaria comune dell'input. I suggerimenti che completano il prefisso e sono fortemente correlati al prefisso, sono mainstream popolari, aggiungono valore e 'hanno senso' data la lunghezza della stringa.

189. **Good**: Un suggerimento che probabilmente soddisfa un'intenzione secondaria del prefisso. Un'intenzione secondaria è meno probabile rispetto a un'intenzione primaria. Questo è rilevante nel contesto della popolarità e della rilevanza del contenuto suggerito.

### Esempi di Valutazione

190. **Esempio 1: Query [dua]**
- **Suggerimento:** dua lipa madonna
- **Classificazione:** Good
  - **Motivazione:** Questo suggerimento contiene "dua lipa", che è molto rilevante per la query "dua". Tuttavia, l'aggiunta di "madonna" potrebbe rendere il suggerimento meno diretto. Nonostante ciò, è ancora rilevante e probabile che soddisfi un'intenzione secondaria.

191. **Esempio 2: Query [be]**
- **Suggerimento:** betty wright
- **Classificazione:** Good
  - **Motivazione:** Questo suggerimento porta a un'artista con 725K ascoltatori mensili su Spotify e 258K iscritti su YouTube; tuttavia, Wright non ha rilasciato musica da un po' di tempo e il suggerimento potrebbe non essere altamente popolare.

192. **Esempio 3: Query [kylie m]**
- **Suggerimento:** kylie minogue the one
- **Classificazione:** Good
  - **Motivazione:** Questo suggerimento porta a una canzone dell'artista inteso, ma non è una delle più popolari. Solo le canzoni/albums più popolari e le playlist di alta qualità contenenti la musica dell'artista dovrebbero essere considerate Perfect.

### Esempio di Valutazione con Errore Ortografico

#### Query [freez]
- **Suggerimento:** freeze t pain
- **Classificazione:** Unacceptable: Spelling
  - **Motivazione:** Nonostante quanto possa sembrare rilevante questo suggerimento, il nome "t pain" è scritto in modo errato; pertanto, è un suggerimento inaccettabile. Correzione ortografica: "t-pain" (con un trattino in mezzo).

### Esempi di Valutazione Aggiuntivi

#### Query: [mi]
- **Suggerimento:** miley cyrus flowers
- **Classificazione:** Accettabile
  - **Motivazione:** Sebbene sia pertinente per un possibile intento, non è l'unico risultato rilevante per la query "mi". Pertanto, secondo le linee guida, un sugger
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>To-Do List</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="todo-container">
        <h1>To-Do List</h1>
        <input type="text" id="todo-input" placeholder="Add a new task">
        <button id="add-todo">Add</button>
        <ul id="todo-list"></ul>
    </div>
    <script src="scripts.js"></script>
</body>
</html>
[33mcommit 0be8d6c2f38fc982068a92612e83fcd437afecf3[m[33m ([m[1;36mHEAD[m[33m -> [m[1;32mmain[m[33m, [m[1;31morigin/main[m[33m, [m[1;31morigin/HEAD[m[33m)[m
Author: Speed <speedonedirection@gmail.com>
Date:   Sat Mar 29 12:47:50 2025 +0000

    Aggiornato guidelines.md con nuovi esempi di valutazione

[33mcommit c95932d1b54f05b41e608f624caee9d2d13265d4[m
Author: Speed <speedonedirection@gmail.com>
Date:   Fri Mar 28 01:14:32 2025 +0000

    Aggiornato guidelines.md con esempio Query [workout]

[33mcommit e80f22b0ed3c4a5c06532efaa8ad0856ff0fe9c9[m
Author: SpeedOned <speedonedirection@gmail.com>
Date:   Thu Mar 27 22:46:14 2025 +0100

    Create main.yml

[33mcommit d3f97bb8af22b4b81c8baea64032007bc52e14f1[m
Author: SpeedOned <speedonedirection@gmail.com>
Date:   Thu Mar 27 22:41:44 2025 +0100

    Add files via upload

[33mcommit 02c6fe3d1552a056dcb942cddb45895b7b0c054f[m
Author: SpeedOned <speedonedirection@gmail.com>
Date:   Thu Mar 27 20:59:31 2025 +0100

    ## Esempi
    
    ## Esempi
    
    ### Query: [mi]
    **Suggerimento:** miley cyrus flowers
    - **Classificazione:** Accettabile
    - **Motivazione:** Sebbene sia pertinente per un possibile intento, non è l'unico risultato rilevante per la query "mi". Pertanto, secondo le linee guida, un suggerimento che soddisfa un intento secondario o meno comune dovrebbe essere classificato come accettabile.
    
    ### Query: [workout]
    **Suggerimento:** workout songs
    - **Classificazione:** Accettabile
    - **Motivazione:** Questo suggerimento potrebbe sembrare ridondante in quanto contiene un linguaggio ovvio nel nostro contesto; tuttavia, potrebbe essere utile in casi dove una Text Hint contiene una combinazione di Genere/Umore/Attività + le stringhe "music" o "songs". Poiché questi sono troppo specifici ma comunque di valore, la classificazione migliore è accettabile. Inoltre, il simbolo di open box alla fine rappresenta uno spazio inserito dall'utente dopo il termine di ricerca, implicando che l'intento dell'utente è una frase di due parole (o più).
    
    ### Esempi addizionali
    
    #### Query: [workout]
    **Suggerimento:** workout music
    - **Classificazione:** Accettabile
    - **Motivazione:** Simile al caso di "workout songs", il suggerimento "workout music" è pertinente ma potrebbe sembrare ridondante. Tuttavia, rimane di valore per gli utenti interessati a musica specifica per l'allenamento.
    
    #### Query: [workout playlist]
    **Suggerimento:** best workout playlist
    - **Classificazione:** Perfetto
    - **Motivazione:** Il suggerimento "best workout playlist" è altamente rilevante e di valore diretto per utenti che cercano playlist specifiche per l'allenamento, aggiungendo valore alla query originale.
    
    ### Note
    - Assicurati di considerare l'intento dell'utente e la specificità della query quando classifichi i suggerimenti.
    - I suggerimenti che sembrano ovvi o ridondanti nel contesto possono comunque essere accettabili se aggiungono valore in modo specifico.
# Ratings for a Narrow Prefix: [rosalia]

## Perfect
### Suggestion (Hint): rosalia despecha
- **Classificazione:** Perfect
- **Motivazione:** Points to a very popular song by the intended artist.

## Good
### Suggestion: rosalia los angeles
- **Classificazione:** Good
- **Motivazione:** Points to a lesser-known/not too popular song album by the intended artist.

### Suggestion: rosalia tokischa
- **Classificazione:** Good
- **Motivazione:** Points to a popular collab by the intended artist but is slightly specific for the search prefix, as it doesn't mention the song's name. A Perfect suggestion would be "rosalia linda" which is the song featuring Tokischa.

## Acceptable
### Suggestion: rosalia la fam
- **Classificazione:** Acceptable
- **Motivazione:** Points to a popular song by the intended artist BUT is incomplete. Should be "rosalia la fama".

## Unacceptable: Other
### Suggestion: rosalia despecha-single
- **Classificazione:** Unacceptable: Other
- **Motivazione:** Despite how popular the content the suggestion points to might seem, the word 'single' is redundant (a single album contains only one song) and therefore unacceptable.

## Unacceptable: Spelling
### Suggestion: rosalia despecha
- **Classificazione:** Unacceptable: Spelling
- **Motivazione:** Despite how popular the content the suggestion points to might seem, both tokens are misspelt as they're missing accents: "rosalía despechá".
# Ratings for a Narrow Prefix: [rosalia]

## Perfect
### Suggestion (Hint): rosalia despecha
- **Classificazione:** Perfect
- **Motivazione:** Points to a very popular song by the intended artist.

## Good
### Suggestion: rosalia los angeles
- **Classificazione:** Good
- **Motivazione:** Points to a lesser-known/not too popular song album by the intended artist.

### Suggestion: rosalia tokischa
- **Classificazione:** Good
- **Motivazione:** Points to a popular collab by the intended artist but is slightly specific for the search prefix, as it doesn't mention the song's name. A Perfect suggestion would be "rosalia linda" which is the song featuring Tokischa.

## Acceptable
### Suggestion: rosalia la fam
- **Classificazione:** Acceptable
- **Motivazione:** Points to a popular song by the intended artist BUT is incomplete. Should be "rosalia la fama".

## Unacceptable: Other
### Suggestion: rosalia despecha-single
- **Classificazione:** Unacceptable: Other
- **Motivazione:** Despite how popular the content the suggestion points to might seem, the word 'single' is redundant (a single album contains only one song) and therefore unacceptable.

## Unacceptable: Spelling
### Suggestion: rosalia despecha
- **Classificazione:** Unacceptable: Spelling
- **Motivazione:** Despite how popular the content the suggestion points to might seem, both tokens are misspelt as they're missing accents: "rosalía despechá"
### Esempi di Valutazione Aggiuntivi

#### Query: [cora]
- **Suggerimento:** corazon despeinado
- **Classificazione:** Unacceptable: Spelling
  - **Motivazione:** Nonostante quanto possa sembrare rilevante questo suggerimento, la parola "corazon" è scritta in modo errato; pertanto, è un suggerimento inaccettabile. Correzione ortografica necessaria: "corazón" (con un accento).
