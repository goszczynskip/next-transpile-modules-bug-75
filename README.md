# Repo for bug [75](https://github.com/martpie/next-transpile-modules/issues/75) of next-transpile-modules

## Repro steps

* make sure you have yarn up to date (v1.22)
* run `yarn install`
* `cd application`
* `yarn dev`
* Visit `localhost:3000`
  
This will produce error in console.
```
...
[ error ] ../feature/index.tsx 3:29
Module parse failed: Unexpected token (3:29)
You may need an appropriate loader to handle this file type, currently no loaders are configured to process this file. See https://webpack.js.org/concepts#loaders
| import React, {FC} from "react";
|
> export const FeatureComponent: FC = () => {
|   return <div>FeatureComponent</div>;
| }
[ event ] build page: /next/dist/pages/_error
...
```