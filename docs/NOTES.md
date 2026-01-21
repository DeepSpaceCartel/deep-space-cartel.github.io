# NOTES

## Development

In order to accept connections in container from host browser update the following in `package.json`:

```JSON
"scripts": {
    "dev": "astro dev --host 0.0.0.0 --port 4321",
},
```