## One way to start a Expo project

#### 1. Install Expo CLI
```
npm install -g expo-cli
```

#### 2. Create a new project
```bash
npx create-expo-app `app-name`
```

#### 3. Change App.js for App.tsx
```bash
mv App.js App.tsx
```

#### 4. Run project
```bash
npm run start
```

#### 5. Install NativeWind
```bash
npm install nativewind
```

#### 6. Install tailwindcss
```bash
npm install tailwindcss -D
```

#### 7. Create tailwind.config.js
```bash
npx tailwindcss init
```

#### 8. In tailwind.config.js, add the following:
```js
content: ["./App.{js,jsx,ts,tsx}", ".<custom directory>/**/*.{js,jsx,ts,tsx}"],
```

#### 9. In babel.config.js, add the following:
```js
plugins: ["nativewind/babel"],
```

#### 10. In ts.config.json, add the following:
```js
"compilerOptions": {
    "types": ["nativewind/types"]
  },
```

#### 11. Install eslint
```bash
npm install eslint @rocketseat/eslint-config -D
```

#### 12. Create .eslintrc.json
```json
{
  "extends": ["@rocketseat/eslint-config/react"]
}
```

#### 13. Install prettier
```bash
npm install prettier-plugin-tailwindcss -D
```

#### 14. Create pretttier.config.js
```js
module.exports = {
  plugins: [require("prettier-plugin-tailwindcss")],
};
```

