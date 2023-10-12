## Spitballin and ideas:
- manual assignment integ (make a portal for this which only i can access (hard code creds))
- upload solutions in solutions section
- get solutions form others through (make a different portal that only allows only solutions that too queue) (creep later)
- better card ui design 
- framer animation integ (future)
- ## group by years (after current sem, feature creep)
- years table (get all possible subjects to make it usable by anyone)
- karma feature (feature creep)
- integrate llama to check code snippet validity (feature creep)
- roles (krosscheckers, admin, kontributors)
- only one login portal for all accs and accs to be made manually
- illama or gpt integration for better answers
- register as contributer today?
- contribution stats in profile page
- add profile pic (feature creep)
- switch to postgres or mysql
- report (far far future)
- flush function to get rid of data (cronjob, every week/5 days )
- only 1 answer per assignment (constraint using composite key)
- year sort in future
- realtime scrapper to get data
- profile page will have stats of answers


## Ideas:
- Resources section
- OAuth integration

## Todo:
- [x] Make Role enum
- [x] Make middllewares for kontributors and krosscheckers
- [x] Addition routes for assignment 
- [x] Make de-alias functions to get the actual id of the elements
- [x] Link up the tables user, subject, assignment, solution
- [x] Make get routes 
- [x] design kontibute page\
- [ ] extend landing page
- [ ] make site responsive 
- [ ] test test test (v important)
- [x] test out content field
- [x] cron job to delete files once assigments are deleted
- [ ] content table to allow more than one file (creep)
- [ ] map the downloads onto the fe and find a way to preview
- [ ] make just assignments page
- [ ] add shadcnUI
- [ ] add ssr to prevent panel acccess for non users



## Routes to make:
- [x] get assigments by subject
- [x] get solutions by assignment (map user too)
- [ ] getting solutions for an assignment (separate or togather)
- [ ] test the routes/try out phpunit?





## Architecture and specifics:
- [[KaizenKlass BE]]
- [[KaizenKlass FE]]
- [[KaizenKlass Hosting]]
- [[KaizenKlass App]]

## Caution:
- Don't expose sensitive data, store it in a env or file and gitignore it 
- when refactoring make the fe code flexible so that changes to the backend maintain integrity


## Armaan improvements:
- Relations
- service class logic
- unset function php
- str class instead of uuid (illuminate/support/str)::uuid
- welcome flow (register->generate a token right away)
- improve route naming (eg:/assignments/{uuid}/solutions/add)
- docs for routes
- Test Armaan changes
- mobile first

## Common issues:
- cookie not being saved cuz site on local host not 127.0.0.1:3000 (they both gotta be on the same thing)

