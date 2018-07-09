## Congress API changelog

#### 2018-07-09

* Fixed DW-Nominate score loader.

#### 2018-06-14

* Added `last_updated` attribute to list of members and member detail responses.

#### 2018-06-05

* Added lobbying responses. ([Issue 207](https://github.com/propublica/congress-api-docs/issues/207))

#### 2018-05-22

* Added response for statements that mention a specific bill. ([Issue 205](https://github.com/propublica/congress-api-docs/issues/205))

#### 2018-03-15

* Added `gender` to member list responses. ([Issue 195](https://github.com/propublica/congress-api-docs/issues/195))

#### 2018-03-12

* Fixed invalid JSON bug in hearings response. ([Issue 200](https://github.com/propublica/congress-api-docs/issues/200))

#### 2018-02-16

* Updated documentation to specify proper syntax for current member by district response for at-large districts. ([Issue 196](https://github.com/propublica/congress-api-docs/issues/196))
* Updated chair and ranking member information for current committees. ([Issue 193](https://github.com/propublica/congress-api-docs/issues/193))
* Added data for congressional committees for 113th and 114th congresses. ([Issue 189](https://github.com/propublica/congress-api-docs/issues/189))

#### 2018-02-06

* Fixed several issues impacting votes by date responses and some individual vote responses. ([Issue 192](https://github.com/propublica/congress-api-docs/issues/192))

#### 2018-02-02

* Fixed bug that resulted in list of committees requests not working for 113th and 114th congresses. ([Issue 189](https://github.com/propublica/congress-api-docs/issues/189))
* Fixed bug that resulted in committees not displaying as part of member detail XML responses. ([Issue 190](https://github.com/propublica/congress-api-docs/issues/190))

#### 2017-12-22

* Added more personal explanation endpoints, including responses for individual members and votes, and by category (docs [here](https://projects.propublica.org/api-docs/congress-api/votes/#personal-explanations)).

#### 2017-12-13

* All `not_voting` attributes on JSON Get a Specific Roll Call Vote endpoints return integers instead of strings.

#### 2017-12-05

* Fixed a bug with House Speaker election votes in Specific Member's Vote Positions responses.

#### 2017-12-02

* Fixed `num_results` value on Get Recent Committee Hearings responses to show total number of hearings for the given congress.
* Fixed `num_results` value on bills by subject response to show total number of bills for the given subject.
* Fixed `enacted` date on bill responses and updated dates for 115th Congress bills. ([Issue 89](https://github.com/propublica/congress-api-docs/issues/89))

#### 2017-11-29

* Added `suffix` attribute to member responses. ([Issue 180](https://github.com/propublica/congress-api-docs/issues/180))

#### 2017-11-27

* Fixed bug with displaying At-large districts. ([Issue 181](https://github.com/propublica/congress-api-docs/issues/181))

#### 2017-11-15

* Fixed quote-escaping issue with `latest_major_action` in some bill responses.

#### 2017-11-07

* Added `last_vote` to bill responses. ([Issue 177](https://github.com/propublica/congress-api-docs/issues/177))
* Made most bill responses (related bills, subject bills and cosponsored bills) match bill list responses. (Related to #177)

#### 2017-10-27

* Fixed `num_results` on statements by member responses.
* Fixed a bug with bill search JSON responses.
* Removed HTML encoding from committeee & subcommittee member names and also bill sponsor names. ([Issue 108](https://github.com/propublica/congress-api-docs/issues/108))
* Fixed an issue with the bill schedule loader.

#### 2017-10-18

* Fixed vote responses to remove nomination details from `bill` attribute. ([Issue 171](https://github.com/propublica/congress-api-docs/issues/171))
* Fixed bill loader to always load both official and short titles.
* Added `sponsors_by_party` and `short_title` to Get Recent Bills by a Specific Member response. ([Issue 163](https://github.com/propublica/congress-api-docs/issues/163))

#### 2017-10-17

* On statement search, `num_results` now represents the total number of search results (aids in pagination).

#### 2017-10-12

* Added `fec_candidate_id` to member list responses. ([Issue 165](https://github.com/propublica/congress-api-docs/issues/165))
* Added `cosponsors_by_party` to bills list and detail responses. ([Issue 163](https://github.com/propublica/congress-api-docs/issues/163))
* For votes by date responses and votes by member responses in which there is no bill in our database, still display some `bill` attributes like we do on vote detail responses.
* Added `sponsor_id` to bill attributes in votes responses. ([Issue 168](https://github.com/propublica/congress-api-docs/issues/168))

#### 2017-10-04

* Added `side` and `title` to committee and subcommittee portions of member detail responses for 115th Congress. ([Issue 160](https://github.com/propublica/congress-api-docs/issues/160))

#### 2017-09-29

* Added `short_title` to member responses ([Issue 155](https://github.com/propublica/congress-api-docs/issues/155))
* Statement search now supports full text search.

#### 2017-09-21

* Added `bill_ids` to Floor Action responses. ([Issue 153](https://github.com/propublica/congress-api-docs/issues/153))

#### 2017-09-11

* Added `bill_ids` to Committee Hearing responses. ([Issue 151](https://github.com/propublica/congress-api-docs/issues/151))
* Added `url` to former members elements in committee responses with link to Congressional Record section describing resignation.
* Added `parent_committee_id` to subcommittee objects on member responses. ([Issue 126](https://github.com/propublica/congress-api-docs/issues/126))

#### 2017-09-07

* Fixed unescaped quote marks in related bills responses. ([Issue 149](https://github.com/propublica/congress-api-docs/issues/149) and [Issue 150](https://github.com/propublica/congress-api-docs/issues/150))
* Removed `domain` from member responses. ([Issue 145](https://github.com/propublica/congress-api-docs/issues/145))
* Fixed bug that permitted committee API requests to use the wrong chamber. ([Issue 139](https://github.com/propublica/congress-api-docs/issues/139))
* Fixed `rank_in_party` for joint committees. ([Issue 142](https://github.com/propublica/congress-api-docs/issues/142) and [Issue 141](https://github.com/propublica/congress-api-docs/issues/141))

#### 2017-09-06

* Fixed unescaped quote marks in floor update responses. ([Issue 146](https://github.com/propublica/congress-api-docs/issues/146))
* Fixed Senate subcommittees bug affecting committee responses. ([Issue 144](https://github.com/propublica/congress-api-docs/issues/144))


#### 2017-09-05

* Added upcoming bills responses. ([See Docs](https://projects.propublica.org/api-docs/congress-api/bills/#get-upcoming-bills))
* Member position response now supports offset parameter. ([Issue 147](https://github.com/propublica/congress-api-docs/issues/147))
* Added `chamber` to committee members. ([Issue 140](https://github.com/propublica/congress-api-docs/issues/140))

#### 2017-08-28

* Added sponsor details to related_bills responses.
* Fixed vote detail responses for elections of Speaker of the House. ([Issue 102](https://github.com/propublica/congress-api-docs/issues/102))
* Added `amendment` element to vote detail responses. ([Issue 96](https://github.com/propublica/congress-api-docs/issues/96))
* Removed HTML encoding from bill subjects responses. ([Issue 130](https://github.com/propublica/congress-api-docs/issues/130))
* Added `subcommittees` element to member detail responses. ([Issue 126](https://github.com/propublica/congress-api-docs/issues/126))

#### 2017-08-23

* Presidential bill actions no longer have a `chamber` value. ([Issue 123](https://github.com/propublica/congress-api-docs/issues/123))

#### 2017-08-22

* Added response for subcommittee detail. ([Issue 121](https://github.com/propublica/congress-api-docs/issues/121))
* Removed HTML encoding in bill actions. ([Issue 122](https://github.com/propublica/congress-api-docs/issues/122))
* Included `side` attribute in committee memberships. ([Issue 119](https://github.com/propublica/congress-api-docs/issues/119))
* Fixed empty strings on some joint committees. ([Issue 118](https://github.com/propublica/congress-api-docs/issues/118))
* Fixed committee name attribute on committee detail response. ([Issue 115](https://github.com/propublica/congress-api-docs/issues/115))
* Removed HTML encoding in floor update responses. ([Issue 112](https://github.com/propublica/congress-api-docs/issues/112))


#### 2017-08-21

* Make `rank_in_party` on committee detail responses an integer. ([Issue 120](https://github.com/propublica/congress-api-docs/issues/120))
* Added committee `id` to committee detail responses. ([Issue 117](https://github.com/propublica/congress-api-docs/issues/117))
* Replaced empty strings on committee responses. ([Issue 118](https://github.com/propublica/congress-api-docs/issues/118))
* Added `chamber` to each committee on committee list responses. ([Issue 113](https://github.com/propublica/congress-api-docs/issues/113))
* Added `chair_state`, `chair_party` and `chair` attributes to committee detail responses. ([Issue 114](https://github.com/propublica/congress-api-docs/issues/114))


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
