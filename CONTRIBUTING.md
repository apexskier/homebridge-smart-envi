# Contributing guide

## Local Development

Link plugin globally to get local homebridge to pick it up.

```
npm run link
```

Run homebridge locally with your local plugin and logs.

```
npm run build && DEBUG=*apexskier* homebridge -D -I
```

- `-D`: debug mode
- `-I`: show accessories in homebridge UI

## Publishing

Publishing is done through GitHub actions for trusted publishing.

When ready to publish, run this locally:

```bash
git push origin tags/$(npm version [type])
git push origin main
```
