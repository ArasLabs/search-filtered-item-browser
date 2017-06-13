# Searchable Filtered Item Browser

When the Filtered item Browser is used to generate an idlist of values you may select from, it may be necessary to use standard searching functionality to narrow that list even further.

The method code in this example will allow you do perform a search on a filtered item browser that returns all members of the Administrator group. This example will allow you to search further on the return of members.

## History

This project and the following release notes have been migrated from the old Aras Projects page.

Release | Notes
--------|--------
[v1](https://github.com/ArasLabs/search-filtered-item-browser/releases/tag/v1) | Initial Release

#### Supported Aras Versions

Project | Aras
--------|------
[v1](https://github.com/ArasLabs/search-filtered-item-browser/releases/tag/v1) | 9.2.0 SP3

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed
2. Aras Package Import tool
3. **ProductLineBasedWorkflow** import package

### Install Steps

Use the following steps to create a client-side (JavaScript) method that will be called from
onSearchDialog for a property of type Item.

1. Log into Aras Innovator as an Administrator
2. From the TOC select **Administration > Methods** and create a new Client-Side,
JavaScript method
    - Name=SearchableFIB
    - Copy the method code from [the appendix](./Documentation/Searchable%20Filtered%20Item%20Browser.pdf).
3. Save, Unlock and close SearchableFIB
4. From the TOC select **Administration > ItemTypes** and open your ItemType for edit
    - Find your property of type Item and right click and select view
    - Lock the property
    - Add a new Event
        - Select TestFIB
        - Set event to onSearchDialog
    - Save, Unlock and Close your property
5. Save, Unlock and Close your ItemType

Once the event has been added onSearchDialog, next time you bring up the dialog, you will
now have a searchable filtered item browser that returns all identities within the
Administrators group.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## Credits

Created by Aras Corporation Support.

## License

Published to Github under the MIT license. See the [LICENSE file](./LICENSE.md) for license rights and limitations.
