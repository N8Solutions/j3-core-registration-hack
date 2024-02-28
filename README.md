# j3-core-registration-hack
Joomla v3.10.12 hack of the registration.php file to show user custom fields in the admin notificaiton email for new user registrations.

The code modifications will append the custom fields that are added to the Joomla registration page to the notification email that administrators will receive when a user signs up for an account.

This works by placing User Custom Fields into a Field Group, then staticly referencing the ID of each Field Group that you want added to the notification email.

The path for the core registration file is `/components/com_users/models/registration.php`

The modified section is `COM_USERS_EMAIL_REGISTERED_NOTIFICATION_TO_ADMIN_BODY`.

The code is annotated in the file for easy reference.
