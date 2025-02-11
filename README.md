# pw-sample-bs-error

# Requirements
- Node 18+

# How run:

- Set the username and accesskey into browserstack.yml file:

- Open terminal on root directory of the project:

```
 npm install
 npm i -g npx
 npx browserstack-node-sdk install
 npx browserstack-node-sdk test
```


# Problem:

If a test passes the following test use the same session and overwrite the result:

```
npx browserstack-node-sdk playwright test "resultisoverwritten.spec.ts"
```


If a test fail then the following test will always start a new session:

```
npx browserstack-node-sdk playwright test "resultsaresepareted.spec.ts"
```


