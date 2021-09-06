<div align="center">

  ![Logo](./images/logo.svg)
  
</div>

# ```(YouForgotBlueberries) => ACII```

For those of us who want to see *You Forgot Blueberries* while in our terminal, but ain't got time to open YouTube.

## Requirements

- Python3
- PortAudio (_Only required for installation with audio support_)
- FFmpeg (_Only required for installation with audio support_)
- Linux or MacOS ... by now

## Installation

Standard installation

```bash
$ pip3 install video-to-ascii
```

With audio support installation

```bash
$ pip3 install video-to-ascii --install-option="--with-audio"
```

## How to use

Just run `video-to-ascii` in your terminal

```bash
$ video-to-ascii -f blueberries.mp4
```

### Options

**`--strategy`**
Allow to choose a strategy to render the output.

**`-o --output`**
Export the rendering output to a bash file to share with someone.

**`-a --with-audio`**
If an installation with audio support was made, you can use this option to play the audio track while rendering the video ascii characters.

## How it works

Every video is composed by a set of frames that are played at a certain frame rate. Since a terminal has a specific number of rows and columns, we have to resize our video to adjust to the terminal size limitations. To reach a correct visualization of an entire frame we need to adjust the _frame height_ to match the _terminal rows_, avoiding using more _characters_ than the number of _terminal columns_. When picking a character to represent a pixel we need to measure the relevance of that pixel's color in the frame, based on that we can then select the most appropriate character based on....


Eh.. who cares.. just sit back and watch the [ASCII](https://en.wikipedia.org/wiki/ASCII).
