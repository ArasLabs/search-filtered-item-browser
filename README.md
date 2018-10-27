# Searchable Filtered Item Browser

It is possible to add filters to a search dialog for an Item property, to limit the results available for users to select from. This project contains both a document originally written for 9.2.0 SP3 as well as sample code that was written for 11.0 SP12.

The method code included in the example imports demonstrate how to perform a search to retrieve all of the Admin Identities that have a corresponding user.

## History

This project and the following release notes have been migrated from the old Aras Projects page.

Release | Notes
--------|--------
[v1](https://github.com/ArasLabs/search-filtered-item-browser/releases/tag/v1) | Initial Release
[v2](https://github.com/ArasLabs/search-filtered-item-browser/releases/tag/v2) | Importable Examples

#### Supported Aras Versions

Project | Aras
--------|------
[v1](https://github.com/ArasLabs/search-filtered-item-browser/releases/tag/v1) | 9.2.0 SP3
[v2](https://github.com/ArasLabs/search-filtered-item-browser/releases/tag/v2) | 11.0 SP12

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed
2. Aras Package Import tool
3. **Search Filter Examples** import package

### Install Steps

#### Database Installation
1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
  * _Note: You must login as root for the package import to succeed!_
4. Enter the package name in the TargetRelease field.
  * Optional: Enter a description in the Description field.
5. Enter the path to your local `..\RefreshFromDatabase\Import\imports.mf` file in the Manifest File field.
6. Select **aras.labs.RefreshFromDatabase** in the Available for Import field.
7. Select Type = **Merge** and Mode = **Thorough Mode**.
8. Click **Import** in the top left corner.
9. Close the Aras Package Import tool.

You are now ready to try out the Search Filter example.

### Usage
1. Login as admin
2. Navigate to the new Search Filter Example ItemType in the TOC
3. Create a new Search Filter Example
4. There are 3 different Item Properties here that show three different ways to Filter a SearchDialog
5. For more details, you can check the methods Events tab on the corresponding Property items

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## Credits

Created by Aras Corporation Support.

Updated by Christopher Gillis for Aras Labs. [@cgillis-aras](https://github.com/cgillis-aras)

## License

Published to Github under the MIT license. See the [LICENSE file](./LICENSE.md) for license rights and limitations.
