# Storybook Code Block Reproduction Case

```sh
npm install && npm run storybook
```

1. open storybook
2. switch to "Docs" tab
3. Click "Show Code" button to expand the code block

You should see 

```
[object Object],[object Object],[object Object],[object Object],[object Object],[object Object],[object Object],[object Object],[object Object],[object Object],[object Object],[object Object],[object Object],[object Object],[object Object],[object Object]
```

Interestingly enough, if you click "Copy" button, you will see the following:

```
<Styled(h1)>
  Basic title
</Styled(h1)>
```

which is the expected result.

I tried removing `@storybook/componnents` dependency from `package.json` and it worked as expected.
