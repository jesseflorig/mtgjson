# mtgjsonx

Fetches AllSets-x.json from http://mtgjson.com and caches it so you are always sure to have the newest version.

Includes `AllSets-x.json` to make loading time faster. This module follows the versioning of mtgjson.com.

In addition to the AllSets.json file, the extras includes:

 - Card rulings
 - Foreign names
 - Printings
 - Original text
 - Original type
 - Legalities
 - Source (promos, box sets and theme decks)

Notes
 - the JSON data is collected by @lsmoura, https://github.com/lsmoura/mtgjson.
 - this package is forked from the mtgjson npm package by @freeall, https://github.com/freeall/mtgjson.

## Installation

`npm install mtgjsonx`

## Usage

``` js
var mtgjsonx = require('mtgjsonx');

mtgjsonx(function(err, data) {
	if (err) return console.log(err);

	console.log(data.LEA.cards); // Prints out all cards from the Limited Edition Alpha (LEA) set
});
```

## License
MIT
