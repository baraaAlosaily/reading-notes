# Audio, Video, Images

The HTML `<audio>` element is used to play an audio file on a web page.

Example

```
<!DOCTYPE html>
<html>
<body>

<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>

</body>
</html>
```

It will be like this
![audio1](./img./audio1.png)

### HTML Audio - How It Works

The `controls` attribute adds audio controls, like play, pause, and volume.

The `<source>` element allows you to specify alternative audio files which the browser may choose from. The browser will use the first recognized format.

The text between the `<audio>` and `</audio>` tags will only be displayed in browsers that do not support the `<audio>` element.

HTML `<audio`> Autoplay
To start an audio file automatically, use the autoplay attribute:

```
<audio controls autoplay>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>

</body>
</html>
```

Add muted after autoplay to let your audio file start playing automatically (but muted):

```
<!DOCTYPE html>
<html>
<body>

<audio controls autoplay muted>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>

</body>
</html>
```

### HTML Audio - Methods, Properties, and Events

The HTML DOM defines methods, properties, and events for the <audio> element.

This allows you to load, play, and pause audios, as well as set duration and volume.

There are also DOM events that can notify you when an audio begins to play, is paused, etc.

| Tag        | Description                                                                          |
| ---------- | ------------------------------------------------------------------------------------ |
| `<audio>`  | Defines sound content                                                                |
| `<source>` | Defines multiple media resources for media elements, such as `<video>` and `<audio>` |

HTML Video

The HTML `<video>` element is used to show a video on a web page.

Example

```
<!DOCTYPE html>
<html>
<body>

<video width="400" controls>
  <source src="mov_bbb.mp4" type="video/mp4">
  <source src="mov_bbb.ogg" type="video/ogg">
  Your browser does not support HTML video.
</video>

<p>
Video courtesy of
<a href="https://www.bigbuckbunny.org/" target="_blank">Big Buck Bunny</a>.
</p>

</body>
</html>
```

It will be like this

![video](./img/video.png)

### How it Works

The controls attribute adds video controls, like play, pause, and volume.

It is a good idea to always include width and height attributes. If height and width are not set, the page might flicker while the video loads.

The `<source>` element allows you to specify alternative video files which the browser may choose from. The browser will use the first recognized format.

The text between the `<video>` and `</video>` tags will only be displayed in browsers that do not support the `<video>` element.

### HTML Video - Methods, Properties, and Events

The HTML DOM defines methods, properties, and events for the `<video>` element.

This allows you to load, play, and pause videos, as well as setting duration and volume.

There are also DOM events that can notify you when a video begins to play, is paused, etc.

### HTML Video - Media Types

| File Format | Media Type |
| ----------- | ---------- |
| `MP4`       | video/mp4  |
| `WebM`      | video/webm |
| `Ogg`       | video/ogg  |

### HTML `<img>` Tag

Example

```
<!DOCTYPE html>
<html>
<body>

<h1>The img element</h1>

<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">

</body>
</html>
```

Definition and Usage

The `<img>` tag is used to embed an image in an HTML page.

Images are not technically inserted into a web page; images are linked to web pages. The `<img>` tag creates a holding space for the referenced image.

The `<img>` tag has two required attributes:

src - Specifies the path to the image
alt - Specifies an alternate text for the image, if the image for some reason cannot be displayed
Note: Also, always specify the width and height of an image. If width and height are not specified, the page might flicker while the image loads.

### Summary

- You can specify the dimensions of images using CSS.
- This is very helpful when you use the same sized images on several pages of your site.
- Images can be aligned both horizontally and vertically using CSS.
- You can use a background image behind the box created by any element on a page.
- Background images can appear just once or be repeated across the background of the box.
- You can create image rollover effects by moving the background position of an image.
- To reduce the number of images your browser has to load, you can create image sprites.
