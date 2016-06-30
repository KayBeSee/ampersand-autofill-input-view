# Ampersand Autofill Input View
Cause copying and pasting _id sucks.

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
var Chapters = require('ampersand-rest-collection');

new AutoCompleteView({
                label: 'Chapter',
                name: 'chapter',
                collection: new Chapters(),
                queryKey: 'school_name',
                idAttribute: '_id',
                textAttribute: '_id',
                placeHolder: 'Type Chapter Name',
                minKeywordLength: 3,
                maxResults: 10,
                value: this.model && this.model.chapter || this.model.chapter._id,
                type: 'text',
                parent: this
            }),
```

[Kevin Mulcrone]: <http://KayBeSee.com>
