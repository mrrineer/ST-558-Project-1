# ST-558-Project-1

---
title: "XML-Vignette"
authors: Group H
date: 6/6/2019
output:
  html_document:
    toc: yes
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = FALSE, message = FALSE, warning = FALSE, cache = TRUE)
```

# Introduction to XML 

Extensible Markup Language (XML) is a means of storing data on the internet so that it can be retrieved by both humans and machines. XML is similar to other [markup languages](https://en.wikipedia.org/wiki/Markup_language) such as HTML, but offers more flexibility and customization. XML lets the user create and define their tags in order to meet their specific needs. "A key difference between HTML and XML is that HTML defines how data looks, while [XML defines what data is."](https://www.makeuseof.com/tag/xml-file-case-wondering/). XML has many practical [uses](https://www.ibm.com/support/knowledgecenter/en/ssw_ibm_i_71/rzamj/rzamjintrouses.htm):

* Allows for creation of interactive webpages  
* Increases ease of returning useful web search results  
* Use, store, tramsmit, and display data across various devices  
* Increased accessability for data exchange across businesses and customers  
* Expresses metadata in a portable, resuable format  

# R Packages for XML Data

For reading XML data into R the package `xml2()` can be used. The `xml2()` package has several [improvements](https://www.rdocumentation.org/packages/xml2/versions/1.2.0) over the `xml()` package and thus would be more favorable. For instance, `xml2()` automatically frees memory used by an XML document, it doesn't require the user to know the exact type of object they have, and it more conveniently handles namespaces in Xpath expression than `xml()`. 

# XML Data Set

```{r read in data}
install.packages("xml2", repos="http://cran.us.r-project.org")
library(xml2)
library(plyr)


```

