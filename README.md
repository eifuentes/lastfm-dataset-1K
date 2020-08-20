# Last.FM 1K User Dataset

This repository hosts the [Last.fm Dataset - 1K users](http://ocelma.net/MusicRecommendationDataset/lastfm-1K.html) under the same license and terms in the offical README, copied for convenience below.

The dataset has been preprocessed and hosted for easier use in the standard PyData set of tools. In addition, an educational/developer friendly subset is hosted for quality assurance tasks and experimentation. See the releases section of this repository to download.

## README
*Version 1.0, May 2010*

### What is this?

This dataset contains *user*, *timestamp*, *artist*, *song* tuples collected from <a href="http://www.last.fm/api">Last.fm API</a>, 
using the <a href="http://www.last.fm/api/show?service=278">user.getRecentTracks()</a> method.

This dataset represents the whole listening habits (till May, 5th 2009) for nearly **1,000** users.

### Files

| Filename | MD5 |
| - | - |
| userid-timestamp-artid-artname-traid-traname.tsv | 64747b21563e3d2aa95751e0ddc46b68 |
| userid-profile.tsv | c53608b6b445db201098c1489ea497df |

### Data Statistics

#### userid-timestamp-artid-artname-traid-traname.tsv

| Element | Statistic |
| - | - |
| Total Lines | 19,150,868
| Unique Users | 992
| Artists with MBID | 107,528
| Artists without MBDID | 69,420

### Data Format

The data is formatted one entry per line as follows (tab separated, `\t`)

#### userid-timestamp-artid-artname-traid-traname.tsv

```
userid \t timestamp \t musicbrainz-artist-id \t artist-name \t musicbrainz-track-id \t track-name
```

#### userid-profile.tsv

```
userid \t gender ('m'|'f'|empty) \t age (int|empty) \t country (str|empty) \t signup (date|empty)
```

### Example:

#### userid-timestamp-artid-artname-traid-traname.tsv

```
user_000639 \t 2009-04-08T01:57:47Z \t MBID \t The Dogs D'Amour \t MBID \t Fall in Love Again?
user_000639 \t 2009-04-08T01:53:56Z \t MBID \t The Dogs D'Amour \t MBID \t Wait Until I'm Dead
...
```

#### userid-profile.tsv

```
user_000639 \t m \t Mexico \t Apr 27, 2005
...
```

### License

The data contained in `lastfm-dataset-1K.tar.gz` is distributed with permission of <a href="http://last.fm">Last.fm</a>. 

The data is made available for non-commercial use.

Those interested in using the data or web services in a commercial context should contact <i>partners [at] last [dot] fm</i>.

For more information see Last.fm <a href="http://www.last.fm/api/tos">terms of service</a>.

### Acknowledgements

Thanks to <a href="http://last.fm">Last.fm</a> for providing the access to this data via their web services. 

Special thanks to <a href="http://www.last.fm/user/nova77LF">Norman Casagrande</a>.

### References

When using this dataset you must reference the <a href="http://last.fm">Last.fm</a> webpage.

Optionally (not mandatory at all!), you can cite <i>Chapter 3</i> of <a href="../MusicRecommendationBook/index.html">this book</a>

```
@book{Celma:Springer2010,
  author = {Celma, O.},
  title = {{Music Recommendation and Discovery in the Long Tail}},
  publisher = {Springer},
  year = {2010}
}
```

### Contact

This data was collected by <a href="http://www.dtic.upf.edu/~ocelma/">Òscar Celma</a> @ <a href="http://mtg.upf.edu">MTG</a>/<a href="http://upf.edu">UPF</a>
