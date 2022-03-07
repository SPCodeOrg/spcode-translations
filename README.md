# SPCode Translation Files

In this repository you will find the translation files that SPCode will automatically download and use.

## How can I suggest a modification?

To suggest a change in any of the files, fork the repo, make your changes and make a pull request. If everything seems fine, your changes get merged and SPCode will reflect your changes in no time.

## How can I add a language that is not in SPCode?

Same as before. Fork the repo, clone the `default.xml` translation file, and begin translating. Once you're done, pick a 2-3 letter language code for your new file and submit the pull request.

## What if my language is written from right to left (RTL)?

Simply, below the first node called `<language>`, add a node called `<rtl>` and set its inner text to `true`, like this:
```xml
<rtl>true</rtl>
```

## Translation tips and guidelines

- You must not change the structure of the XML file, including the name of ___any___ node (text between `<>`) UNLESS you're updating a node name to match the one from `default.xml`.
- Although the order in which you add new nodes ___does NOT matter___, try to maintain the order of the nodes in the default file.
- To know which nodes to add, you can:
  - Search for the phrase you see in English when you switch to your language in the default file
  - Use a tool like [DiffChecker](https://www.diffchecker.com/) to compare your language file with the default file to see which nodes are missing
- You can test your language in the editor before you send the PR! Just place the file inside the `translations` folder in your SPCode installation directory and restart the editor. After that, you will see your language in the languages box in Options.
