[GitHub](https://github.com/lllisteu/lllisteu-data)

# lllist.eu data

This repository contains data for art exhibitions and art museums in Europe. It is updated irregularly.

The [lllist.eu](https://lllist.eu/) website lists art exhibitions in Europe and is generated from exhibition data in this repository.

## History of lllist.eu

lllist.eu became active in February 2012 and was updated frequently until March 2018. Since then, the website and this repository are updated irregularly.

![lllist.eu viewed on an iphone 6](lllist_iphone.png)

The site shows current exhibitions (sorted by closing date), and future exhibitions (sorted by opening date).

lllist is a [single-serving site](https://en.wikipedia.org/wiki/Single-serving_site) inspired by Paul Hammond's [Minimuni](https://minimuni.paulhammond.org/). It is served as a static web page, generated from data stored in simple text files: one file for each exhibition.

## Data

Data is stored in simple text files. Each file holds data for one exhibition (or museum), formatted as YAML frontmatter. Files are encoded in UTF-8 and have a .txt extension.

### Exhibition data

This is an example of a file for an exhibition:

```yaml
---
title: Abraham Cruzvillegas
uid: '20171106103952'
dt-created: 2017-11-06 10:39:52 GMT
event-dt-begin: '2018-02-16'
event-dt-end: '2018-03-25'
event-location: 'Kunsthaus Zürich'
link: http://www.kunsthaus.ch/en/exhibitions/coming-soon/abraham-cruzvillegas/
---
```

Field names are mostly self explanatory:

Field|Description|Wikidata equivalent
---|---|---
title|exhibition title| |
uid|unique identifier| |
dt-created|record creation date/time| |
event-dt-begin|opening date of the exhibition|[P1619](https://www.wikidata.org/wiki/Property:P1619)
event-dt-end|closing date of the exhibition|[P3999](https://www.wikidata.org/wiki/Property:P3999)
event-location|exhibition venue (museum)|[P276](https://www.wikidata.org/wiki/Property:P276)
link|URL of exhibition webpage| |

### Museum data

The set of museum data is still growing. Apart from museums, it includes some exhibition venues without a collection (_Kunsthalle_).

Field names are mostly self explanatory:

Field|Description|Wikidata equivalent
---|---|---
title|museum name| |
uid|unique identifier| |
dt-created|record creation date/time| |
link|URL of museum webpage|[P856](https://www.wikidata.org/wiki/Property:P856)
tags|tags| |
wikidata_id|corresponding [Wikidata](https://www.wikidata.org/) item| |
wikipedia|corresponding [Wikipedia](https://en.wikipedia.org/) article| |
lat|[latitude](https://en.wikipedia.org/wiki/Geographic_coordinate_system)|[P625](https://www.wikidata.org/wiki/Property:P625)
lon|[longitude](https://en.wikipedia.org/wiki/Geographic_coordinate_system)|[P625](https://www.wikidata.org/wiki/Property:P625)
isa|object class (usually _museum_)| |

## Resources

* Related projects
    * Museum of Modern Art [collection](https://github.com/MuseumofModernArt/collection) and [exhibition](https://github.com/MuseumofModernArt/exhibitions) data
    * [The Tate Collection](https://github.com/tategallery/collection)
* [Europeana Collections](https://www.europeana.eu/)
* [_Unsustainable Museum Data_](https://matthewlincoln.net/2015/01/26/unsustainable-museum-data.html) by Matthew Lincoln

## License

Data is provided “as is”, without warranties of any kind.

This dataset is placed in the public domain using a [CC0 License](https://creativecommons.org/publicdomain/zero/1.0/).
