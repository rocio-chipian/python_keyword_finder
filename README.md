# python_keyword_finder
Returns keywords in a text and their scores using Rake and Stanford NLTK.

Receives a text and the custom stopwords in the body of a POST request to /keywords
Body looks like:
{
    "text": "the text",
    "stopwords": "the, stopwords, separated, by, commas"
}

Returns a json that looks like:
{
    "keywords": [
        {
            "name": "keyword1 name",
            "score": keyword1 score
        },
        {
            "name": "keyword2 name",
            "score"keyword2 score
        }
    ]
}
