# User Interface Specification Document For User Management Screen

## Requirements:

- Different user types should have different access levels and abilities
- Guests should not access user management page
- Admins should be able to add, delete, edit and list of guests. However admins should not be able to edit or see the personal information(password, phone etc.) of guests
- Admins should be able to see list other admins without their personal information(email, phone, password etc.)
- SuperAdmins should be able to add,delete, edit and list all users. However they should not be able to edit or see the personal information(password, phone etc.) of other users

## Components:

- "Adding New User" button at the top left  
- "Hide Disabled Users" checkbox next of "Adding new user" button
- List for showing users' non-personal information and a textbox to show specific number of users 
- "Edit","delete" and "show info" buttons for each user information row in the list of users

## What to show at the begining:

- Admins should see the list of all guests and admins as well as CRUD action buttons for each user
- SuperAdmins should see the list of all users as well as CRUD action buttons for each user

## UI details

- New user button :
  - It should show "add new user" page as a pop-up when user clicked. 
  - This pop-up page should include label and textboxes for each information type of user , a dropdown list to select the user type and chackbox to enable the user.
  - Pop-up page should also have "save user" button at the down-middle
  - When save user button is clicked, it should show a message box saying "are you sure to add this user"
  - New user will be added if "yes" option is clickled

- "Hide disabled user" checkbox:

  - When this checkbox is not selected, the user should be able to see the list of all users according to their access level
  - When the chechbox is selected, the users should see only the enabled users according to their access level

- User List:

  - Each row should contamine all information type of one user expect the password information
  - It should show all users or enabled users according to "Hide disabled user" checkbox
  - It should have number of pages according textbox to show specific number of users
  - Each row should have "Edit","delete" and "show info" buttons for each user information row

- Textbox to show specific number of users:

  - User should enter the number of users he/she want to see in one page
  - Specified number of users should be shown in one page of the list
