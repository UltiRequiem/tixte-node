# Tixte Wrapper

> The best Tixte wrapper around

Install

```sh
npm i @ultirequiem/tixte # yarn add @ultirequiem/tixte
```

Usage

```ts
export const tixteClient = new TixteClient(process.env.TIXTE_API_KEY!, {
  defaultURL: "sergif.likes.cash",
});

export const upload = async (event) => {
  const {
    data: { url, direct_url },
  } = await tixteClient.uploadFile(Buffer.from(event.body!, "base64"), {
    extension: "gif",
  });

  return { url, direct_url };
};
```

[Check a real word example!](https://github.com/UltiRequiem/sergif/tree/main/src/api)

## Using `@ultirequiem/tixte`

Are you using this package in your codebase? Add it here!

- [Sergif](https://sergif.ultirequiem.com) - Uses this packages on the Netlify Functions

## Licence

Licenses under the MIT Licence.
