# Angular Localization Helper

Visual Studio Code extension to help maintaining angular i18n localization files

## Features

* Merge @angular-cli generated file into existing localization file.
* Search and highlight missing translations.
* Currently support Xliff 1.2
* Upcoming support for Xliff 2.0 and Xmb files
* Macbook Pro Touchbar support.

## Installation

Install through VS Code extensions: search for `Angular Localization Helper`

Install through terminal: `ext install angular-localization-helper`

## Usage

Generate/Update the base localization using the angular-cli, then use the extension to merge the changes into existing file.

### Using the Command Palette

> 1.  CMD + Shift + P to open the command palette
> 2.  i18n Sync

By default, the extension expects the base file to be named `messages.xlf`. If no corresponding file is found, you are prompted to identify the base file. This setting will be saved for future use. If the extension is invoked from a localization file, that file will be updated, otherwise the extension will prompt you for the file to update. You can also create a new file.

On Macbook Pros the extension's commands appear on the touchbar.

## Extension Settings

### i18nSync.baseFile (default: messages.xlf)

Identifies the base localization file generated by the `@angular-cli`. If file does not exist, you are prompted to identify the file and the setting is saved.

### i18nSync.fileType (default: xlf)

Identify the type of localization to process (xlf or xmb)

### i18nSync.missingTranslation (default: !MISSING_TRANSLATION!)

Target tag text for missing translation

### i18nSync.decoration (default: dark red on yellow with white border)

Missing translation highlight decoration

## Known Issues

* Xlf 2.0 and Xmb format are not yet implemented
* Incorrect highlight on find next missing translation
* List missing translations are not yet implemented

## Release Notes

### 1.0.0

Initial release. Synchronize Xlf 1.2 files

---

**Enjoy!**
