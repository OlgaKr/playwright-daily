# Playwright Daily Lab — Cheatsheet

Short Playwright examples for quick reference.

## Run tests

Run all tests:

```bash id="0fo9vd"
npx playwright test
```

Run one file:

```bash id="3crg10"
npx playwright test tests/example.spec.ts
```

Run in headed mode:

```bash id="m7xm3a"
npx playwright test --headed
```

Run in UI Mode:

```bash id="p9k73g"
npx playwright test --ui
```

Run in debug mode:

```bash id="azf9gd"
npx playwright test --debug
```

## Basic test

```ts id="i0ar4m"
import { test, expect } from '@playwright/test';

test('example test', async ({ page }) => {
  await page.goto('https://example.com');

  await expect(page).toHaveTitle(/Example/);
});
```

## Common locators

```ts id="9tqu29"
page.getByRole('button', { name: 'Submit' });
page.getByText('Welcome');
page.getByLabel('Email');
page.getByPlaceholder('Enter email');
page.getByTestId('login-button');
page.locator('.product-card');
```

## Common actions

```ts id="gvcbha"
await locator.click();
await locator.fill('Olga');
await locator.check();
await locator.uncheck();
await locator.hover();
await locator.press('Enter');
```

## Common assertions

```ts id="t9xhkl"
await expect(locator).toBeVisible();
await expect(locator).toHaveText('Success');
await expect(locator).toContainText('Success');
await expect(locator).toHaveValue('Olga');
await expect(locator).toHaveCount(3);
```

---

New examples will be added gradually during daily practice.
