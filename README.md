- [My org-mode usage](#sec-1)
- [Integrating with macOS / iOS](#sec-2)
- [Enter Apple Shortcuts](#sec-3)
  - [Store your org folder on iCloud](#sec-3-1)
- [Shortcut 'Installation'](#sec-4)


# My org-mode usage<a id="sec-1"></a>

I use [spacemacs](https://www.spacemacs.org) and [org-mode](https://orgmode.org) for pretty much everything I do.

-   I have written a textbook using [org and LaTeX](https://orgmode.org/manual/LaTeX-Export.html)
-   I read and post on [mastodon](https://emacs.ch/@grim) using [mastodon.el](https://github.com/mooseyboots/mastodon.el)
-   I take all of my personal and work notes with org-mode
-   I track all of my personal and work todo lists with org-mode
-   I write blog posts using [ox-hugo](https://ox-hugo.scripter.co)
-   I read my rss feeds using [elfeed](https://github.com/skeeto/elfeed)
-   I code using emacs and [magit](https://github.com/magit/magit)
-   &#x2026; and probably a million other things that don't immediately come to mind

# Integrating with macOS / iOS<a id="sec-2"></a>

The machine I use most is an M1 macbook pro, and my mobile device is an iphone.

It is simple to add a todo or a note using org-mode capture templates, when inside of emacs on the macbook. (`C-c c`).

On the iphone, it is nearly impossible to achieve the workflow I normally use.

I wanted a way to basically use org-capture on the iphone. There are various apps that come so close to solving this problem ([beorg](https://beorg.app), [mobile org](https://mobileorg.github.io), [plain org](https://plainorg.com)), but none of them really had the functionality I was looking for. *(They are all great iOS apps, and do have their use cases)*

# Enter Apple Shortcuts<a id="sec-3"></a>

I created a shortcut using [Apple Shortcuts](https://support.apple.com/guide/shortcuts/welcome/ios) that meets my use case:

-   Accepts quick input for personal todos and notes, and work todos and notes.
-   Functions identically on macOS and iOS

**Here is a link to the shortcut file: [org-capture-shortcut GitHub](https://github.com/samhaingrim/org-capture-shortcut)**

## Store your org folder on iCloud<a id="sec-3-1"></a>

Your org folder must be on your iCloud drive.

`/Users/<your username>/Library/Mobile\ Documents/com~apple~CloudDocs/org`

I symlink mine to my home directory

`ln -s /Users/<your username>/Library/Mobile\ Documents/com~apple~CloudDocs/org /Users/<your username>/org`

# Shortcut 'Installation'<a id="sec-4"></a>

When importing this shortcut, it *should* ask you a few questions as a setup:

-   Folder location for your personal org files *(example: ~/org*)/
-   Folder location for your work org files *(example: ~/org/work*)/
-   Filname (without path) of your personal TODO file *(example: ~/org/todo.org)*
-   Filename (without path) of your work TODO file *(example: ~/org/work/todo.org)*
-   Filename (without path) of your personal notes file *(example: ~/org/notes.org)*
-   Filename (without path) of your work notes file *(example: ~/org/work/notes.org)*

That being said, this shortcut is based on my use-case. If you also need personal and work todos and notes, it should work out of the box for you. You can otherwise edit it to meet your own use-case.

If you find this shortcut useful, I only ask that you link back to me [at this blog](https://blog.samhain.io) or at my [mastodon account](https://emacs.ch/@grim).

Thanks for reading!
