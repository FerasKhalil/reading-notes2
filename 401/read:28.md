# Read: Class 28 Django CRUD and Forms
## Django Forms
- An HTML frrom is a group of one or more fields/ widgets on a web page, which can be used to collect information
	from users for submission to a server.
- Forms are a flixible mechanism for collecting user input.
- Can make form out of text fields, radiobuttons, checkboxes and all html inputs.
	- Source from (https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)

- The main things that django's form does are:
	1. Display the default form the first time it is requested by a user.
	2. Receive data from a submit request and bind it to the form.
	3. Clean and validate the data.
	4. Re-display the form if any data is invalid.
	5. Perform required actions if the data was valid.
	6. Redirect the user to another page once all actions are complete.

- You should import forms in order to be able to use it.
	- from django import forms


- The arguments that are common to most fields are listed below (these have sensible default values):

	- required: If True, the field may not be left blank or given a None value. Fields are required by default, so you would set required=False to allow blank values in the form.
	- label: The label to use when rendering the field in HTML. If a label is not specified, Django will create one from the field name by capitalizing the first letter and replacing underscores with spaces (e.g. Renewal date).
	- label_suffix: By default, a colon is displayed after the label (e.g. Renewal date:). This argument allows you to specify a different suffix containing other character(s).
	- initial: The initial value for the field when the form is displayed.
	- widget: The display widget to use.
	- help_text (as seen in the example above): Additional text that can be displayed in forms to explain how to use the field.
	- error_messages: A list of error messages for the field. You can override these with your own messages if needed.
	- validators: A list of functions that will be called on the field when it is validated.
	- localize: Enables the localization of form data input (see link for more information).
	- disabled: The field is displayed but its value cannot be edited if this is True. The default is False.
	- - Source from (https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)