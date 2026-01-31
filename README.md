# ELK


With KQL, we can search for the logs in two different ways.

Free text search
Field-based search



It didn't return any results because KQL looks for the whole term/word in the documents.

KQL allows the wildcard * to match parts of the word. Let's find out how to use this wild card in the search query.

Search Query: United*

We have used the wildcard with the term United to return all the results containing the term United and any other term after it. If we had logs with the term United Nations. It would also have returned those as a result of this wildcard.


Source_Country : "United States" and UserName : "James OR Albert" WRONG FORMAT   
Source_Country : "United States" and UserName : (James OR Albert) RIGHT FORMAT
