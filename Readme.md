# StateRestore for DataTables with Bootstrap 5 styling

StateRestore is a state management UI for DataTables. It allows users to create multiple table states which can be saved and then reloaded at any time. This is particularly useful for complex tables where specific views are common and the user might wish to toggle between states.

States can be saved locally, or for a more permanent part of your table's features, to a remote database via Ajax, which also provides the ability for users to share states.

For full information about StateRestore including its features and configuration option, please [refer to the DataTables manual](https://datatables.net/manual/extensions/staterestore/).



## Installation

The easiest way to install any extension for for DataTables, including StateRestore, is with the [download builder](https://datatables.net/download). With the download builder, you select the styling and aspects of DataTables suite that you want, and it will generate the packages / install commands for you to use.

The download builder includes options for direct loading with `script` and `link` tags, details for using a package manager such as [npm](https://www.npmjs.com/) and [NuGet](https://www.nuget.org/), or a download option if you wish to have the files locally.


### NPM

Installation from NPM can be done with the `datatables.net-staterestore-bs5` package:

```
npm install \
    datatables.net-bs5 \
    datatables.net-buttons-bs5 \
    datatables.net-staterestore-bs5
```


## Basic Usage

In its most simple case, you can enable StateRestore by simply setting `stateRestore: true` as an option in the DataTables initialisation.

```js
import DataTable from 'datatables.net-bs5';
import 'datatables.net-buttons-bs5'
import 'datatables.net-staterestore-bs5'

// Register DataTables Plus license key
DataTable.key('plus_....');

// Initialisation
new DataTable('#myTable', {
	layout: {
		topStart: {
			buttons: ['stateCreate', 'statesList', 'pageLength']
		}
	},
	stateRestore: true
});
```


## Documentation / Support

* Full installation, usage and documentation is [in the manual](https://datatables.net/extensions/staterestore/)
* [DataTables support forums](http://datatables.net/forums)


## License

This software is released under the [DataTables Plus License](https://datatables.net/license/plus). To use the software a license key must be applied - see [DataTables Plus](https://datatables.net/plus).
