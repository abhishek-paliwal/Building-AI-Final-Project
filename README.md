# SEO - Finding possible predictive parameters for top ranking in Google using NLP (Final project for the Building AI course)

## Summary

SEO is very important for any online business and brands these days. For newer articles, high ranking in Google searches is paramount. After searching for a given  keyword, and listing top result URLs on SERP (Search Engine Results Page) as input data, this project aims to deduce the most important ranking factors. 

## Background

Whenever a brand or business publishes a new article for themselves or their clients, a lot of research goes into writing the content. However, more often than not, the article still does not rank high in Google SERPs, and therefore all that effort goes in vain. Ranking high in SERPs can be achieved using the proper analysis of the ranking factors for the top results. Thus, an informative inference can be made which would give significant insights while publishing an article for a chosen keyword. 

With this proper analysis of the current top results, the following problems can be solved. Solving these problems should be paramount for any new startups and also for existing businesses who want to improve their online presence.

**Problems which can be solved with this approach**

* Ignorance about the important of relative ranking factors
* Low visibility and rankings
* Low web traffic
* Low page authority
* Lack of better visitor experience


## How is it used?

Here is the process of using the code provided as a solution. It should be useful for anyone who wants to refine their SEO. This code algorithm  parses the input URLs and finds all the possible top-ranking parameters for each of those URLs. Along with the general python programming code, this program also utilizes some existing NLP python modules. 

### Here are the files in this project:

**Packages Requirements**

* [requirements.txt](requirements.txt)

**Inputs**

* [PROJ01-PYTHON-RAKE-SmartStoplist.txt](PROJ01-PYTHON-RAKE-SmartStoplist.txt)
* [PROJ01-ALL-URLS-FOR-NLP.txt](PROJ01-ALL-URLS-FOR-NLP.txt) (List of top 5-10 top ranking URLs from SERP)
* Eg., Our list of URLs include top search results for this chosen keyword: `mummy pizza toast`

**Output (will be created automatically)**

* [PROJ01_AI_NLP_HTML_OUTPUT.HTML](PROJ01_AI_NLP_HTML_OUTPUT.HTML) (Sample output)

**Runtime Code**

* [PROJ01-using-ai-nlp-to-find-ranking-seo-parameters-from-list-of-top-google-serp-urls.py](PROJ01-using-ai-nlp-to-find-ranking-seo-parameters-from-list-of-top-google-serp-urls.py)

**CLI Run Commands (BASH/ZSH/Linux)**

```
# Install packages
$ pip3 install -r requirements.txt
# Run the program
$ python3 PROJ01-using-ai-nlp-to-find-ranking-seo-parameters-from-list-of-top-google-serp-urls.py
```

### Structure of the output HTML file

The output HTML file thus created after the successful run of the program will have the following extracted details for each of the input URLs.

- ALL_HYPERLINKS_ARRAY
- ALL_IMAGES_ARRAY
- BSOUP_ALL_DATE_TIMES_FROM_WEBPAGE_ARRAY
- BSOUP_NUMWORDS
- BSOUP_READINGTIME_212WPM
- FULL_HEADINGS_ARRAY_FINAL
- META_DESCRIPTION 
- META_GENERATOR 
- NLP_ARTICLE_ANY_VIDEO
- NLP_ARTICLE_AUTHORS
- NLP_ARTICLE_PUBLISH_DATE
- NLP_ARTICLE_SUMMARY
- NLP_ARTICLE_TOP_IMAGE
- NLP_NUMWORDS
- NLP_TOP_KEYWORDS
- RAKE_TOP_KEYWORD_PHRASES
- TITLE_TAG_VALUE 
- TOP20_WORDS_STRING_HTML 

**Final note:** After analyzing all these parameters for every input URL, the user can infer some common ranking factors for his/her own content to be published, and then make changes accordingly into the SEO strategy.


## Data sources and AI methods

The data is freely available as it comes directly from the SERP page. The user then copies the URLs of the top ranking pages in a text file, as input data. The program then parses the URL from the internet and gathers useful insights, and outputs results as a single HTML webpage. The AI methods used for this project makes extensive use of the NLP techniques.

## Challenges

Search Engines such as Google and Bing guard their ranking parameters as secrets. Therefore, having the best of the intentions, sometimes it could still be hard to get any inference from the program results. Also, for some keywords, the challenge could be to parse the content on various URLs which might be using some uncommon platform to generate their website. There, the URLs might not reveal why they appeared at the top, other than the fact that they were indeed referenced by some website which have a high Domain Authority on the internet. However, some insights can still be found which can then be inferred as common patterns. 

## What next?

To make the project code fully automated, efforts can be made such that instead of the user doing the copy-pasting of the URLs, the URLs can directly be gathered from the SERP, and can then be fed as input automatically.

## Acknowledgments

* NA / No copyrighted data is used.