# ng-lint-staged

Inspired by: https://github.com/angular/angular-cli/issues/7612#issuecomment-455802617

Angular 7 provides the `--files` CLI option to lint certain files only instead of all project files.
However, since `lint-staged` provides a regular list only, a tiny argument transformation is required.

This shim provides such a transformation.


## Usage

**Note** that a trailing `--` is required in the call to `ng-lint-staged` to inform it about the starting point of
the files list.

```json
{
  "lint-staged": {
    "src/**/*.ts": [
        "ng-lint-staged lint --fix --"
    ]
  }
}
```


## License

(The MIT License)

Copyright (c) 2019 elunic AG/William Hefter <wh@elunic.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
