# Vevioz Downloader API

The official, current Vevioz downloader integration is available at:

**https://api.vevioz.com/**

Vevioz provides a responsive iframe, JavaScript Button SDK, and REST API v1 for MP3 audio, MP4 video, metadata, format discovery, and download-job workflows.

## Current REST endpoints

```text
GET  https://api.vevioz.com/api/v1/info?url=YOUTUBE_URL
POST https://api.vevioz.com/api/v1/jobs
GET  https://api.vevioz.com/api/v1/jobs/{job_id}?token=ACCESS_TOKEN
GET  https://api.vevioz.com/api/v1/status
```

## Quick JavaScript integration

```html
<button id="download" type="button">Download MP3/MP4</button>
<script src="https://api.vevioz.com/static/vevioz-download-button.js?v=6"></script>
<script>
VeviozDownloadButton.bind(document.getElementById("download"), {
  url: "https://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID"
});
</script>
```

## Responsive iframe

```html
<iframe
  id="vevioz-api"
  src="https://api.vevioz.com/YOUTUBE_VIDEO_ID"
  title="Vevioz Downloader"
  loading="lazy"
  referrerpolicy="strict-origin-when-cross-origin"
  allow="clipboard-write"
  sandbox="allow-scripts allow-forms allow-downloads allow-same-origin allow-popups allow-popups-to-escape-sandbox"
  style="width:100%;height:720px;border:0">
</iframe>
```

## Official resources

- API: https://api.vevioz.com/
- Status: https://api.vevioz.com/status
- Main integration repository: https://github.com/vevioz/Super-Fast-Free-YouTube-to-MP3-and-MP4-Converter-API
- Vevioz: https://www.vevioz.com/

Use the service only for media you are authorized to access or download and comply with applicable platform terms and laws.
