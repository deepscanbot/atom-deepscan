# atom-deepscan

[![Version](https://img.shields.io/apm/v/atom-deepscan.svg?style=flat-square)](https://atom.io/packages/atom-deepscan)
[![DeepScan Grade](https://deepscan.io/api/projects/337/branches/538/badge/grade.svg)](https://deepscan.io/dashboard/#view=project&pid=337&bid=538)

Atom package to detect bugs and quality issues in JavaScript, TypeScript and React. Works with [DeepScan](https://deepscan.io).

DeepScan is a cutting-edge JavaScript code inspection tool that helps you to find bugs and quality issues more precisely by data-flow analysis. You can also use it for React because DeepScan delivers [React specific rules](https://deepscan.io/docs/rules/#react).

> **Note:**
> To use this extension, you should confirm that your code is transferred to the DeepScan server for inspection when you save your changes.
> You can confirm it by pressing the Confirm button that appears when restarting Atom after the installation.
>
> Note that your code is completely deleted from the server right after the inspection.

![Navigation](https://github.com/deepscan/atom-deepscan/raw/master/preview.png)

## Installation

```ShellSession
apm install atom-deepscan
```

## How it works

- You need [Linter](https://atom.io/packages/linter) package. Once Linter package is installed, just restart Atom.
- Report issues in the Linter view when you open a JS or JSX file and save it.
- Highlight issues in the code.
- For support of `.jsx` file, include grammar of [atom-react](https://github.com/orktes/atom-react).
- For support of `.ts` and `.tsx` file, include grammar of [language-typescript-grammars-only](https://github.com/tcarlsen/language-typescript-grammars-only).

## Settings Options

This plugin contributes the following variables to the settings:

- `enable`: enable/disable DeepScan. Disabled by default. Enabled when you confirm.
- `server`: set an url of DeepScan server. "https://deepscan.io" by default.
- `ignoreRules`: set an array of rules to exclude.

![Settings](https://github.com/deepscan/atom-deepscan/raw/master/settings.png)