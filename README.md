# Shrooms
Shrooms is a simple yet extremely effective piece of UserCSS that breaks web pages to the point of unusability, often creating some truly hilarious results. Originally created to absolutely annihilate the look of Flarum forums, it was found to also have an extremely potent effect on other websites as well, ranging from personal web pages to websites owned by multi-billion dollar corporations.

## How does it work?
Most websites use the `display` rule to manage the layout of their page. Many use a combination of the various options to meet their end goal. This stylesheet hooks into the styling for pretty much *every* element on a web page, changes their display rule to inline or flex (which breaks a huge amount of many pages and even causes some normally hidden elements like scripts or titles to show up), and resizes them with a ridiculous width. This is done entirely by using the following CSS rule:
```css
* {
    display: inline;
    text-shadow: 0 0 5px lime;
    color: black;
    font-family: Impact;
    width: 100%;
}
```

For an extra kick in some places, there are also some CSS rules that hook into additional elements if present to mess with their display rule as well on top of the changes noted above.

```css
header, #content * {
    display: flex;
}

#app {
    display: content;
}
```

## Screenshots
| Website/Service             | Screenshot                                   |
|-----------------------------|----------------------------------------------|
| Flarum                      | ![](/images/flarum-screenshot.png?raw=true)  |
| Stylus' built-in CSS editor | ![](/images/stylus-screenshot.png?raw=true)  |
| Twitter                     | ![](/images/twitter-screenshot.png?raw=true) |
| TikTok                      | ![](/images/tiktok-screenshot.png?raw=true)  |

## License
Shrooms is licensed under the GPLv3 License.
