# Tixte Wrapper

> The best Tixte wrapper around

Install

```sh
npm i @ultirequiem/tixte # yarn add @ultirequiem/tixte
```

Usage

```ts
const tixteClient = new TixteClient(process.env.TIXTE_API_KEY, {
  defaultURL: "sergif.likes.cash",
});

const upload = async (event) => {
  const { data } = await tixteClient.uploadFile(
    Buffer.from(event.body!, "base64"),
    {
      extension: "gif",
    }
  );

  return data;
};
```

[Check a real word example!](https://github.com/UltiRequiem/sergif/tree/main/src/api)

## Using `@ultirequiem/tixte`

Are you using this package? Add it here!

- [Sergif](https://sergif.ultirequiem.com) - Netlify Functions - **Netlify x Hashnode 2022 Hackathon**

- [Piolafood](https://github.com/UltiRequiem/piolafood) - Next.js Endpoints - **First Buildergroop Hackathon**

## Licence

Licenses under the MIT Licence.
