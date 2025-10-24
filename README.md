# Leaflet RSS Embed

A lightweight service to embed your [Leaflet](https://about.leaflet.pub/) publication feed into any Leaflet document. The styling matches Leaflet's design, ensuring seamless integration into your existing documents.

## Demo

Check out the live demo: [https://leaflet.pub/ed1df522-3500-4e21-b6d6-350539096424](https://leaflet.pub/ed1df522-3500-4e21-b6d6-350539096424)

## How to Use

Embed the service using an iframe with URL parameters to customize the feed display:

### Basic Usage

Create an embed block in you leaflet document and add the following URL (replace the URL with your URL of your publications feed):

```html
https://www.niklasjordan.com/leaflet-rss-embed/?rss=YOUR_RSS_FEED_URL
```

### URL Parameters

| Parameter | Description | Default | Required |
|-----------|-------------|---------|----------|
| `rss` | Your Leaflet RSS feed URL | None | **Yes** |
| `color` | Link color in hex format (URL-encoded, e.g., `%230047FF`) | `#0047FF` | No |
| `limit` | Number of feed items to display | `5` | No |

### Examples

**Display 10 items from your feed:**
```html
<iframe src="https://www.niklasjordan.com/leaflet-rss-embed/?rss=https://yourname.leaflet.pub/rss&limit=10"></iframe>
```

**Custom link color (red):**
```html
<iframe src="https://www.niklasjordan.com/leaflet-rss-embed/?rss=https://yourname.leaflet.pub/rss&color=%23FF0000"></iframe>
```

**All parameters combined:**
```html
<iframe src="https://www.niklasjordan.com/leaflet-rss-embed/?rss=https://yourname.leaflet.pub/rss&color=%2300FF00&limit=3"></iframe>
```

## License

MIT
