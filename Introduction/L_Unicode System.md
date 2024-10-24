# Unicode System

Unicode is a universal international standard character encoding that is capable of representing most of the world's written languages.

## Why Java Uses Unicode System?

Before Unicode, there were many language standards:
- **ASCII** (American Standard Code for Information Interchange) for the United States.
- **ISO 8859-1** for Western European languages.
- **KOI-8** for Russian.
- **GB18030** and **BIG-5** for Chinese, and so on.

## Problems

This caused two problems:
1. A particular code value corresponds to different letters in the various language standards.
2. The encodings for languages with large character sets have variable lengths. Some common characters are encoded as single bytes, while others require two or more bytes.

## Solution

To solve these problems, a new language standard was developed: **Unicode System**. In Unicode, each character holds 2 bytes, so Java also uses 2 bytes for characters.
- **Lowest value:** `\u0000`
- **Highest value:** `\uFFFF`
