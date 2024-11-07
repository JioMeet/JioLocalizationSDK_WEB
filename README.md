<h1 align="center" style="border-bottom: none">
    <b>
        <a href="https://localization-platform.sit.translate.jio">Jiotranslate for Web</a><br>
    </b>
    The Jiotranslate i18n SDK for Web
    <br>
</h1>

# What is Jiotranslate for Web?

Web integration library of Jiotranslate. This package makes it super simple to add i18n to your Web app!

## Installation

```
npm install @jiotranslate/web-beta
```

Then use the library in your app:

## Usage

First, create a Jiotranslate instance and run it.

```ts
import { JioTranslate, DevTools, FormatSimple } from "@jiotranslate/web-beta";

const jt = JioTranslate().use(DevTools()).use(FormatSimple()).init({
  apiKey: "your_api_key",
  apiUrl: "https://localization-platform.sit.translate.jio/",
});

jt.run();
```

Then, use it to translate your strings.

```ts
jt.onLangLoaded.subscribe(() => {
  document.title = tg.translate("hello_world");
});
```

## Why use Jiotranslate?

It saves you a significant amount of time on localization tasks. It also ensures your software is perfectly translated.

### Features

- Comprehensive localization solution tailored for your JavaScript application 🙌
- Seamless in-context localization right from the start 🎉

- Translation management system 🎈
