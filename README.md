# Ghost
Proof of concept Ghost CMS

## How to install
- Install ghost-cli terlebih dahulu
```bash
npm install -g ghost-cli@latest
# atau
yarn global add ghost-cli@latest
```
- Lalu duplikat file `.config.development.json` dan hilangkan tanda `.`, kemudian buka file tersebut.
- Rubah key `database` ke lokasi direktori kamu, contoh:
```json
{
  "filename": "/Users/namauser/lokasifolderghost/content/data/ghost.local.db",
}
```
- Dan rubah juga di file config tersebut `contentPath`, contoh:
```json
{
  "filename": "/Users/namauser/lokasifolderghost/content",
}
```
- Setelah selesai pindah ke folder `versions/4.12.1/` dan install dependency:
```bash
yarn
```
- Sebelum memulai jalankan dulu perintah:
```bash
ghost doctor
```
- Lalu jalankan ghost di root folder
```bash
ghost start
```

## Reference
https://ghost.org/docs/ghost-cli/#ghost-doctor
