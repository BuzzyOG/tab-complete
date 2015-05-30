# jQuery Tab Complete

Tab Completion for jQuery. Tab-complete allows developers to specify a list of options to be auto completed when typing in the binded input. Words can be auto completed from anywhere within the text input, the beginning, middle, or end.

## Installation

You can run:

```bower install tab-complete```

```npm install tab-complete```

or manually copy the tab-complete files to your project.

Installing tab-complete via NPM will install [TrieJS](https://github.com/pthurlow/triejs) as a module for you.

## Usage

Include [TrieJS](https://github.com/pthurlow/triejs) and Tab-Complete

```
<script src="trie.min.js"></script>
<script src="jquery.tab-complete.js"></script>
```

```
$("#example-input").tabComplete({
	getOptions: function() {
		return ["John", "Jake", "Joe", "Sam", "Gil", "Ken", "Garret"]
	}
});
```

The getOptions() function should return an array of options that will be auto-completed.