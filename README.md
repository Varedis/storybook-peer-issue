# storybook-peer-issue
Replication repo for storybook peer dependency issue

# How to use

In it's current state with `react` and `react-dom` marked as dependencies this will cause a broken package tree, perform the following steps:

1. Install npm@7 `npm i -g npm@7`

2. Checkout the code.

3. Perform an install `npm install`.

4. Check the `node_modules` and expand the `@storybook` folder. Note that `addon-docs` is not installed there.

5. Remove `react` and `react-dom` as dependencies in `package.json`.

6. Delete `package-lock.json` and delete the `node_modules` folder.

7. Perform another install `npm install`.

8. Check the `node_modules` and expand the `@storybook` folder. Note that `addon-docs` now exists and is installed.

9. Add `react` and `react-dom` back as dependencies.

10. Delete `package-lock.json` and delete the `node_modules` folder.

11. Repeat step 3 and 4.
