This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, install the dependencies

```bash
npm install
# or
yarn add
```

SEcond, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

Now you can start editing the project. The page auto-updates as you edit the file.

To configure the EsLint rules, just copy the following JSON code into the `.eslintrc.json` file.

```json
{
  "env": {
    "browser": true,
    "es2021": true
  },
  "extends": [
    "next/core-web-vitals",
    "plugin:react/recommended",
    "airbnb",
    "plugin:react/jsx-runtime",
    "prettier"
  ],
  "overrides": [],
  "parserOptions": {
    "ecmaVersion": "latest",
    "sourceType": "module"
  },
  "plugins": ["react", "react-hooks", "prettier"],
  "rules": {
    "react-hooks/rules-of-hooks": "error", // Checks rules of Hooks
    "react-hooks/exhaustive-deps": "warn", // Checks effect dependencies
    "react/jsx-filename-extension": [1, { "extensions": [".js", ".jsx"] }],
    "react/prop-types": "off", // Desactive if required
    "react/jsx-props-no-spreading": "off", // Desactive if required
    "prettier/prettier": [
      "error",
      {
        "trailingComma": "all",
        "singleQuote": true,
        "jsxSingleQuote": false,
        "printWidth": 100,
        "tabWidth": 2,
        "endOfLine": "auto",
        "arrowParens": "always"
      }
    ]
  }
}
```