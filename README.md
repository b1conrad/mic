# mic

Music Intrument Checkout

## origin

This project was the work of one afternoon on August 29, 2024 between 1 and 3 p.m.

## requirement

### School of Music instrument rental system
 
#### Users
1. Admin and Student users
2. Admin can add, delete and edit instruments
3. Students can view, reserve and return instruments
4. Logged out can only see the landing page
5. Secure passwords required
6. 2FA optional
7. Verifying admin and student users
8. Notify admin when instrument has been reserved/returned
9. Notification to students about returning instruments
10. Show calendar of when instruments are checked out/available
11. Make sure the website never goes down.
12. Make sure that everything is backed up both physically and to the cloud.
13. Make sure that there are no improper redundancies in place.

#### Instruments
1. Name, description, quantity, price and picture
2. Ability to reserve (student)
3. Ability to check-out for a specific period (Admin)
4. Ability to check-in (Admin)
5. Ability to track all instruments in collection


## approach

Given the short amount of time, while my team discussed our options, I decided to start typing.
Rationale: so that there would be something to see.

### my requirements
For an initial prototype, I elected to not consider authentication, notification, and calendars.
Quite a bit still remains.

#### Users
1. Admin versus anyone else (which latter includes students)
2. Admin can add, delete and edit instruments
3. Anyone (including students) can view instruments
4. Anyone can see the landing page (in fact the only page)
5. Ensure the website never goes down and is backed up (by using GitHub and GitHub pages)

#### Instruments
1. Name and picture
2. Ability to check-out (Anyone, purely locally with no guarantees, by following a manual process)
3. Ability to check-out (Admin, by following a manual process)
4. Ability to check-in (Admin, by following a manual process)
5. Ability to track all instruments in each collection, by following a manual process

## tools

The requirements document (excerpted above), along with three folders full of images were provided to us.

1. WiFi Internet connection provided by the venue
2. Macbook pro running macOS Monterey Version 12.4 (21F79)
3. Google chrome web browser (through which to download what was given, and test during development)
4. Terminal on which a directory was created to receive download and provide `git` repo
5. As editor, `vi`
6. As repository and hosting, GitHub and GitHub pages

## Admin vs Student
Leaving out authentication, etc., how can I claim any difference between admins and students?

An Admin is anyone to whom I have given commit rights in the GitHub repository. See [Admin Instructions](https://b1conrad.github.io/mic/AdminInstructions.html).

Anyone else (including Students) can view the [`index.html`](https://b1conrad.github.io/mic/) page as provided by GitHub pages.
It includes instructions for their part of the manual process.



