# Pseudol10n
Pseudolocalization or Pseudol10n (there are 10 `chars` between l-ocalizatio-n, hence `l10n`) is a method to test the internationalization of text while maintaining readability. The purpose of this testing is to expose issues regarding length and flow of text, layout issues and logic issues.

If you are getting translations done externally it can be a time consuming and expensive process so localization testing should take place long before you get any kind of translator involved. By verifying everything is correct you will save time and iterations back and forth with translators.

## Example
Localization from English to Vietnam averagely will be causing the text to expand around 35%, so text like `Multiple Airlines` will be pseudolocalized to `[Mųŀŧįƿŀė ȂįřŀįƞėšMųŀŧįƿ]` (the original translation for *Multiple Airlines* is *nah hong hong kong*).

Notice that pseudolocalized text is still readable, so you won't lose context when adjusting the UI.

`add image of example here`

## Installation
1. Download the repository from this [link](https://github.com/arieare/Sketch-Pseudol10n/archive/master.zip).
2. Grab the `Pseudol10n` folder from the ZIP.
3. Double click the plugin to install in your sketch.


## Usage
### A. Pseudolocalize selected text layers
1. Make sure your text copy are in English (EN).
2. Select a text layer, or group of layers.
3. Pseudolocalize to your target language.
4. Your pseudolocalized text layers will be suffixed with `[target language]` (for example `[TH]` for Thailand) and the original text layers will be hidden.

![alt text](img/1-psdlc-selected-text.gif "Pseudolocalize selected text layers")

### B. Pseudolocalize all text in artboards
1. Make sure your text copy are in English (EN).
2. Select artboards to pseudolocalize.
3. Pseudolocalize to your target language.
4. All text layers inside selected artboard will be pseudolocalized and suffixed with `[target language]` (for example `[TH]` for Thailand) and the original text layers will be hidden.

### C. Pseudolocalize page
1. Make sure your text copy are in English (EN).
2. Deselect anything.
3. Pseudolocalize to your target language.
4. A new duplicate page will be created and suffixed with `[target language]` (for example `[TH]` for Thailand).
5. All text layers should be pseudolocalized.
6. A `json` file containing your string key will be copied to your clipboard.
7. Open up your favorite text editor (such as Sublime) and paste the `json`.
8. Save it as `json` file, and give it to your content editor to be translated.

### D. Pseudolocalize page
1. Go to page that you wish to be localized.
2. Localize from a `json` file.
3. Pick `json` file that you already translated on `C`.

### E. Exclude text layers
1. A lot of time you'll find some text doesn't need to be localized (for example, numbers!)
2. To exclude text layers just lock them before performing pseudolocalization.

## Help me improve Pseudol10n
To propose changes, fork the repository and submit a pull request!

## Questions?
[@arieare](http://twitter.com/arieare)

## Thanks to
[Sketch i18n](https://github.com/kristof/sketch-i18n), [pseudoloc js](https://github.com/bunkat/pseudoloc)
