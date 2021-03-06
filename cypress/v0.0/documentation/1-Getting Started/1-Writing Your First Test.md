slug: writing-your-first-test
excerpt: Walkthrough writing your first test

# Contents

- :fa-angle-right: [Folder Structure](#section-folder-structure)
- :fa-angle-right: [Test Files](#section-test-files)
- :fa-angle-right: [How to Write Tests](#section-how-to-write-tests)

***

# Folder Structure

After adding a new project, Cypress will automatically scaffold out a suggested folder structure. By default it will create:

```text
/cypress
/cypress/fixtures
/cypress/integration
/cypress/support
```

Cypress also adds placeholder files to help get you started with examples in each folder.

**Example JSON fixture**
```text
/cypress/fixtures/example.json
```

**Example Integration Test**
```text
/cypress/integration/example_spec.js
```

**Example JavaScript Support Files**
```text
/cypress/support/commands.js
/cypress/support/defaults.js
/cypress/support/index.js
```

While Cypress allows for configuration of where your tests, fixtures, and support files can be located, if you're starting your first project, we recommend you use the above structure.

[block:callout]
{
  "type": "info",
  "body": "You can modify the folder configuration in your `cypress.json`. See [configuration](https://on.cypress.io/guides/configuration) for more detail.",
  "title": "Configure Folder Structure"
}
[/block]

***

# Test Files

Test files may be written as `.js`, `.jsx`, `.coffee`, or `cjsx` files.

Cypress supports ES2015, ES2016, ES2017, and JSX. ES2015 modules and CommonJS modules are also supported, so you can `import` or `require` both npm packages and local modules.

To see an example of every command used in Cypress, open the `example_spec.js` within your `cypress/integration` folder.

To start writing tests for your app, simply create a new file like `app_spec.js` within your `cypress/integration` folder. Refresh your tests list in the Cypress GUI and your new file should have appeared in the list.

***

# How to write tests

Cypress is built on top of [Mocha](https://on.cypress.io/guides/bundled-tools#section-mocha) and uses its `bdd` interface. Tests you write in Cypress will mostly adhere to this style.

If you're familiar with writing tests in JavaScript, then writing tests in Cypress will be a breeze.

We're still working on introductory docs and videos. For now, [check out some examples](https://on.cypress.io/guides/all-example-apps) of applications using Cypress tests.
