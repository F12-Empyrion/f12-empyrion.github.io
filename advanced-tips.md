# Advanced Tips

## Colorization of device names

You can add colors and some formatting to your device names.

This is done using what looks like a variant of [bbcode](https://en.wikipedia.org/wiki/BBCode).

Here are the codes I've found to be working so far, please [inform me](mailto:lasse@vkarlsen.no) if you know of or find more.

Some general advice first:

* You don't have to specify the closing code/tag if you want the rest of the name to have the formatting
* Formatting is counted towards the maximum length of the name, so any formatting you add will give you fewer available characters for the name itself

* Bold: `[b]Bold Text[/b]`
* Italic: `[i]Italic Text[/b]`
* Underline: `[u]Underlined text[/b]`
* Strikethrough: `[s]Strikethrough[/s]`
* Color: `[rrggbb]Color` (not sure about the closing tag here.) You can use any html-color here, and [here](https://htmlcolorcodes.com/) is a helpful webpage. You want the code after HEX on that page, just leave out the `#` sign. Example: `[ff0000]Red [00ff00]Blue [0000ff]Green`.
