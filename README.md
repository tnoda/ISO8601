# ISO8601

ISO8601 is a simple implementation of the ISO 8601 (Data elements and 
interchange formats — Information interchange — Representation of dates and 
times) standard.

## Comments

Because Durations and DateTime has substract method, Durations has sign to represent a negative value:

  * `(ISO8601::Duration.new("PT10S") - ISO8601::Duration.new("PT12S")).to_s #=> "-PT2S"`
  * `(ISO8601::Duration.new("-PT10S") + ISO8601::Duration.new("PT12S")).to_s #=> "PT2S"`


## TODO

* Decimal fraction in dateTime and duration patterns
* Recurring time intervals
* Ordinal date pattern (YYYY-DDD)
* Week date pattern (YYYY-Www-D)

## Contributors

* [Nick Lynch](https://github.com/njlynch)
* [Pelle Braendgaard](https://github.com/pelle)

## Credits
Arnau Siches under [LGPL](http://www.gnu.org/licenses/lgpl.html) license. LICENSE file for details.
