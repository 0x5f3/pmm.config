This config will populate the following:

- !Suggested (random, recently added|released, trending, popular, top-rated, most watched)
- !Seasonal *
- Parental
- Documentaries
- Stand-up *
- Awards
- !Year (top-rated)
- !Decades (top-rated)
- !Genre (popular)
- !Genre (top-rated)
- Sub-genre (top-rated) *
- Studio *
- TMDB collections *
- Network ^

( ! = enabled by default)
( * = movies only )
( ^ = shows only )


For more details on what each section contains: [movies](MOVIES.md) | [shows](SHOWS.md)
<br/>
<br/>
<br/>
**Install:**

clone into PMM's root directory:
```
git clone https://github.com/0x5f3/pmm.config config
```

**Usage:**

The initial process for populating collections:
```
python plex_meta_manager.py --config config/movie.yml --collections-only --run --ignore-schedules
python plex_meta_manager.py --config config/show.yml --collections-only --run --ignore-schedules
```
Following a successful initial run:

```
python plex_meta_manager.py --config config/movie.yml --collections-only --run
python plex_meta_manager.py --config config/show.yml --collections-only --run
```
<br/>
A successful run will result in something similar to this:
<br/>
<br/>

![movies](/assets/_/_movies.png)
<br/>
  
![shows](/assets/_/_shows.png)
