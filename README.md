# rocket-boots-eslint
*Opinionated ES Linting Config*

## How to Use

1. Bring the library into your project:
   ```
   npm install github:rocket-boots/rocket-boots-eslint --save-dev
   ```
2. Make a `.eslintrc.cjs` file in the root of your ECMAScript/JavaScript project with:
   ```js
   module.exports = {
		extends: [
			'./node_modules/rocket-boots-eslint/eslint-config.cjs',
		],
		rules: {
			// your custom rules here
		},
	};
	```
	OR
    ```js
	const config = require('./node_modules/rocket-boots-eslint/eslint-config.cjs');
	module.exports = { ...config };
	```
  - See https://eslint.org/docs/latest/use/configure/configuration-files#using-a-configuration-file
  - Note: Because of the `.cjs` this config can co-exist with an ESM ("module" type) node project.
