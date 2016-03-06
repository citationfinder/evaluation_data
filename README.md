

### Structure evaluation set

```
<set_name>
  |
  |- authors.csv
  |- celery.log
  |- meta_<strategy_name>.csv
  |- <strategy_name>
      |- <author_id>.csv
```

### Sets

#### `fire`

#1
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

#2
```
[
    [AuthorStrategy()],
    [JournalStrategy()],
    [ConferenceStrategy()]
]
```