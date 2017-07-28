+++
title = "Api behaviour Notes"
description = ""
+++

There are some important notes to take it in a consideration when you are working with our travel matching API.


* Driver can only pick one passenger.

* There is no drop-off location. Passenger and driver must go to the same place.

* Our endpoints is not named in usual way eg. /api/travel-intent-pattern/v1/travel-intent-pattern/

* Don't use same value for  `driver_id` & `passenger_id` when filtering rideshare.

    Example: `rideshare/v1/rideshare/?driver_id=samething&passenger_id=samething` wont work

* Rideshares can occur between communities. Thus in each rideshare entity, there is `driver_community_id` and `passenger_community_id`

* You can NOT create a rideshare by itself. Thus you can't make a POST request to `rideshare/v1/rideshare/`
