# SCF Evaluation data

Documentation: [scholarly-citation-finder.readthedocs.io](http://scholarly-citation-finder.readthedocs.io/en/latest/evaluation/)

### Sets

#### `fire`

1#
```
[
	[AuthorStrategy(ordered=True)],
	[AuthorStrategy(ordered=True, min_year=True)],
	[JournalStrategy(ordered=True)],
	[JournalStrategy(ordered=True, min_year=True)],
	[ConferenceStrategy(ordered=True)],
	[ConferenceStrategy(ordered=True, min_year=True)],
	[AuthorStrategy(ordered=True, recursive=True, min_year=True), JournalStrategy(ordered=True, min_year=True), ConferenceStrategy(ordered=True, min_year=True)]
]
```

2#
```
[
    [AuthorStrategy()],
    [JournalStrategy()],
    [ConferenceStrategy()]
]
```

(3#)
```
[
	[AuthorStrategy(ordered=True, recursive=True)]
]
```