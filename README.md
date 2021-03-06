# tvst [![Build Status](https://travis-ci.org/shahriar1/tvst.svg?branch=master)](https://travis-ci.org/shahriar1/tvst)

> TV Shows Tracker (TVST) on command line

![TVST command line](tvst.gif)


## Table of contents
  * [Install](#install)
  * [Upgrade](#upgrade)
  * [Usage](#usage)
    * [Schedule](#schedule)
      * [Examples](#schedule-examples)
        * [See all shows of today](#schedule-examples-today)
        * [See all shows of tomorrow](#schedule-examples-tomorrow)
        * [See all shows of yesterday](#schedule-examples-yesterday)
        * [See all shows of a particular date](#schedule-examples-by-date)
        * [See if tomorrow has a episode of a particular tv show](#schedule-examples-tomorow-particular)
        * [See today's schedule of a particular country](#schedule-examples-country)
    * [Next Episode](#next-episode)
      * [Examples](#next-episode-examples)
        * [See next episode's details of a particular show](#next-episode-examples-details)
    * [Previous Episode](#previous-episode)
      * [Examples](#previous-episode-examples)
        * [See previous episode's details of a particular show](#previous-episode-examples-details)
    * [Favorite Shows](#favorite-shows)
      * [Examples](#favroite-shows-examples)
        * [Add show(s) as your favorite](#favorite-shows-add)
        * [Remove show(s) from your favorite](#favorite-shows-remove)
        * [See schedules of all of your favorite shows](#favorite-shows-schedule)
    * [Help](#help)
    * [Version](#version)
  * [Credits](#credits)
  * [License](#license)


## :punch: More awesome features are in development :punch:

## Install <a name="install"></a>

Install with [npm](https://www.npmjs.com/):

```bash
npm install -g tvst
```
## Upgrade <a name="upgrade"></a>

```bash
npm update -g tvst
```

## Usage <a name="usage"></a>

```

  Usage: tvst [options] [command]


  Commands:

    schedule <date>  Show list of TV shows of a specific date
    ne <show-name>   Date & Air time of next episode of a show
    pe <show-name>   Date & Air time of previous episode of a show
    fav-add          Add TV shows in your favorite list
    fav-list         Show list of your favorite shows
    fav-remove       Remove show(s) from your favorite shows
    help [cmd]       display help for [cmd]

  TV Shows Tracker (TVST) On Command Line - For Developers

  Options:

    -h, --help     output usage information
    -V, --version  output the version number

```   


### Schedule - `schedule` <a name="schedule"></a>
```
tvst schedule <date>
```

#### Usage of schedule

```
$ tvst schedule --help

  Usage: tvst-schedule [options]

  Options:

    -h, --help              output usage information
    -c --country <country>  ISO Country Code - eg. US or GB etc.
    -f --filter <filter>    Filter By Show Name
```


#### Examples: <a name="schedule-examples"></a>

- See all shows of today: <a name="schedule-examples-today"></a>
```bash
tvst schedule today
```

- See all shows of tomorrow: <a name="schedule-examples-tomorrow"></a>
```bash
tvst schedule tomorrow
```

- See all shows of yesterday: <a name="schedule-examples-yesterday"></a>
```bash
tvst schedule yesterday
```

- See all shows of a particular date: <a name="schedule-examples-by-date"></a>
```bash
tvst schedule '2016-06-14'
```

- See if tomorrow has a episode of a particular tv show: <a name="schedule-examples-tomorow-particular"></a>
```bash
tvst schedule tomorrow -f 'game of thrones'
```

- See today's schedule of a particular country: <a name="schedule-examples-country"></a>
```bash
tvst schedule today -c GB
```


### Next Episode - `ne` <a name="next-episode"></a>
```
tvst ne <show-name>
```

#### Examples <a name="next-episode-examples"></a>

- See next episode's details of a particular show: <a name="next-episode-examples-details"></a>
```bash
tvst ne 'game of thrones'
```

:notebook_with_decorative_cover: If you're not sure about spelling of a specific show name, just guess, it will return list of possible shows


:notebook_with_decorative_cover: If any show has no update of next episode then it returns details of previous episode


### Previous episode - `pe` <a name="previous-episode"></a>


```bash
tvst pe <show-name>
```

#### Examples  <a name="previous-episode-examples"></a>

- See previous episode's details of a particular show: <a name="previous-episode-examples-details"></a>
```bash
tvst pe 'game of thrones'
```

:notebook_with_decorative_cover: If you're not sure about spelling of a specific show name, just guess, it will return list of possible shows

### Favorite shows - `fav-add` `fav-remove` `fav-list` <a name="favorite-shows"></a>
```bash
tvst fav-add
```
```bash
tvst fav-remove
```
```bash
tvst fav-list
```

#### Examples <a name="favorite-shows-examples"></a>
- Add show(s) to your favorite: <a name="favorite-shows-add"></a>
```bash
tvst fav-add
```
:notebook_with_decorative_cover: It is an interactive command - just follow the instruction.

- Remove show(s) from your favorite: <a name="favorite-shows-remove"></a>
```bash
tvst fav-remove
```
:notebook_with_decorative_cover: It is an interactive command - just follow the instruction.

- See schedules of all of your favorite shows: <a name="favorite-shows-schedule"></a>
```bash
tvst fav-list
```

:notebook_with_decorative_cover: If you're not sure about spelling of a specific show name, just guess, it will return list of possible shows

### Help <a name="help"></a>
```bash
tvst help
```

### Version <a name="version"></a>
```bash
tvst --version
```


## Credits
###### [TVMaze API](http://tvmaze.com/api)


## License

The MIT @ [Shahriar Mahmood](https://github.com/shahriar1)
