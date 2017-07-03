# Angular 4+

The library can be imported directly from TS code with:

```typescript
import * as XLSX from 'xlsx';
```

This demo uses an array of arrays as the core data structure.  The component
template includes a file input element, a table that updates based on the data,
and a button to export the data.

OR it can generate worksheet From Table Data,Threse way may use less code,
but it limited by table data,like image,button,it will not able to export.

## Switching between Angular versions
Please See SheetJS Site

## SystemJS Configuration

The default angular-cli configuration requires no additional configuration.

Some deployments use the SystemJS loader, which does require configuration.  The
SystemJS example shows the required meta and map settings:

```js
SystemJS.config({
	meta: {
		'xlsx': {
			exports: 'XLSX' // <-- tell SystemJS to expose the XLSX variable
		}
	},
	map: {
		'xlsx': 'xlsx.full.min.js', // <-- make sure xlsx.full.min.js is in same dir
		'fs': '',     // <--|
		'crypto': '', // <--| suppress native node modules
		'stream': ''  // <--|
	}
});
```
