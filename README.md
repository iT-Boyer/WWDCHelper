<p align="center">
<img src="logo.png" alt="WWDCHelper Logo" title="WWDCHelper Logo" width="450">
</p>

<p align="center">
<a href="https://travis-ci.org/kingcos/Learning-WWDC"><img src="https://www.travis-ci.org/kingcos/Learning-WWDC.svg?branch=master"></a>
<a href="https://codecov.io/gh/kingcos/Learning-WWDC"><img src="https://codecov.io/gh/kingcos/Learning-WWDC/branch/master/graph/badge.svg"></a>
<img src="https://img.shields.io/badge/Swift-3.1-orange.svg">
<img src="https://img.shields.io/badge/Platform-macOS-red.svg">
<img src="https://img.shields.io/badge/License-MIT-blue.svg">
</p>

[中文版 README](README_CN.md)

> Inspired by qiaoxueshi/WWDC_2015_Video_Subtitle, ohoachuck/wwdc-downloader, and @onevcat's videos. Thanks for their inspiration and efforts. 👏

## Info

WWDCHelper is a command line tool on macOS for you to get WWDC info easily. Now you can get download links of SD/HD video & PDF, and download subtitles in English or **Simplified Chinese** directly by it.

You can also download subtitles at the [releases](https://github.com/kingcos/WWDCHelper/releases) page only.

> **Notice:**
> 
> Although I have written in Swift for years, I still have a lot to learn about Swift. And to be honest, CLI (Command Line Interface) is not familiar for me. So this program is not perfect, even a little wired. So you can issue me if you have any questions, advices or find some bugs . I will be very appreciated for your help. ❤️

## How

### Install

You should have [Swift Package Manager](https://swift.org/package-manager/) installed or latest Xcode installed with command line tools in your macOS.

```sh
> git clone https://github.com/kingcos/WWDCHelper.git
> cd WWDCHelper
> ./install.sh
```

### Run

```sh
> wwdchelper -h
Usage: WWDCHelper [options]
  -y, --year:
      Setup the year of WWDC. Only support 2017 now. Default is WWDC 2017.
  -s, --sessions:
      Setup session numbers in WWDC.
  -l, --language:
      Setup the language of subtitle. Only support Chinese or English now. Default is Chinese.
  --sd:
      Setup default subtitle filename of SD video.
  --hd:
      Setup default subtitle filename of HD video.
  -p, --path:
      Setup where download the subtitle to. Default is the Download folder.
  -h, --help:
      Print this help info.
  -v, --version:
      Print version info.
```

### Demo

- If you want just Session 102 & 202 info of WWDC 2017:

```sh
> wwdchelper -s 102 202
or
> wwdchelper -y 17 -s 102 202
```

### NOT Implemented

> Maybe implement these features in the future.

- [x] Download multiple subtitles at once
- [ ] Support subtitles in Traditional Chinese
- [ ] Support subtitles in both English & Chinese
- [ ] Support WWDC before 2017
- [ ] Support for Linux 🐧

### Reference

- [qiaoxueshi/WWDC_2015_Video_Subtitle](https://github.com/qiaoxueshi/WWDC_2015_Video_Subtitle)
- [ohoachuck/wwdc-downloader](https://github.com/ohoachuck/wwdc-downloader)
- [onevcat/FengNiao](https://github.com/onevcat/FengNiao)

## WWDC 17 - Notes

- [102 - Platforms State of the Union](/2017/102)

### Design

- [819 - Designing for a Global Audience](/2017/819)
- [822 - App Icon Design](/2017/822)
- [823 - Designing Glyphs](/2017/823)

## LICENSE

MIT