---
layout: page
title:  "Agency API"
permalink: /agency-api/
---

The API itself is a simple, yet robust API engine.  It has been optimized to be straighforward and fault tolerant.  
  
We provide you with an Amazon S3 bucket (or you can provide your own) and point the API at it.  Then, you upload static data CSV files into the S3 bucket, and they are automatically converted into a queryable, developer-friendly API.  The API is then updated by adding, overwriting, and deleting files.  Each static file generates a 

In the initial setup, you will pick a base URL, such as `https://api.[agency].gov/data/`. When a new file is uploaded into the bucket, an API for that dataset is then generated at `https://api.[agency].gov/data/name-of-file`.  Each static file results in a new API.  

For each API , the file structure dictates the API design. When you upload a CSV dataset, then the column headers will become query parameters for the API.  This direct connection between how the dataset is structured and how the API functions enables us to more easily refine your data publication and improve the developer experience.  

The API includes straightfoward functionality such as querying, pagination, and sorting.  For more details on the API and how to use it, see the [agency manual](https://pages.18f.gov/api-program/agency-manual).
