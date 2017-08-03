+++
title = "Change Notes"
description = ""
weight = 5
+++
**Here you'll find the changenotes for each version bump**

## 0.0.6 • 2016-08-24

* Added `Rideshare Action` endpoint as real endpoint.

## 0.0.5 • 2016-08-05

* Added `Rideshare` endpoint as real endpoint.

## 0.0.5 • 2016-07-27

* Added `Travel Intent` endpoint as real endpoint.

## 0.0.4 • 2016-07-18

* Added `Travel Intent Pattern` endpoint as real endpoint.

## 0.0.3 • 2016-07-01

* Added `/rideshare-suggestions/{id}/actions` endpoint to trigger state changes on RideShareSuggestions:
  * *The Rideshare Suggestion Action endpoint allows to report an action taken by a related user: Either "ACCEPTED" or "REJECTED".
Based on actor, action and current state of the Suggestion different State Transitions can occur*
* Added `propagated_until` (readOnly, date-time) and `propagation_period` (seconds) on the TravelIntentPattern in order to define when was the last time it was propagated and how long to propagate it to
* Added `new_state` and `old_state` to all entities

## 0.0.2 • 2016-06-29

* Made the TravelIntentPattern a seperate entity and endpoint (instead of embedding it in Travel Intent)
* Changed the format of any `user_id` to be `uuid` instead of `email`
* Added `created` & `modified` to each model (format: `date-time`)

## 0.0.1 • 2016-06-25

* Initial version