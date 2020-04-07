# Django & SearchEngine
This project is search engine which crawling, indexing, analysis and show search result.  contains the crawled data
of 500 pages with seed URL being https://en.wikipedia.org/wiki/Main_Page.
It is a feature used by search engines for query expansion. User marks the relevant and irrelevant documents according to his/her
discretion and then the IR (Information retrieval) system recommends the user an expanded query which might give more relevant result.
Pseudo relevance feedback on the other hand treats the first two documents to be relevant and then suggest a query.

#### skill-set
+ Django
+ Python Package
    + nltk
    + numpy

#### Preview
![Relevance feedback image](https://github.com/ericserraupwork/django-search-engine/blob/master/Screenshots/relevance%20feedback%20(2).png)
![Relevance feedback result image](https://github.com/ericserraupwork/django-search-engine/blob/master/Screenshots/relevance%20feedback%20result.png)

#### Document Clustering
Clustering means grouping similar things together. I have used k - means clustering to group documents together. The documents were
clustered into 50(k=50) clusters after iterating over 25 times. The user is recommended the cluster to which the most relevant result of
the system belongs.
Clusters
![Cluster 1](https://github.com/ericserraupwork/django-search-engine/blob/master/Screenshots/clusters%20(1).png)
![Cluster 2](https://github.com/ericserraupwork/django-search-engine/blob/master/Screenshots/clusters%20(2).png)

#### Page Rank Algorithm
PR (PageRank) value of all the crawled document were calculated using the algebraic method discussed here
https://en.wikipedia.org/wiki/PageRank#Algebraic. The project includes method to sort based on either naïve (based on TFID) or based on
the page rank values of the pages.

#### HITS analysis
The hub and authority score of retrieved pages are calculated by the diagonalization of the product of the adjacency matrix and its
transpose. These are then displayed on the links and can be useful in identifying the hubs and authority.

![hits](https://github.com/ericserraupwork/django-search-engine/blob/master/Screenshots/hits%20analysis.png)

#### Author
+ Eric Serra
+ ericserraupwork@gmail.com
