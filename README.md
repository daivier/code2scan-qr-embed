# Free QR Code Generator Widget

Embed a **free QR Code generator** on any website with **one line of HTML**. No signup, no API key, no watermark.

> Live widget: **https://www.code2scan.com/embed/qr** · Copy the snippet at **https://www.code2scan.com/qr-code-widget**

![QR Code generator widget](https://www.code2scan.com/icons/icon-192.png)

## Quick start

Paste this where you want the generator to appear:

```html
<iframe src="https://www.code2scan.com/embed/qr"
        width="100%" height="400"
        style="border:0;max-width:340px" loading="lazy"
        title="Free QR Code Generator"></iframe>
<p style="font:13px sans-serif">
  <a href="https://www.code2scan.com/" target="_blank" rel="noopener">Free QR Code Generator</a> by Code2Scan
</p>
```

That's it. Your visitors get a working QR Code generator; you don't run or maintain anything.

## What it does

The embedded generator creates **static QR Codes that never expire** and work offline once scanned:

- **Links / URLs**, plain text
- **WhatsApp** (pre-filled message), **Wi-Fi** (join network on scan)
- **Pix** (Brazil's instant-payment QR — key, amount, message)
- **vCard** / contact, email, phone, SMS, event

Codes are rendered client-side, need **no account**, and have **no watermark**. The interface ships in **9 languages** (EN, ES, PT, FR, DE, IT, HI, JA, AR).

## Platform guides

| Platform | How to embed |
|---|---|
| **Plain HTML** | Paste the snippet into your page. See [`examples/plain.html`](examples/plain.html). |
| **WordPress** | Add a **Custom HTML** block and paste the snippet. See [`examples/wordpress.html`](examples/wordpress.html). |
| **Wix / Squarespace** | Add an **Embed / Code** element and paste the snippet. |
| **React / Next.js** | Drop the `<iframe>` straight into your JSX (it's valid HTML). |

## Customize the size

The widget is responsive. Change `max-width` and `height` to fit your layout:

```html
<iframe src="https://www.code2scan.com/embed/qr"
        width="100%" height="460"
        style="border:0;max-width:400px" loading="lazy"
        title="Free QR Code Generator"></iframe>
```

## How it works

- The widget is a standalone page served at `/embed/qr`, iframable on any origin (`Content-Security-Policy: frame-ancestors *`).
- QR rendering happens in the browser with [`qr-code-styling`](https://github.com/kozakdenys/qr-code-styling).
- No tracking cookies, no API key, no backend call for static codes.

## Need more?

Dynamic QR Codes (editable destination + scan analytics), a Link‑in‑Bio builder, a URL shortener and a barcode generator live at **[code2scan.com](https://www.code2scan.com/)**.

## License

The example code in this repo is released under the [MIT License](LICENSE). The hosted widget is a free service of [Code2Scan](https://www.code2scan.com/).
