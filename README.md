# Retro-Shadow-Buttons

## _Fun little library to get those text-based retro game styled buttons on your website_

## Installation

A good idea would be to simply clone this git repo and pick up the CSS file. Working on a direct npm install as well!
```shell
git clone https://github.com/SockAndSandal/Retro-Shadow-Buttons.git
```


## Getting started

To get started, simply make a `div` using the  `retro` class name and enter some text inside. This will create a button that can support say, a sentence of text. The class uses Roboto Mono as a default, with a font size of 20, but you can couple the button class with a header or paragraph class to match your choices in type.

 ```html
<div class = "retro">
  Hello! This is a button!
 </div>
```


## Using the Buttons

This library was made with [my website](www.amanbeer.com) kept in mind, which was based on the concept of a text-based choice-based game in mind. Thus, most buttons are made keeping a large amount of text in mind. The button assumes no particular width and will probably stretch to the entire width, thus you'd have to control it using a wrapper container or a column. (I used Bootstrap to sort that out for me) 

Let me break down the 3 classes that are relevant to this little set of buttons I have created. They're really tuned to work well with a black background, but some inline CSS can change that. You're also free to edit the CSS for the buttons as you like, it's lucid enough for understanding.

### Small Buttons

The `.rbtn-small` class can be used where you just want to make a small button for something like 'Listen on Spotify!' and don't want the extra padding on the right. You'd want to use both `retro` and `rbtn-small` for the desired effect.

 ```html
<div class = "retro rbtn-small">
  Listen on Spotify!
 </div>
```

![Small Button](https://raw.githubusercontent.com/SockAndSandal/Retro-Shadow-Buttons/main/images/small%20button.png)

### Big Buttons

The `rbtn-big` class comes in handy when you're trying to nest a bunch of different kinds of text in a single button. Where would that be useful? As a design language, that could come in handy to make each header or title of your blog an entire big button, with a preview and everything of the sort. You'd want to use both `retro` and `rbtn-small` for the desired effect.

```html
<div class="retro rbtn-big">                        
      <h3 style="color: black;"><strong>{{ entry.title }}</strong></h3>
      <h5 style="color: black;">{{entry.preview}}</h5>
</div>
```

![Big Button](https://raw.githubusercontent.com/SockAndSandal/Retro-Shadow-Buttons/main/images/big%20button.png)

### Images

The `retro-img` class is used if you want to take an image (or a GIF for that matter) and make a button out of that.

```html
<div class="retro-img">                        
  <img src="linktoimage">
</div>
```

![Image Button](https://raw.githubusercontent.com/SockAndSandal/Retro-Shadow-Buttons/main/images/image%20buttons.png)


## Accessibility

Retro-Shadow-Buttons supports the [`prefers-reduced-motion` media query](https://webkit.org/blog/7551/responsive-design-for-motion/) so that users with motion sensitivity can opt out of animations. On supported platforms (currently all the majors browsers and OS), users can select "reduce motion" on their operating system preferences and it will turn off CSS transitions for them without any further work required.

## Contributing

Pull requests are the way to go here. I really only have two rules for submitting a pull request: match the naming convention (camelCase, categorised [fades, bounces, etc]) and show a demo of submitted animations in a [pen](https://codepen.io). That **last one is important**.
