# Playwright Snippets

![Build status](https://github.com/mskelton/vscode-playwright-test-snippets/workflows/Release/badge.svg?branch=main)
[![Extension version](https://img.shields.io/vscode-marketplace/v/mskelton.playwright-test-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=mskelton.playwright-test-snippets)
[![Extension installs](https://img.shields.io/vscode-marketplace/i/mskelton.playwright-test-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=mskelton.playwright-test-snippets)
[![Semantic release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)

[Playwright test](https://playwright.dev) snippets for VS Code.

## Snippets

The following snippets are provided by this package. If you have ideas of other snippets that would be helpful, please [open an issue](https://github.com/mskelton/vscode-playwright-test-snippets/issues/new).

### Test blocks

#### `pw-describe`

```ts
test.describe('$1', () => {
  $0
})
```

#### `pw-test`

```ts
test('$1', async ({ page }) => {
  $0
})
```

#### `pw-beforeEach`

```ts
test.beforeEach(async ({ page }) => {
  $0
})
```

#### `pw-afterEach`

```ts
test.afterEach(async ({ page }) => {
  $0
})
```

#### `pw-beforeAll`

```ts
test.beforeAll(async ({ browser }) => {
  $0
})
```

#### `pw-afterAll`

```ts
test.afterAll(async ({ browser }) => {
  $0
})
```

#### `pw-step`

```ts
await test.step('$1', async () => {
  $0
})
```

#### `pw-use`

```ts
test.use({ $0 })
```

### Lariat

[Lariat](https://github.com/Widen/lariat) is a Playwright page object framework that simplifies page object construction. We've included some useful Lariat snippets as part of this extension.

#### `pw-collection`

```ts
import Collection from 'lariat'

export class MyPage extends Collection {
  $0
}
```

#### `pw-page-object`

```ts
import { Page } from '@playwright/test'
import Collection from 'lariat'

export class MyPage extends Collection {
  constructor(page: Page) {
    super(page.locator('$1'))
  }

  $0
}
```
