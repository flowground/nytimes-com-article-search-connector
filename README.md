# ![LOGO](logo.png) Article Search **flow**ground Connector

## Description

A generated **flow**ground connector for the Article Search API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/nytimes.com/article_search/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:19+03:00

## API Description

With the Article Search API, you can search New York Times articles from Sept. 18, 1851 to today, retrieving headlines, abstracts, lead paragraphs, links to associated multimedia and other article metadata.  

 Note: In URI examples and field names, italics indicate placeholders for variables or values. Brackets [ ] indicate optional items. Parentheses ( ) are not a convention — when URIs include parentheses, interpret them literally.

## Authorization

Supported authorization schemes:
- API Key
## Actions

### Article Search

> Article Search requests use the following URI structure:

*Tags:* `Stories`

#### Input Parameters
* `q` - _optional_ - Search query term. Search is performed on the article body, headline and byline.

* `fq` - _optional_ - "Filtered search query using standard Lucene syntax. 

The filter query can be specified with or without a limiting field: label. 

See Filtering Your Search for more information about filtering."

* `begin_date` - _optional_ - "Format: YYYYMMDD 

Restricts responses to results with publication dates of the date specified or later."

* `end_date` - _optional_ - "Format: YYYYMMDD 

Restricts responses to results with publication dates of the date specified or earlier."

* `sort` - _optional_ - "By default, search results are sorted by their relevance to the query term (q). Use the sort parameter to sort by pub_date."

    Possible values: newest, oldest.
* `fl` - _optional_ - "Comma-delimited list of fields (no limit)

  Limits the fields returned in your search results. By default (unless you include an fl list in your request), the following fields are returned: 
  
  web_url
  
  snippet
  
  lead_paragraph
  
  abstract
  
  print_page
  
  blog
  
  source
  
  multimedia
  
  headline
  
  keywords
  
  pub_date
  
  document_type
  
  news_desk
  
  byline
  
  type_of_material
  
  _id
  
  word_count"

* `hl` - _optional_ - Enables highlighting in search results. When set to true, the query term (q) is highlighted in the headline and lead_paragraph fields.

Note: If highlighting is enabled, snippet will be returned even if it is not specified in your fl list."

* `page` - _optional_ - "The value of page corresponds to a set of 10 results (it does not indicate the starting number of the result set). For example, page=0 corresponds to records 0-9. To return records 10-19, set page to 1, not 10."

* `facet_field` - _optional_ - Comma-delimited list of facets

Specifies the sets of facet values to include in the facets array at the end of response, which collects the facet values from all the search results. By default no facet fields will be returned. Below is the list of valid facets:

section_name

document_type

type_of_material

source

day_of_week

To learn more about using facets, see Using Facets.

* `facet_filter` - _optional_ - When set to true, facet counts will respect any applied filters (fq, date range, etc.) in addition to the main query term. To filter facet counts, specifying at least one facet_field is required. To learn more about using facets, see Using Facets.


## License

**flow**ground :- Telekom iPaaS / nytimes-com-article-search-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
