## 📦 Install

This package is binary and doesn't require installation however you can add it to your repository as a `devDependency`:

```shell
npm install --save-dev @khulnasoft-opensource/check-engines
```

## 🚀 Usage

All you have to do is run the script next to your `package.json`:

```shell
npx @khulnasoft-opensource/check-engines
```

## 🔧 Configuration

The most common use case for this package is to let it run on `install` and `start` generic `npm` scripts:

```json
{
  "scripts": {
    "preinstall": "npx @khulnasoft-opensource/check-engines",
    "prestart": "npx @khulnasoft-opensource/check-engines"
  }
}
```

Or with less copy paste:

```json
{
  "scripts": {
    "engines": "npx @khulnasoft-opensource/check-engines",
    "preinstall": "npm run engines",
    "prestart": "npm run engines"
  }
}
```
