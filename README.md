# pocs

pocs from our testing work. all bugs in this repo are responsibly disclosed.

| target | type | class | severity | disclosed | status | reference |
|---|---|---|---|---|---|---|
| priceline | web API | BOLA, cross-account reservation PII (CWE-639) | High (7.5) | 2026-06-04 | disclosed | [writeup](priceline/README.md) |
| priceline | mobile app | unrestricted Google Maps API key (CWE-790) | Low | 2026-06-04 | disclosed | [writeup](priceline/mapskey.md) |
| epicgames | mobile app, OAuth | code interception, shipped client secret, no PKCE (CWE-603) | High | 2026-07-18 | disclosed | [writeup](epicgames/README.md) |
| vercel | cloud platform | egress OIDC token not bound to tenant, 24h replay (CWE-283) | High | 2026-09-01 | disclosed | [writeup](vercel/README.md) |
| decagon | web API, chat widget | HMAC signature not enforced, cross-tenant support history (CWE-347) | High (8.1) | 2026-08-22 | disclosed | [writeup](decagon/README.md) |
| djangocms | CMS | missing authorization, placeholder structure disclosure (CWE-862) | Medium (4.3) | 2026-08-20 | disclosed | [CVE-2026-61663](https://github.com/django-cms/django-cms/security/advisories/GHSA-8qj2-c6q4-f399), [writeup](djangocms/README.md) |
| livekit | VoIP protocol | SIP trunk IP allowlist matched against the From header (CWE-346) | Critical (9.1) | 2026-08-22 | disclosed | [GHSA-82qx-7757-5jqv](https://github.com/livekit/protocol/security/advisories/GHSA-82qx-7757-5jqv), [writeup](livekit/README.md) |
