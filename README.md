# Lyrist

Lyrist displays the lyrics of the currently-playing iTunes track (using [LyricWiki][]) on the command line in OS X.

![Screenshot of Lyrist in action][screenshot]

I have the terminal always running and just a keystroke away (thanks to [TotalTerminal][]), which makes Lyrist *very* convenient for me; your mileage may vary.

## Installation

1. [Download the latest version][download] and unzip it.
2. Intall [Node][] if you don't have it on your system. You can install it from the [Node website][Node] or alternatively, if you have [Homebrew][], by running `brew install node`.
3. Open Terminal and navigate to the folder where you unzipped Lyrist's source files.
4. Run `make` (this compiles the AppleScript).

To easily run the script from anywhere, you can add an alias to it in your bash profile (located at `~/.bash_profile`; you can create it if it doesn't exist) like so:

	alias lyrist="/PATH/TO/lyrist/lyrist.js"
	
I like to run `lyrist`'s output through `less` so that I can easily scroll through it:

	alias lyrist="/PATH/TO/lyrist/lyrist.js | less -XRq"

## Usage

Using Lyrist is simple. When a song is playing (or paused) in iTunes, go to the terminal and type the name of the alias you just created above (`lyrist` in this case). Press `enter`. *Et voilà!*

Note: If you didn't create an alias, navigate to the folder where you unzipped Lyrist and run `./lyrist.js`.

## Issues and Feedback

I'd love any feedback you have. Use the [Issues][] tab for questions, bugs, and suggestions.

[LyricWiki]: http://lyrics.wikia.com/Lyrics_Wiki
[TotalTerminal]: http://totalterminal.binaryage.com/
[download]: https://github.com/spinningarrow/lyrist/zipball/master
[Node]: http://nodejs.org/
[Homebrew]: http://mxcl.github.com/homebrew/
[Issues]: https://github.com/spinningarrow/lyrist/issues

[screenshot]: https://lh6.googleusercontent.com/-15X1ZgVxCDQ/UTIj_nnBF8I/AAAAAAAAAeE/YWG4Zka_OXo/s537/lyrist.png