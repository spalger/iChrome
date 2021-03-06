# iChrome

iChrome is a highly customizable, iGoogle homepage replacement extension influenced by Google Now. It includes almost 100 HD themes, over 30 widgets, support for multiple tabs, "OK Google" hotword detection and voice search and almost complete customization.

This is the full source for iChrome except for API secrets which have been replaced with empty strings (`""`).

The code's somewhat messy, but I'm currently in the middle of a restructure in the [restructure](https://github.com/AMKohn/iChrome/tree/restructure) branch.  I'm also looking to add internationalization in V2.1.2, so if you'd like to translate it to a specific language please let me know.

## Roadmap

#### V2.1.4 - WIP
 - Code cleanup and restructure using Backbone, Require and Lo-Dash.

#### V2.1.5
 - Internationalization with support for (at least): Russian, German, Dutch, Ukrainian, French, Spanish, Chinese and Portuguese
 - Various small widget features

#### V2.x
 - A real website

### V2.2
These are very much in flux, any of them could be postponed or skipped.
 - A widgets store that other developers can contribute to, possibly it isn't quite the main focus of the release
 - iChrome Pro:
   - Shareable tabs
   - Prioritized support and suggestions
   - The ability to create up to 50, synced, custom, dynamic themes (video, slideshows, time and date dependent) that are hosted on iChrome servers
   - The ability to group and disconnect synced computers
   - The ability to configure a backup schedule
   - Up to 50 online backups per computer
   - A dashboard to manage (copy, remove from account, disconnect, reset, restore from any - including another computers - backup and group) a computers configuration
   - The ability to permanently save up to 50 configurations or backups separately from the 50 per computer
   - "Parental" controls with the ability to blacklist widgets and lock configurations remotely
   - More, I'm still thinking it through

## Contributing

If you'd like to contribute, please fork the repo and submit a pull request.

## Style Guide
I follow a more complicated style guide, but here's the basic overview:

 - Code is indented with 4 space tabs, never spaces
 - Double quotes are always used unless the string is HTML
 - Trailing semicolons are always used
 - When multiple variables are being defined at the top of a function they should generally be combined into one `var` statement
 - Ternary operators are fine especially for string concatenation
 - Performance should always be favored over readability for small snippets. i.e. `$(body).append($('<div></div>').attr("data-id", id.split("-")[1]))` instead of `var elm = $('<div></div>'), id = id.split("-")[1]; elm.attr("data-id", id)....`

## License

iChrome is licensed under a [Creative Commons Attribution-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-sa/3.0/deed.en_US).

Basically, feel free to use the code however you want as long as you give credit. And, if you don't mind please let me know.
