## Original endpoint:
- https://api.crunchbase.com/api/v4/entities/organizations/tesla-motors?user_key=4ff906e99dd65901d37098b95a2a9485

## Output:

```json
{

"properties": {

"identifier": {

"uuid": "a367b036-5952-5435-7541-ad7ee8869e24",

"value": "Tesla",

"image_id": "dj8rndg9wkqkpgvplvzi",

"permalink": "tesla-motors",

"entity_def_id": "organization"

}

}

}
```
## Explanation:
calling this end point as it is only gets the most basic info and wouldn't have served to enrich data and is insufficient

## New endpoint:
- https://api.crunchbase.com/api/v4/entities/organizations/gobaby-2?card_ids=acquiree_acquisitions,acquirer_acquisitions,child_organizations,child_ownerships,event_appearances,fields,founders,headquarters_address,investors,ipos,jobs,key_employee_changes,layoffs,parent_organization,parent_ownership,participated_funding_rounds,participated_funds,participated_investments,press_references,raised_funding_rounds,raised_funds,raised_investments&field_ids=categories,short_description,rank_org_company,founded_on,website,facebook,created_at&user_key=4ff906e99dd65901d37098b95a2a9485

this is the same endpoint but i tried all possible card_ids in an attempt to fetch all the cards, 
i also took the field_ids to get more data related to the organzation

## Output:
```json


{

"properties": {

"identifier": {

"uuid": "1dcf3d60-e7a2-95f0-0fbb-0c7a307184c0",

"value": "goBaby",

"image_id": "v1485305805/htbednnsfgdbm8zhd0zp.png",

"permalink": "gobaby-2",

"entity_def_id": "organization"

},

"short_description": "The Airbnb for baby gear rentals.",

"facebook": {

"value": "https://www.facebook.com/goBaby.co"

},

"created_at": "2016-03-10T09:00:04Z",

"rank_org_company": 110157

},

"cards": {

"fields": {

"rank_delta_d30": -0.3,

"image_url": "https://images.crunchbase.com/image/upload/t_cb-default-original/v1485305805/htbednnsfgdbm8zhd0zp.png",

"diversity_spotlights": [

{

"uuid": "212d952e-261d-40db-8311-a6b4c3c94c6a",

"value": "Women Founded",

"permalink": "women-founded",

"entity_def_id": "diversity_spotlight"

},

{

"uuid": "5b651b5d-f338-4204-90b3-0c18aff46b9f",

"value": "Women Led",

"permalink": "women-led",

"entity_def_id": "diversity_spotlight"

}

],

"identifier": {

"uuid": "1dcf3d60-e7a2-95f0-0fbb-0c7a307184c0",

"value": "goBaby",

"image_id": "v1485305805/htbednnsfgdbm8zhd0zp.png",

"permalink": "gobaby-2",

"entity_def_id": "organization"

},

"linkedin": {

"value": "https://www.linkedin.com/company/gobaby"

},

"short_description": "The Airbnb for baby gear rentals.",

"rank_org": 111443,

"facebook": {

"value": "https://www.facebook.com/goBaby.co"

},

"created_at": "2016-03-10T09:00:04Z",

"location_identifiers": [

{

"uuid": "d64b7615-985c-fbf4-4aff-aa89d70c4050",

"value": "New York",

"permalink": "new-york-new-york",

"entity_def_id": "location",

"location_type": "city"

},

{

"uuid": "83ead471-332b-d02e-67b7-67279aed075b",

"value": "New York",

"permalink": "new-york-united-states",

"entity_def_id": "location",

"location_type": "region"

},

{

"uuid": "f110fca2-1055-99f6-996d-011c198b3928",

"value": "United States",

"permalink": "united-states",

"entity_def_id": "location",

"location_type": "country"

},

{

"uuid": "b25caef9-a1b8-3a5d-6232-93b2dfb6a1d1",

"value": "North America",

"permalink": "north-america",

"entity_def_id": "location",

"location_type": "continent"

}

],

"twitter": {

"value": "https://twitter.com/gobabyco"

},

"rank_delta_d90": -0.2,

"website_url": "http://www.gobaby.co",

"updated_at": "2022-07-19T02:46:26Z",

"rank_delta_d7": 0.2

}

}

}
```
```