[![Build Status](https://github.com/andgineer/garmin-daily/workflows/Test/badge.svg)](https://github.com/andgineer/garmin-daily/actions)
[![Coverage Status](https://coveralls.io/repos/github/andgineer/garmin-daily/badge.svg?branch=main)](https://coveralls.io/github/andgineer/garmin-daily?branch=main)
# Fill Google Sheets with data from Garmin Connect

![garmin-daily.png](https://andgineer.github.io/garmin-daily/garmin-daily.png)

## User manual

[garmin-daily](https://andgineer.github.io/garmin-daily/en/)

## Developers

### Create / activate environment
    . ./activate.sh

It will also install the package in [edit mode](https://realpython.com/what-is-pip/#installing-packages-in-editable-mode-to-ease-development).

### pre-commit
Do not forget to install, so static check github action won't fail on your commits

    pip install pre-commit
    pre-commit install  # in the project folder

### Scripts
    make help

### API
[Auto-generated reference](https://andgineer.github.io/garmin-daily/api-reference/).

```python
daily = GarminDaily()
daily.login()
day = daily[datetime.date(2023, 4, 15)]
print(day.total_steps)
```

### Garmin Connect credentials
[user manual](https://andgineer.github.io/garmin-daily/en/)

### Docs
Github pages https://andgineer.github.io/garmin-daily/ are auto created from markdown files
in `docs/`.

## Coverage report
* [Codecov](https://app.codecov.io/gh/andgineer/garmin-daily/tree/master/src%2Fgarmin_daily)
* [Coveralls](https://coveralls.io/github/andgineer/garmin-daily)
