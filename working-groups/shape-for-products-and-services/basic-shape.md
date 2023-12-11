  # Shape for Products and Services


Here is a first draft of a shape.  I have left out types, categories, and keywords. These are all important but are a bit more complex so let's deal with them later.  I am using s: to stand for the schema.org vocabulary and have taken terms from s:Product, s:Service, s:SoftwareApplication. I use d: for the DOAP (Description of a Project) vocabulary.  Not every product or service would use all the terms. Other terms from these and other vocabularies can also be added, this is just the basic set.


**Products and Services**
```
  s:name                 #
  s:description          #
  s:logo                 # 
  s:screenshot           #
  s:audience             # social audience, see below for geographic
  s:areaServed           # geo region, use standard codes
  s:availableLanguage    # human language, use standard codes
  s:isAccessibleForFree  # boolean
  s:license              # an open source license or "proprietary"
  s:provider             # agent who creates service
  s:manufacturer         # agent who creates product
  s:status               # Exploration,Development,Production,Archived
  s:programmingLanguage  # 
  s:operatingSystem      # 
  d:implements           # IRI of a specification
  d:homepage             # 
  d:repository           # 
  d:download-page        # 
  d:bug-database         # 
  d:service-endpoint     # 
```
