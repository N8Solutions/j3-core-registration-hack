# j3-core-registration-hack
Joomla v3.10.12 hack of the registration.php file to show user custom fields in the admin notificaiton email for new user registrations.

The code modifications will append the custom fields that are added to the Joomla registration page to the notification email that administrators will receive when a user signs up for an account.

This works by placing User Custom Fields into a Field Group, then staticly referencing the ID of each Field Group that you want added to the notification email.

The path for the core registration file is `/components/com_users/models/registration.php`

The modified section is `COM_USERS_EMAIL_REGISTERED_NOTIFICATION_TO_ADMIN_BODY`.

This is the full registration.php file with the modifications.

> [!NOTE]
> The code is annotated in the file for easy reference starting at line **607**.
> Line **616** is where you adjust the ID's for the custom field groups that you want added to the notification email.

> [!CAUTION]
> Note: Under normal circumstances you should not hack the core Joomla files. This was done only because Joomla v3 is EOL but still receiving extended security updates.
> If you use this file, and if you subscribe to those updates, please be sure to check the file after updating to make sure the changes to this file do not get overwritten.
