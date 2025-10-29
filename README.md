# CDN by Kreftforeningen

This repository hosts CDN assets for fonts and brand files (logos).

- Deployment target: Netlify
- Intended usage: Public, cacheable static assets served over HTTPS

## CORS

Static headers on Netlify are configured via the `_headers` file to allow cross-origin access. For public CDN assets (fonts/logos), permissive CORS is typically acceptable. If you need to strictly allow only `kreft.no` and `kreftforeningen.no` (including subdomains), use a dynamic header (Edge Function) to echo back the request `Origin` when it matches an allowlist.

## Caching

Assets should be immutable and cached long-term. Adjust cache directives if your update strategy differs.

## Usage

- utm.kreftforeningen.no
- aarsrapport.kreftforeningen.no
- livestream.kreftforeningen.no
- julekort.kretforeningen.no

## Author

Asbjørn Ness

## License

MIT
