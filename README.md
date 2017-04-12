# Nihilanth
A simple, clean and responsive theme for [Ghost](https://ghost.org/), inspired by [Coding Horror](https://blog.codinghorror.com/).

![showcase](http://i.imgur.com/TIalI3q.png)

## Installation
**1.** Download the theme right here from the "Releases" section (it's always the name with "nihilanth").

**2.** Upload the theme. If you have any questions just check the [Ghost Documentation](http://docs.ghost.org/usage/settings/).

## Sidebar
Here's a guide about how to customize your sidebar:

**1.** Open the `index.hbs` and the `post.hbs` files and look for this:
```html
<aside class="sidebar">
  <div class="box-side" style="width:240px;height:200px;">
    <img src="http://placehold.it/240x200"/>
  </div>
  <div class="box-side" style="width:240px;height:200px;">
    <img src="http://placehold.it/240x200"/>
  </div>
  <div class="res-side">
  <h3>CONTACT ME</h3>
  <ul>
  <li><a target="_blank" href="{{@blog.url}}">Link 1</a></li>
  <li><a target="_blank" href="{{@blog.url}}">Link 2</a></li>
  <li><a target="_blank" href="{{@blog.url}}">Link 3</a></li>
  <li><a target="_blank" href="{{@blog.url}}">Link 4</a></li>
  </ul>
  </div>
```

If you are familiar with HTML and CSS, editing this will be childs play. If you're not, here are some instructions:

**2.** You can change the size of the first two boxes by editing the `width:240px;height:200px;` part. It's pretty obvious that `width` stands for the width of the box, and height... I think you can figure this one out. But *I do NOT recommend* changing their widths, since they were chosen to have the best look on both 1080p and 768p resolutions, but you can set them up to 290px.

**3.** You can change the boxes' content by writing whatever you want on the space between `<div class="box-side" style="width:240px;height:200px;">` and `</div>`. Remember that you will need to edit things like text and image centering by yourself. You should also remember to always respect the box sizes that you've defined.

**4.** For the "Contact Me" section, the customization process is a lot easier. Just look for `<h3>CONTACT ME</h3>` (on `index.hbs` and `post.hbs`) and change whatever you want there. You can change "CONTACT ME" to whatever title you want and and the links to whatever you want too - just change the link on `href="{{@blog.url}}` to `href="your_link_here"` and Link 1, 2 3... to the text you want these links to have.

**5.** Remember to edit BOTH of the files (`index.hbs` and `post.hbs`).

**6.** If you're completely lost, I recommend checking out [some tutorials](http://www.w3schools.com/). You can also contact me (check my GitHub bio).

## How to add Disqus comments

Open the `post.hbs` file, look for `<!--Nihilanth Disqus configuration-->`. Replace the EXAMPLE link with your forum's link, as it says in the comments.

If you have any questions about how to do this, check out [Disqus instructions](https://help.disqus.com/customer/portal/articles/472097-universal-embed-code).

## Changing Syntax Highlighting

Nihilanth features syntax highlighting (yay)! But you might want to change the highlighting style, and doing this is very easy:

Open your `default.hbs` file and look for `{{!Code Highlighting (highlight.js)}}`. Then follow the instructions on the comments and you're done!

## Credits

This theme was heavily inspired by Jeff Atwood's [Coding Horror](https://blog.codinghorror.com/), so thank him for the awesome style! I've also used [this theme](https://github.com/gergelyorosz/GhostSocialCasper) as a "guide" for creating my sidebar. So, I'd like to  thank Jeff Atwood and Gergely Orosz!
