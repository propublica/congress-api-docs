## Congress API changelog

#### 2017-06-14

* Added `enacted` and `vetoed` as types for recent bills responses. ([Issue 18](https://github.com/propublica/congress-api-docs/issues/18))
* Display integers and boolean values as native data types in JSON responses. ([Issue 26](https://github.com/propublica/congress-api-docs/issues/26))
* Added response to search bill subjects.
* Added committee hearing responses.
* Added personal explanation responses.
* Added floor updates responses. ([Issue 16](https://github.com/propublica/congress-api-docs/issues/16))
* Added response to retrieve bills by subject. ([Issue 20](https://github.com/propublica/congress-api-docs/issues/20))
* Updated example JSON for bills responses.

#### 2017-06-07

* Fixed bill action date timezone bug.
* Added `date_of_birth` to Member list responses.

#### 2017-05-31

* Added `geoid` attribute to House member list endpoint, based on [Census geoidentifiers](https://www.census.gov/geo/reference/geoidentifiers.html) ([Issue 27](https://github.com/propublica/congress-api-docs/issues/27)).
