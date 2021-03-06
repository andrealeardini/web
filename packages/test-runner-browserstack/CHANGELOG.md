# @web/test-runner-browserstack

## 0.1.2

### Patch Changes

- ce2a2e6: align dependencies
- Updated dependencies [ce2a2e6]
  - @web/dev-server-legacy@0.1.2
  - @web/test-runner-selenium@0.2.2

## 0.1.1

### Patch Changes

- aa65fd1: run build before publishing
- Updated dependencies [aa65fd1]
  - @web/dev-server-legacy@0.1.1
  - @web/test-runner-selenium@0.2.1

## 0.1.0

### Minor Changes

- fdcf2e5: Merged test runner server into core, and made it no longer possible configure a different server.

  The test runner relies on the server for many things, merging it into core makes the code more maintainable. The server is composable, you can proxy requests to other servers and we can look into adding more composition APIs later.

- 9be1f95: Added native node es module entrypoints. This is a breaking change. Before, native node es module imports would import a CJS module as a default import and require destructuring afterwards:

  ```js
  import playwrightModule from '@web/test-runner-playwright';

  const { playwrightLauncher } = playwrightModule;
  ```

  Now, the exports are only available directly as a named export:

  ```js
  import { playwrightLauncher } from '@web/test-runner-playwright';
  ```

### Patch Changes

- Updated dependencies [cdddf68]
- Updated dependencies [fdcf2e5]
- Updated dependencies [9be1f95]
  - @web/test-runner-selenium@0.2.0
  - @web/dev-server-legacy@0.1.0

## 0.0.12

### Patch Changes

- d77093b: allow code coverage instrumentation through JS
- Updated dependencies [d77093b]
  - @web/test-runner-selenium@0.1.8

## 0.0.11

### Patch Changes

- 02a3926: expose browser name from BrowserLauncher
- Updated dependencies [02a3926]
- Updated dependencies [74cc129]
  - @web/test-runner-selenium@0.1.7

## 0.0.10

### Patch Changes

- 432f090: expose browser name from BrowserLauncher
- 5b36825: prevent debug sessions from interferring with regular test sessions
- Updated dependencies [432f090]
- Updated dependencies [5b36825]
  - @web/test-runner-selenium@0.1.6

## 0.0.9

### Patch Changes

- 736d101: improve scheduling logic and error handling
- Updated dependencies [736d101]
  - @web/test-runner-selenium@0.1.5

## 0.0.8

### Patch Changes

- 5fada4a: improve logging and error reporting
- Updated dependencies [5fada4a]
  - @web/dev-server-legacy@0.0.3
  - @web/test-runner-selenium@0.1.4

## 0.0.7

### Patch Changes

- 04a2cda: make test-runner-browserstack work with dev-server-core
- Updated dependencies [04a2cda]
  - @web/test-runner-selenium@0.1.3

## 0.0.6

### Patch Changes

- db5baff: cleanup and sort dependencies

## 0.0.5

### Patch Changes

- 1d6d498: allow changing viewport in tests
- Updated dependencies [1d6d498]
  - @web/test-runner-selenium@0.1.1

## 0.0.4

### Patch Changes

- Updated dependencies [c4cb321]
  - @web/test-runner-selenium@0.1.0

## 0.0.3

### Patch Changes

- 14b7fae: handle errors in mocha hooks
- Updated dependencies [14b7fae]
  - @web/test-runner-selenium@0.0.4

## 0.0.2

### Patch Changes

- f2bf9ae: first setup of browserstack
- Updated dependencies [fbc1eba]
  - @web/test-runner-selenium@0.0.3
