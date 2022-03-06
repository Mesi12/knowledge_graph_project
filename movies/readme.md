# movies yarrml mapping 
```bash
yarrrml-parser -i imdb.yml -o rules_imdb.rml.ttl
java -jar D:\MSc\Tools\rmlmapper-4.9.2.jar -o output_imdb.ttl -m rules_imdb.rml.ttl -s turtle
```

# movie-character yarrrml mapping
```bash
yarrrml-parser -i movie_character.mapping.yml -o rules_movie_character.rml.ttl
java -jar D:\MSc\Tools\rmlmapper-4.9.2.jar -o output_movie_character.ttl -m rules_movie_character.rml.ttl -s turtle
```

# limes link main characters of movies to character info
```bash
rm -rf .server-storage 
rm limes_accepted_movieChar.nt 
rm limes_reviewme_movieChar.nt 
rm -rf cache

java -jar D:\MSc\Tools\limes.jar limes_movieCharacters.xml
```