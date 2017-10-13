# List Group

class: ListGroup (implements View)
selector: `n-list-group`

| @Input    | Type                       | Default Value |
| --------- | -------------------------- | ------------- |
| items     | Array<Object>              | `[]`          |
| listTpl   | string \| TemplateRef<any> | null          |
| checkmark | boolean                    | true          |

| @Output | Event            |
| ------- | ---------------- |
| select  | `{item: Object}` |

`listTpl` binds `item` to the template context

`items` expects an array of objects where the objects follow the format:
```javascript
{
	content: "string",
	selected: false,
	disabled: false //optional
}
```