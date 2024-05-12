# Description

It is time to get our hands dirty and to manipulate some real world data. You have been hired by a new company named EncyclEarthpedia and your first task it build a search engine. EncyclEarthpedia is an online encyclopedia but specialized in the planet Earth, its geology, biology, and everything related to the Earth.

The search engine should be simple at first. The user needs to be able to type some words and the engine returns the most relevant articles.

There is a problem though. The engineers working on the database messed up and EncyclEarthpedia's database and API are not available for a week. This is a bummer ! If we can't have access to the articles, how are we going to build our engine ?

Instead of waiting for a week, we are going to build a simple model for some similar article from Wikipedia.

What we are going to do is:

Get some article from Wikipedia to work with.
Extract meaningful and usable content from this article.
Clean up and filter the data to narrow the scope to relevant words
Build a simple frequency model.
Analysing the article based on this model.
This first work of this article would be the start of our search engine, using some notion from Information Retrieval and tf-idf statistic.

Getting the data
We are going to work with an article about the Ozone Layer.

# Task

As you may have notice, the answer from the API is not very user-friendly. It is a big json objects with many keys and values that are not really relevant for us. What we really want to work with is the actual 'content' of the article. But what do we mean by "content" ? Are the titles or the table of contents useful? (yes). Are the hidden URL relevant to us?

Only the actual content interests us so we need somehow to remove all the flourish like markups, the urls, and any useless words or characters.

→ First merge and store all the meaningful contents from the big json into a handy variable. Any kind of data structure can be used. A simple list would do the trick though

def merge_contents(data):
	...
merge_content = merge_contents(data)



# Install & Usage

jupyter-notebook -no-browser