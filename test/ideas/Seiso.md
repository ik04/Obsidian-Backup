## Features:
- take note of each slip
- laundry status 
- laundry agnostic 
- categories for each laundromat 
- save for each user

## Schema: 
- User
- Laundry (seed with formats)
- Slip (related to laundry)

## User:
- email
- name
- password
## Laundry:
- name
- schema
## Slip:
- Schema from Laundry
- user_id
- status

## Routes:
- select laundry 
- add slip, default 0 for each point of schema  
- history 
- fetch schema for filling (FE)
- edit slips not yet processed 
- delete existing unprocessed slips
