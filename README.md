# Selective Page Edit

Use a Selector at the Role-level to grant edit access to a selective group of Pages. 

### Overview

The user must already have page-edit permission on one of their roles in order to get 
edit access to assigned pages. Otherwise, they will only gain view access.

This module is fully functional as-is, but intended as a proof-of-concept for those 
wanting to go further with adding custom edit and/or view access.

NOTE: Original idea is from PageEditPerRole module by Ryan Cramer, http://processwire.com 
I was also borrowed from Ryann Micua's work at https://github.com/ryannmicua/PageEditPerRole/ 

### How to install

1. Copy the SelectivePageEdit folder to /site/modules/
2. Go to Modules in the ProcessWire admin and click "Check for new modules"
3. Click "install" for "Selective Page Edit"

### How to use

1. Under "Access > Roles" locate the role you want to assign edit access to. Edit this role. 
2. Add a standard ProcessWire Selector (http://processwire.com/api/selectors/) to identify Pages that user in this role should be able to edit.
4. Save the role.
5. Under "Access > Users" locate a  non superadmin user you want to apply the role to. Edit this user.
6. For this user's "Roles" field, select the new role you added the Selector to.
7. Save the user and your are done.
8. To test, login as the user you edited to confirm it works how you expect.
