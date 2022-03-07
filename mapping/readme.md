# network rml mapping: builds up the hero-network
```bash
java -jar rmlmapper-4.9.2.jar -m network.rml.ttl -o output_network.ttl -s turtle
```

# imdb yarrml mapping: connects the movies with their properties
```bash
yarrrml-parser -i imdb.yml -o rules_imdb.rml.ttl
java -jar rmlmapper-4.9.2.jar -o output_imdb.ttl -m rules_imdb.rml.ttl -s turtle
```

# movie-character yarrrml mapping: connects the movies with their main characters
```bash
yarrrml-parser -i movie_character.mapping.yml -o rules_movie_character.rml.ttl
java -jar rmlmapper-4.9.2.jar -o output_movie_character.ttl -m rules_movie_character.rml.ttl -s turtle
```

# rdflib mapping files
* "char_stat_rdflib.ipynb": adds properties to the characters
* "marvel_char_rdflib.ipynb": adds a set of different characteristics to the heroes
* "movie_character_rdflib.ipynb": adds labels to the characters to appear on the graph