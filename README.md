# jQuery HabboAPI

jQuery Habbo Hotel API Plugin.

  - Only 2kB minified.
  - Chrome, Edge, Firefox, IE, Safari, Android, iOS, and more.
  - Support all Habbo Hotel API.

You can also:
  - Export Habbo Hotel Data.
  - Avoid connection problems with the server.
  - Quick and light response in JSON format.

For more technical information, I published an official guide to the Habbo API on [Habboemotion](http://habboemotion.com/guide/habboapi).

### Installation

HabboAPI jQuery Plugin requires [jQuery](https://jquery.com/) to run.

Copy the files to the directory and add the plugin after the jQuery library.

```sh
<script type="text/javascript" src="HabboAPI.min.js"></script>
```
### How to use

Specify the following parameters:
```sh
  // Specify the API
	$.HabboAPI('users', {
		user: 'Sefos', // Habbo username
		hotel: 'es' // Habbo Hotel
	});
```
The API method:

**users:** Basic information on Habbo account.

**profile:** Habbo Account Information Extended.

**badges:** Show badges of Habbo Account

**rooms:** Show rooms of Habbo Account

**friends:** Show friends of Habbo Account.

**groups:** Show groups of Habbo Account.

### Example:

```sh
$(document).ready(function(){
	$.HabboAPI('users', {
		user: 'Sefos', 	// Habbo username
		hotel: 'es' 	// Habbo Hotel
	}, function(response){
		if(response.success){
			// Show data response...
			console.log(response.data);
		}
		if(response.error){
			// Show error...
			console.log(response.text);
		}
	});
});
```

### Author

HabboAPI jQuery Plugin is developed by **[Joaquin A.](https://twitter.com/DevJoaquin)**

### Contact:
**Website:** [http://devjoaquin.com.ve/](http://devjoaquin.com.ve/)

**Twitter:** [@DevJoaquin](https://twitter.com/DevJoaquin)

**Email:** devjoaquin@gmail.com
