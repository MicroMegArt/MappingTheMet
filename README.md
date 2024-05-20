# MappingTheMet

The Metropolitan Museum of Art have made available the CSV spreadsheet of the entire collections on its GitHub repository (https://github.com/metmuseum/openaccess) but these files do not include geographical coordinates. Therefore, it was necessary to geo-reference the objects, which totalled 484,956. 

## The data

The Metropolitan Museum does not provide geographical information in such a uniform manner. The various departments have their own traditions, and their inventories reflect these different ways of looking at objects. The ‘Drawings and Prints’, ‘Photographs’, and ‘Modern and Contemporary Art’ departments enter the artist's nationality in a separate field, ‘Artist Nationality’. When the information is unambiguous, this field is used as the basis for geolocating the works in this study. The ‘European Sculpture and Decorative Arts’ department employs a similar methodology. However, objects that are not attributed to an artist have their geographical origin specified in another field, entitled ‘Culture’. This field, which is filled in for almost all the other Met departments, provides a solid basis for geolocation. It is also completed when the artist is known. 

A notable exception is the department devoted to objects from Africa, Oceania and the Americas (the ‘Michael C. Rockefeller Wing’), which includes a ‘Country’ field in addition to ‘Culture’. For this department, the ‘Country’ field was selected as it is considered to be more suitable for geolocation and hence for mapping.

## Geolocation

A ‘reconciliation’ stage with the Wikidata API was conducted on OpenRefine, in order to place artworks in countries. This enabled the coordinate locations to be extracted from the Wikidata database. The technical steps are outlined in a tutorial available   online (https://github.com/ChristopheCariniSiguret/Cartographie_OpenRefine_Palladio_tutoriel/).

## The final output

This MicroMegArt repository provides the final output files, with the coordinate locations and the Wikidata identifiers. Coordinates have been allocated to 96.95\% of the Met collection. 

The final output for the ‘Michael C. Rockefeller Wing’ was also provided separately. 
