# Amplify Sample App
## React Setup

React App Created with the following command
```
npx create-react-app@latest --scripts-version 4.0.3 uibuild
```

added dependencies
```
npm i -E @aws-amplify/ui-react aws-amplify @types/react
```

when running `npm start` the following error message shows up
```bash
./node_modules/react-map-gl/dist/esm/components/use-control.js 12:46
Module parse failed: Unexpected token (12:46)
File was processed with these loaders:
 * ./node_modules/babel-loader/lib/index.js
You may need an additional loader to handle the result of these loaders.
| 
|     if (!map.hasControl(ctrl)) {
>       map.addControl(ctrl, (opts || onRemove)?.position);
|     }
|
```

## Studio Setup

Create an amplify studio app, created a baseComponent with the following command

```bash
aws amplifyuibuilder create-component --app-id myAppId --environment-name staging --component-to-create file://baseComponent.json
```