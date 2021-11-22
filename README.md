# Basic writing and formatting syntax

Create sophisticated formatting for your prose and code on GitHub with simple syntax.

## Headings

To create a heading, add one to six \# symbols before your heading text. The number of \# you use will determine the size of the heading.

```
# The largest heading
## The second largest heading
###### The smallest heading
```

Rendered H1, H2, and H6 headings

# The largest heading
## The second largest heading
###### The smallest heading


## Styling text

You can indicate emphasis with bold, italic, or strikethrough text in comment fields and .md files.

| Style | Syntax | Keyboard shortcut | Example	Output |
| ----- | ------ | ----------------- | --------------- |
| Bold | \*\* \*\* or \_\_ \_\_ | command/control + b | \*\*This is bold text\*\* | **This is bold text** |
| Italic | \* \* or \_ \_ | command/control + i | \*This text is italicized\* | *This text is italicized* |
| Strikethrough | \~\~ \~\~ |  | \~\~This was mistaken text\~\~ | ~~This was mistaken text~~ |
| Bold and nested italic | \*\* \*\* and \_ \_ |  | \*\*This text is \_extremely\_ important\*\* | **This text is _extremely_ important** |
| All bold and italic | \*\*\* \*\*\* | | \*\*\*All this text is important\*\*\* | ***All this text is important*** |

## Quoting text

You can quote text with a \>.

```
Text that is not a quote

> Text that is a quote
```

Text that is not a quote

> Text that is a quote

## Quoting code

You can call out code or a command within a sentence with single backticks. The text within the backticks will not be formatted. You can also press the command or Ctrl + e keyboard shortcut to insert the backticks for a code block within a line of Markdown.

```Use `git status` to list all new or modified files that haven't yet been committed.```

Rendered inline code block

To format code or text into its own distinct block, use triple backticks.

```
Some basic Git commands are:
\\`\\`\\`
git status
git add
git commit
\\`\\`\\`
```

Rendered code block

Some basic Git commands are:
```
git status
git add
git commit
```

## Links
You can create an inline link by wrapping link text in brackets \[ \], and then wrapping the URL in parentheses \( \). You can also use the keyboard shortcut command + k to create a link. When you have text selected, you can paste a URL from your clipboard to automatically create a link from the selection.

This site was built using \[GitHub Pages\]\(https://pages.github.com/\).

Rendered link [GitHub Pages](https://pages.github.com/).


## Section links

You can link directly to a section in a rendered file by hovering over the section heading to expose the link.


## Relative links

You can define relative links and image paths in your rendered files to help readers navigate to other files in your repository.

A relative link is a link that is relative to the current file. For example, if you have a README file in root of your repository, and you have another file in *docs/CONTRIBUTING.md*, the relative link to *CONTRIBUTING.md* in your *README* might look like this:

```[Contribution guidelines for this project](docs/CONTRIBUTING.md)```

GitHub will automatically transform your relative link or image path based on whatever branch you're currently on, so that the link or path always works. You can use all relative link operands, such as ```./``` and ```../.```

Relative links are easier for users who clone your repository. Absolute links may not work in clones of your repository - we recommend using relative links to refer to other files within your repository.


## Images

You can display an image by adding ! and wrapping the alt text in[ ]. Then wrap the link for the image in parentheses ().

```![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)```

Rendered Image

![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)

GitHub supports embedding images into your issues, pull requests, discussions, comments and .md files. You can display an image from your repository, add a link to an online image, or upload an image. For more information, see "[Uploading assets](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#uploading-assets)."

Tip: When you want to display an image which is in your repository, you should use relative links instead of absolute links.

Here are some examples for using relative links to display an image.

| Context | Relative Link |
| ------- | ------------- |
| In a .md file on the same branch | /assets/images/electrocat.png |
| In a .md file on another branch | /../main/assets/images/electrocat.png |
| In issues, pull requests and comments of the repository | ../blob/main/assets/images/electrocat.png |
| In a .md file in another repository | /../../../../github/docs/blob/main/assets/images/electrocat.png |
| In issues, pull requests and comments of another repository | ../../../github/docs/blob/main/assets/images/electrocat.png?raw=true |

Note: The last two relative links in the table above will work for images in a private repository only if the viewer has at least read access to the private repository which contains these images.

For more information, see "[Relative Links](#relative-links)."


### Specifying the theme an image is shown to

You can specify the theme an image is displayed to by appending #gh-dark-mode-only or #gh-light-mode-only to the end of an image URL, in Markdown.

We distinguish between light and dark color modes, so there are two options available. You can use these options to display images optimized for dark or light backgrounds. This is particularly helpful for transparent PNG images.

| Context | URL |
| ------- | --- |
| Dark Theme | \!\[GitHub Light\]\(https://github.com/github-light.png#gh-dark-mode-only\) |
| Light Theme | \!\[GitHub Dark\]\(https://github.com/github-dark.png#gh-light-mode-only\) |


<!---
tuxnet24/tuxnet24 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
