1. In Webstorm, click File -> Open -> first-project -> Open in a new window
2. Focus on new window
3. File -> Open -> second-project -> Attach to the same window
4. Make sure Biome plugin settings are set to automatically fix isuses on save
5. Go to `first-project/src/someCode.ts` and create some issue, fe. change remove space between var name and type: `(code:string): string`
6. Click cmd + S to save
7. Webstorm should fix the issue
8. Go to `second-project/src/someCode.ts` do exactly the same
9. Webstorm won't apply any fixes


You can also verify if your change in code is causing Biome formating error, by running `npm run lint` in `first-project` directory or `second-project`

Another way to verify the issue exists, is by check language services. For `second-project` Biome will be showing as "Running on Other files"