## Precautions:
- rate-limit the server, test rate limit
## Roles (later):
- admin
- Krosschecker (better name plz)
- kontributor
- 
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
-  possible admin types
-  find a way to track deletions (imp)


## Issue:
- How do i handle the updation of content
- Content cap for description
- content size cap

## Todo: 
- [ ] learn how to add columns to an existing db  (years table and column)
- [ ] regex on emails
- [ ] restrict routes
- [ ] how to take backups
- [ ] content tables
- [ ] years table
- [ ] role updation feature (contributer to crosschecker)
- [ ] test update routes
- [ ] better file naming, since multiple files can be uploaded at the same time, something more random
- [ ] service class logic
- [ ] abstractions, hide primary keys and foreign keys
- [ ] error handling
- [ ] add deadline field to asssignments table
- [ ] get user details route (for admin only, to delete accs)
- [ ] add bio field for user (op)
- [ ] delete solutions files when cascade on delete


## Bugs:
- Handle this correctly
![[Pasted image 20231010152904.png]]