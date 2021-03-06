# jQuery ellipsis [![Build Status](https://travis-ci.org/STAR-ZERO/jquery-ellipsis.png?branch=master)](https://travis-ci.org/STAR-ZERO/jquery-ellipsis) [![Coverage Status](https://coveralls.io/repos/STAR-ZERO/jquery-ellipsis/badge.png?branch=master)](https://coveralls.io/r/STAR-ZERO/jquery-ellipsis?branch=master) [![Dependency Status](https://gemnasium.com/STAR-ZERO/jquery-ellipsis.png)](https://gemnasium.com/STAR-ZERO/jquery-ellipsis)

Originally built by [Kenji Abe (STAR-ZERO)][kenji].

[kenji]:https://github.com/STAR-ZERO

Support truncating text after multiple lines with ellipses.

## Getting Started
Download the [development version][max].

[max]: https://raw.github.com/cpburnz/jquery-ellipsis/master/dist/jquery.ellipsis.js


## Usage

Fit one line

```
$('#target').ellipsis();
```

Fit on two lines in the case of two or more lines

```
$('#target').ellipsis({
    row: 2
});
```

Change ellipsis character

```
$('#target').ellipsis({
    row: 2,
    char: '**'
});
```

Only include full words (remove word fragments at the end)

```
$('#target').ellipsis({
    row: 2,
    onlyFullWords: true
});
```

Callback function

```
$('#target').ellipsis({
    callback: function() {
        console.log($(this).text());
    }
});
```

Ellipsis for middle position

```
$('#target').ellipsis({
    position: 'middle'
});
```

Ellipsis for tail position

```
$('#target').ellipsis({
    position: 'tail'
});
```

## License
jquery-ellipsis is available under the terms of the [MIT License](https://github.com/STAR-ZERO/jquery-ellipsis/blob/master/LICENSE-MIT).

