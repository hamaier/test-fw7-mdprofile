# Alaska Region mdEditor profiles

The [mdEditor](mdEditor) is designed to support creating metadata for a wide variety of data types. As a result, an edit session will likely display much more information than is required for the data that you are describing. Applying a profile allows a user to hide menus and data fields that may not be required for a given use case.

The mdEditor defaults to the "Full Profile" when a metadata record is first created, dsplaying all available menus and data entry fields.

When editing a record, a [Profile Seletion](https://guide.mdeditor.org/tutorial/editor-window-parts/primary-navigation.html#profile) field is displayed on the the mdEditor [Primary Navigation Bar](https://guide.mdeditor.org/tutorial/editor-window-parts/primary-navigation.html). A selected profile will remain associated with metadata record until change during an edit session.


For more information see the mdEditor [Core Profile Definitions](https://adiwg.github.io/mdProfiles/) page.

# Creating a profiles
A discussion of creating profiles is beyond the scope of this documentation. Contact your Data Manager or Data Steward for assistance.

# Installing a profile
Identify url for the custom profile definition file (use "raw." version)

## Add profile Definition
  1. Goto Settings/Profiles/Manage Definitions
  2. Select "Add Definition"
  3. Select "Imported" tab.
  4. Enter URL to profile definition
  5. Enter an optional alias for profile name (alias is displayed when selecting a profile to add)
  4. Select "Save definition". You should receive a notification that the profile has been downloaded.

## Add profile for use by mdEditor
  1. Go to Settings/Profiles
  2. Select "Add Profile"
  3. Add "Title" (displayed in profile selection box) and optional description (mouse-over help provided in profile selection box)
  4. Select a "Profile Definition" from dropdown list (the alias entered in the previous step be displayed)
  5. Identify a schema from the "Selected Schema" list and select "Add"
  6. Select "Save Profile"

Notes:
Changes made to a profile that is loaded in the profile selection field will not be reflected until the editor is reloaded.

Add Validation Schema:
  Go to Settings/validation
  Select "Add Schema"
  Enter URL to the schema root (e.g. https://raw.githubusercontent.com/adiwg/mdJson-schemas/master/schema/schema.json)
  Provide a Title, Description and Type
  Save the schema

Apply Schema to profile. See: Add Schema

# Updating a profile
=================================================
Update profile:
=================================================
	1. Goto Settings/Profiles/Manage Definitions
	2. Select "Check for Updates"
	3. A blue information icon next to profile definition indicates that an update is available
	4. Select the definition "Edit" button. (The currently installed version will be displayed along with the updated version in a blue box)
	5. Select "Update Definition" button to proceed with update.
	6. Refresh browser to activate updated profile.



=================================================
Add schema:
=================================================
Core Schema:
	https://raw.githubusercontent.com/adiwg/mdJson-schemas/master/schema/schema.json

Identify url for the custom schema definition file
	https://github.com/adiwg/mdJson-schemas/raw/master/schema/contact.json
	https://raw.githubusercontent.com/hamaier/test-fw7-mdprofile/master/ak_schema/contact2.json

Add validation schema
	1. Goto Settings/Profiles/Validation
	2. Select "Add Schema"
	3. Enter URL to root schema
	4. Enter an optional description
	5. Select schema "type"
	6. Select "Save Schema". You should receive a notification that the profile has been downloaded.

=================================================
References:
=================================================
test-fw7-mdprofile
	https://github.com/hamaier/test-fw7-mdprofile

Core Profile Definitions for the mdEditor
	https://adiwg.github.io/mdProfiles/

ADIwg mdProfiles:
	https://github.com/adiwg/mdProfiles

mdJson-schemas:
	https://github.com/adiwg/mdJson-schemas

Regional profile definition (TidiedAlaskaMetadataProfile.xlsx)
	- https://doimspp.sharepoint.com/:x:/r/sites/AlaskaDataStewardship/Shared%20Documents/metadata/TidiedAlaskaMetadataProfile.xlsx?d=w655cae781d3e4e79b2799c6b5419ffec&csf=1&web=1&e=jAmqA7
	- https://doimspp.sharepoint.com/:f:/r/sites/AlaskaDataStewardship/Shared%20Documents/metadata?csf=1&web=1&e=r6Exoz


---
# References
  - [mdEditor](https://www.mdeditor.org/)
  - [mdEdiorGuide](https://guide.mdeditor.org/)
