# Ampersand Autofill Input View

### Cause copying and pasting _id sucks.

'
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
'

Update later.

[Kevin Mulcrone]: <http://KayBeSee.com>
