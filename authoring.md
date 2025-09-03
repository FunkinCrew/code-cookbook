# Authoring Funkin' CookBook Articles

So you think you're cool enough to write some tutorials? 

Well, that's great! Here is all you need to know about how to write and maintain articles on this CookBook!

## Standards

Basic quality standards are required for each article, and are the exact same as the [base game](https://github.com/FunkinCrew/Funkin/blob/main/docs/CONTRIBUTING.md).

## Naming/File Structure

Files should be stored inside of `assets/content/cookbook/`, in *sub-directories* of the article's top-level difficulty. So something that would be for beginners would be in `assets/content/cookbook/Introduction`, as an example.

The naming convention of those articles should follow Pascal Case and be prepended with the number in that series they represent.

`Introduction/3.CustomCharacters.md` is an example of the correct scheme. With "Introduction" being the *sub-directory*

## Formatting

We use two-space indenting for all the articles (and this file!) with soft wrapping enabled.

To indicate the topic of the article, we format the tags as so, `[tags]: / "beginner,introduction"`; These tags should be at the top of the article before any actual content, should all be lower case, and also be one word.

You should always sign your name at the bottom of the file, after footnote definitions. A correct example looks like this:

```markdown

...

[^philly]: <https://github.com/FunkinCrew/funkin.assets/blob/main/preload/scripts/stages/phillyStreets.hxc>

> Author: [EliteMasterEric](https://github.com/EliteMasterEric)
```

Otherwise, traditional markdown is the standard. This file is an example of such. :^)

## Embedding/Code blocks

We use code blocks very frequently, and they're incredibly useful. To keep them that way for the user, always remember to have your code blocks **syntax highlighted**. The currently supported highlighting styles are: `jsonc` (we use jsonc because it includes support for comments!), `haxe` (use this for .hxc as well), `js`, and `xml`. If you have a file type that isn't supported, please make an issue or find said *TM Bundle* to make a pull request! (Grammars can be found in `grammars/`)

When embedding a file, you must also include a footnote to that file if it is also found on a **FunkinCrew**, *or really any* git repository. You can find a very detailed guide on footnotes (and many other cool markdown features) [here](https://www.markdownguide.org/extended-syntax/#footnotes)

## Tagging

As mentioned above, tagging is basically the only fast way to find articles, and it's how we indicate topics for said articles. Typical tags are the difficulty of the article, the general topic (think: stages, songs, assets, etc), file formats (`.hxc`, `.json`, `.txt`, etc), or misc if you have something that doesn't quite fit into anything else. Always make sure to ask what something might go under, and we can definitely help you figure it out!

If you do choose to put a file format as a tag, make sure to only include up to two formats in the tags!

## Good Practice

Some great practices (that aren't required) can also be done in your article! A couple that the current articles follow include:

- Including lists of properties and a description of each.
- Linking to different articles or helpful pages.
- Using backquotes to signify property names or important code names/values. (ex: `name`, `[1,2,3,4]`)
- If naming a property, classifying if it is read only or not.