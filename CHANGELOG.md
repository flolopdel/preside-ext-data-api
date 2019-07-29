# Changelog

## v3.0.0

### Administration

* Add admin UI for managing individual user access to entities, verbs and queues

### Queue enhancements

* Ability to turn off the queue feature entirely
* Ability to turn off the queue feature per object
* Allow queue to contain atomic data changes
* Allow queue to return configurable number of records, rather than always 1
* Allow multiple queues for different groups of objects and with individual queue settings

### Documentation enhancements

* Add new plain HTML documentation endpoint
* Object properties should be able to specify type and format for their spec definitions
* Ability to categorize entities (applies to HTML documentation only)
* Ability to set sort order on entities
* Ability to set favicon for an API
* Use plural name of entity for default entity tag name

### Miscellaneous

* Automatically convert foreign keys to assets, links and pages to URLs.
* Ability to exclude/include properties in the API through annotations on the properties

### Bug fixes

* Documentation of foreign keys: only use 'Foreign Key UUID' format when it really is a UUID (i.e., not for int)
* Do not show authentication description when API does not use authentication


## v2.0.2

* Fix path to docs

## v2.0.1

* Better handling of namespaced routes and handler paths
* Update queues to allow namespacing

## v2.0.0

* Add support for multiple configured APIs via namespacing
* Add `dataApiSavedFilters` annotation

## v1.0.19

* Total record count should return filtered count if filter is applied

## v1.0.18

* Prevent stack overflow with recursive loading of services on application startup

## v1.0.17

* [#2](https://github.com/pixl8/preside-ext-data-api/issues/2): Add preValidate interception point for upsert operations

## v1.0.16

* Fixes [#1](https://github.com/pixl8/preside-ext-data-api/issues/1): ensure that booleans are rendered as 'true' or 'false', not '1' or '0'

## v1.0.15

* Add general error message documentation
* When POSTing (creating records), do not ignore missing fields

## v1.0.14

* Add option for specifying whether or not ID field creation is supported

## v1.0.5-1.0.13

* Refactoring build system

## v1.0.4

* Change queue logic so that fetching next item from queue always returns the same item *until* the API user manually removes it from the queue

## v1.0.3

* Fix interceptor logic to not break deletes that use a filter other than record IDs

## v1.0.2

* Improve documentation of queue system API
* Fix the possible field list for the 'fields' REST API param
* Allow for default descriptions of commonly named fields

## v1.0.1

* Initial release