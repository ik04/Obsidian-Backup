## Roles (later):
- admin
- Krosschecker (better name plz)
- kontributor
## Models:
- subjects
- roles (enum)
- assignment
- solution
- user
- Test papers
- content (for solution)
- content (for assignment)


## Fields (problems):
## Content (assignment):
- pdfs, photos, txt 
- deadline: in description for now (coming soon/add to assignment as nullable?)



## Role Methods and other features:
- create assignments (admin)
- create solutions (contributer/admin/crosschecker)
- edit existing responses (optional) (crosschecker/admin)
- add subjects (admin)
- delete subject (admin)
- add years (feature creep) (admin)
- only get assignments that're within the deadline/ make it so the assignments are ordered by time stamp when fetched (can add more features) (cronjob/filter)
- edited by (optional)
- add backup functionality to backup users and data
- allow updation of soltions and assignments and solutions by krosscheckers and admin only (admin and kross)
- update own answers (all users)
- update others answers (kross and admin)
- delete own answers (all users)
- delete others answers (admin and kross)
- update user role (admin)
- show edited by in the future



## Issue:
- How do i handle the updation of content
- Content cap for description

## Todo: 
- [ ] learn how to add columns to an existing db  (years table and column)
- [ ] regex on emails
- [ ] restrict routes
- [ ] how to take backups