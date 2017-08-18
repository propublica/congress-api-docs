## Congress API changelog


#### 2017-08-18

* Allow `both` as a value for vote date range requests. ([Issue 95](https://github.com/propublica/congress-api-docs/issues/95))

#### 2017-08-15

* Fixed `source` and `url` attributes of Senate votes to use https: ([Issue 91](https://github.com/propublica/congress-api-docs/issues/91))
* Added member details to vote responses. ([Issue 97](https://github.com/propublica/congress-api-docs/issues/97))
* Removed HTML encoding of member and committee names. ([Issue 84](https://github.com/propublica/congress-api-docs/issues/84) and [Issue 108](https://github.com/propublica/congress-api-docs/issues/108))
* Added `bill_id` to member vote position responses. ([Issue 104](https://github.com/propublica/congress-api-docs/issues/104))

#### 2017-07-28

* Updated amendment responses.
* Fixed Get Recent Bills for Member responses and added new fields.

#### 2017-07-24

* `both` chamber parameter on Get Recent Bills now applies to all responses, not just `passed`
* Fixed full name display for members. ([Issue 70](https://github.com/propublica/congress-api-docs/issues/70))
* Added `cosponsor_state` and `cosponsor_party` to bill cosponsors response. ([Issue 69](https://github.com/propublica/congress-api-docs/issues/69))


#### 2017-07-19

* Added full text search for bills.
* Better null value display for bills and members. ([Issue 36](https://github.com/propublica/congress-api-docs/issues/36))
* Added first, middle and last name attributes to Get Current Members by State/District responses.

#### 2017-07-14

* Added `has_bills` and `has_statements` to subjects responses
* Added sponsor details to bill lists responses
* Made boolean responses for member#in_office and bill#active actual JSON booleans.

#### 2017-07-13

* Bill detail responses now contain complete summary if available.

#### 2017-07-10

* Added `url` to committee detail responses

#### 2017-06-21

* Added `chamber` and `action_type` to bill actions responses.
* Added `committee_codes` and `subcommittee_codes` to bill detail responses.

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
