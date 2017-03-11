# \<web-share\>

Wraps the [web share api](https://developers.google.com/web/updates/2016/10/navigator-share) with a fallback to sharing on twitter.

### Usage
Basic usage will look like this:

```
<web-share title="My Title" text="This is my text im sharing" url="https://cool-app.com"></web-share>
```
Then to trigger a share simply apply the share property to the `web-share` element with a value of true.
In plain javascript this would trigger a share `document.querySelector('web-share').share = true;`.

Note: the url attribute is optional, if it is not passed then it will use `window.location.href`.


### Usage in frameworks outside of Polymer 2
Since the element is completely controlled through attributes you can easily use this component
with all the big frameworks. For example in Angular usage would look something like this:

```
<web-share [title]="myTitleVar" [text]="myTextVar" [url]="myUrlVar" [share]="myShareBoolean"></web-share>
```
