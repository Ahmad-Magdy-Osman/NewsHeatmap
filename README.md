# [HeatedWorld](https://www.heated.world) - [www.heated.world](www.heated.world)
* Fetching news from Reddit; /r/worldnews
  * https://www.reddit.com/dev/api/
    * [PRAW](https://github.com/praw-dev/praw) - [Documentation](https://praw.readthedocs.io/en/latest/)
  * Top 60 articles in the last 24 hours
  * Top 100 articles in the last 7 days
    * Arranged based on a base scored...
* Parse articles text content
  * [Newspaper3k](https://newspaper.readthedocs.io/en/latest/) [GitHub](https://github.com/codelucas/newspaper)
* Extracting geographical info
  * [Mordecai](https://github.com/openeventdata/mordecai)
    * [Mordecai requires Geonames gazetteer running in Elasticsearch, all through Docker](https://github.com/openeventdata/mordecai#installation-and-requirements).
* Creating world heatmap
  * [Datamaps](http://datamaps.github.io/)
  * Heatmap depends on Reddit's post date(on scale of 1-7) + the number of votes; formula = 1-(n/7). Past 24 hours news should create the initial heatmap first based on votes, and from their a ratio can be taken for the amount of heat the older news will get.
* Creating submaps for each country, with headlines and links to articles and reddit discusions
  * Again, this should be a heatmap based on the previously stated logic.
* Potential ideas
  * Tags' maps, not just location maps. Doesn't have to be a heatmap though.
* Digital Ocean
  * Python3 and Docker...
