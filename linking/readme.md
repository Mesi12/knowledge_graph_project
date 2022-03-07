# Find below the code to execute the different limes files in this folder. They all result in 2 output files. One "accepted" and "review me", based on the threshold of similarity.

# limes link main characters of movies to character info
```bash
rm -rf .server-storage 
rm limes_accepted_movieChar.nt 
rm limes_reviewme_movieChar.nt 
rm -rf cache

java -jar limes.jar limes_movieCharacters.xml
```

# execute limes_characters.xml

```bash

rm -rf .server-storage 
rm limes_accepted_char.nt 
rm limes_reviewme_char.nt 
rm -rf cache

java -jar limes.jar limes_characters.xml

```

# execute limes_network_movie.xml

```bash

rm -rf .server-storage 
rm limes_mov_net_accepted.nt 
rm limes_mov_net_reviewme.nt 
rm -rf cache

java -jar limes.jar limes_network_movie.xml

```