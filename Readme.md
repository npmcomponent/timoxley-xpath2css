*This repository is a mirror of the [component](http://component.io) module [timoxley/xpath2css](http://github.com/timoxley/xpath2css). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/timoxley-xpath2css`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# xpath2css

  Convert simple xpath to css selector.

## Installation

```
$ component install xpath2css
```

## Example 
```js
  var xpath2css = require('xpath2css')
  xpath2css('//a[@id="bleh"]') // => a#bleh
  xpath2css('//ul/li') // => ul > li 
  xpath2css('//div[@class="comment"]') // => div.comment
  xpath2css('//ul/li[3]') // => ul > li:nth-of-type(3)
  xpath2css('//body//div[@data-binding="currentTime"]') // => body div[data-binding=currentTime]
  xpath2css('//div[@id="shoe"][2]/span[@class="body"]//a[contains(@class, "leather")]//img[1]') 
  // => div#shoe:nth-of-type(2) > span.body a[class*=leather] img:first-of-type
```

## Credits

JS code adapted as a component from https://gist.github.com/3320053
Ported by Dither from [cssify](https://github.com/santiycr/cssify)


