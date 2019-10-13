# Newsletter

## Web

* Write it as markdown
* Convert it to HTML and copy to clipboard

  ```console
  $ cd 2019-03
  $ pandoc website.markdown --to html --standalone --table-of-contents | xmllint --format --html --xpath '//html/body/node()' - | pbcopy
  ```

*  Grab the contents of the `body` section and paste it into a Wordpress HTML block

## Mail

* Write it as shortened version of the web, also as markdown
* Convert it to plain text:

  ```console
  $ cd 2019-03
  $ pandoc email.markdown --to plain --wrap=none | pbcopy
  ```
* Paste it into an eMail.
