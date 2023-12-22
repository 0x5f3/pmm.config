This config will populate the following:

- !Suggested (random, trending, popular, top-rated, most watched)
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

Initial run to populate collections:
```
python plex_meta_manager.py --config config/movie.yml --collections-only --run --ignore-schedules
python plex_meta_manager.py --config config/show.yml --collections-only --run --ignore-schedules
```
After a successful initial run:

```
python plex_meta_manager.py --config config/movie.yml --collections-only --run
python plex_meta_manager.py --config config/show.yml --collections-only --run
```

**Notes:**

*If you intend to use the Parental collection, enable "item_label.sync: Parental" (line 38, 1_parental.yml) on the initial run and disable for subsequent runs. This prevents ppm from relabelling all of the items with every run, whereas disabling will only label new items added.*

<br/>
After a successful run, you will have something similar to this:
<br/>
<br/>

![movies](/assets/_/movies.png)
<br/>
  
![shows](/assets/_/shows.png)
