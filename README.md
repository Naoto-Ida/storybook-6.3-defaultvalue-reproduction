# 

## Steps

Run
```
cd sb-regression 
yarn storybook
```

Open http://localhost:6006/?path=/docs/example-button--primary&globals=measureEnabled:false

## Problem

After upgrading from 6.2.9 to 6.3.0, we've lost the feature to have SB select the default value in the Controls column.

For example, in the demo files produced with `npx sb init`, a `Button.tsx` is created.
Its `size` prop has a default value of `medium`, but the [RadioControl](https://github.com/storybookjs/storybook/blob/7064642e1aee7786c77fe735c064c0c29dbcee01/lib/components/src/controls/options/Radio.tsx) does not select the radio option labeled `medium` anymore.

