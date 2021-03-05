# Repro steps:
1) `npm install`
2) `npm run doc` - runs Typedoc 0.19.2 with typedoc-no-inherit-plugin, hides inherited members
3) `npm install typedoc@0.20.x typescript@4.2.x`
4) `npm run doc` - runs Typedoc 0.20.x with typedoc-no-inherit-plugin, doesn't hide inherited members

If running in VS Code, you can turn Auto Attach on and put a breakpoint in `node_modules/typedoc-plugin-no-inherit/dist/plugin.js:54`.
