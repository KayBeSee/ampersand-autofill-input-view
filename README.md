# Ampersand Autofill Input View
Cause copying and pasting _id sucks.

This module is ment to be used in conjunction with [ampersand form view] <https://github.com/AmpersandJS/ampersand-form-view>.

## Installation
`git clone https://github.com/KayBeSee/ampersand-autofill-input-view.git`


## Parameters
**label**: Label that will appear in form  
**name**: name of input field  
**collection**: the collection to query from  
**queryKey**: the property to query within the collection's models  
**idAttribute**: id attribute of model within the collection  
**textAttribute**: property that will appear in dropdown  
**placeholder**: placeholder for field  
**minKeywordLength**: amount of characters that must be present before querying collection  
**maxResults**: maximum number of results to display in dropdown menu when querying  
**value**: corresponding value for form model  
**type**: type of field  
**parent**: parent

## Example Usage
```
var Books = require('ampersand-rest-collection');

new AutoCompleteView({
    label: 'Books',
    name: 'book',
    collection: new Bookss(),
    queryKey: 'book_name',
    idAttribute: '_id',
    textAttribute: '_id',
    placeHolder: 'Type Books Name',
    minKeywordLength: 3,
    maxResults: 10,
    value: this.model && this.model.book || this.model.book._id,
    type: 'text',
    parent: this
}),
```

[Kevin Mulcrone]: <http://KayBeSee.com>
