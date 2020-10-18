# K.C.'s custom styles for Joplin

Inspired by [Devon's repo](https://github.com/devonzuegel/joplin-custom-css) I've created my own style for Joplin. It's nothing fancy, but should work with all dark themes.
In the future I might add specific styles for other themes.

I've also added a [`sample.md`](sample.md) markdown file, which I used for testing the css.

## How to install

There are different ways you can install and use the theme, but the most comfortable way is as follows:

- Clone the repository into your Joplin profile directory. If you don't know where it is, go to `Preferences` and it will show you the location.
- Create symlinks to the `.css` files. (Remove or rename your current css files, if they already exist.)
- Create a new branch for your own changes. This will make it easier when new updates are available.

```
cd ~/.config/joplin-desktop
git clone https://github.com/tessus/joplin-custom-css.git
ln -s joplin-custom-css/Dark/userchrome.css
ln -s joplin-custom-css/Dark/userstyle.css
cd joplin-custom-css
git checkout -b my-css
# make changes to the css files and commit them
# when a new update is available, merge or rebase
git fetch origin master:master && git rebase master
```

## Dark

![](images/Dark.png)

## Credits

Many of the CSS snippets were taken from different topics on the [Joplin forum](https://discourse.joplinapp.org/). A few of them I used ad verbatim, others I had to adjust to match my theme, and others served as an inspiration.
