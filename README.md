# SAFE ROUTE signed regional data

Public downloads for independent SAFE ROUTE test-app users in Malta/Gozo, the United Kingdom,
Tasmania and Latvia. No user account or routing-server account is required. Journeys, preferences,
avoidances and routing state stay on each device. BRouter calculates on the phone; this service
supplies immutable data and has no shared user route state.

Catalogue: https://github.com/Nundrian/safe-route-regional-data/releases/latest/download/catalogue.json

Signed catalogue revision8 contains1,784 entries:1,760 quarter-degree map cells,20 indivisible
native BRouter graph packages and4 optional full-region packages. Existing revision2 archives are
unchanged. Map cells are immutable Git objects on commit45f5871806ec1b21bd97bb93e6ba20e683ad327f;
native/full archives are release assets. Routing and display coverage are tracked independently.
Native routing files cannot be cropped into arbitrary corridors; package size overhead is shown
before acquisition. The largest native archive is116,622,719bytes. Full UK is optional1.71GB.

## Contents and sources

| Area | Archive bytes | Source snapshot |
| --- | ---: | --- |
| Malta/Gozo | 5,510,481 | [Geofabrik Malta261031](https://download.geofabrik.de/europe/malta-261031.osm.pbf) |
| United Kingdom | 1,714,253,461 | [Geofabrik UK261030](https://download.geofabrik.de/europe/united-kingdom-261030.osm.pbf) |
| Tasmania | 62,421,926 | [Geofabrik Tasmania261030](https://download.geofabrik.de/australia-oceania/australia/tasmania-261030.osm.pbf) |
| Latvia | 159,717,607 | [Geofabrik Latvia261031](https://download.geofabrik.de/europe/latvia-261031.osm.pbf) |

OpenStreetMap contributors, [ODbL1.0](https://www.openstreetmap.org/copyright). Derived databases
are supplied under ODbL1.0; preserve contributor attribution and the package notices. Each ZIP
contains corresponding source URL/hash, source-footprint mask, compatible custom BRouter graphs/
profiles/lookups, OSM-only tilemaker MBTiles, Noto glyphs and component hashes/signature. Included
notices identify BRouter MIT, tilemaker BSD and Noto SIL OFL1.1 material. The signature authority
is the unpromoted SAFE ROUTE038 test authority; private signing keys are never published.
No cycling safety, conditional access, ferry transfer, terrain or weather certification is implied.

## Operational limits

This uses existing public GitHub repository storage and Releases, without LFS, Actions, Packages,
Codespaces or metered compute. No paid commitment was created. It is not unlimited hosting.

- Maps:2,882,935,947 archive bytes; largest27,078,994bytes. Native graphs:191,377,453bytes.
- Four full archives:1,941,903,475bytes. All alternatives total5,016,216,875bytes, not one download.
- Releases:up to1,000 assets/release, each under2GiB. Native and full assets use separate releases.
- Git:100MB individual-file limit,2GB push limit; current recommended on-disk repository ceiling10GB.
  Map publication used five pushes bounded below650MB; no file approaches100MB.
- GitHub publishes no aggregate release bandwidth quota, guaranteed download rate, concurrent-user
  capacity or availability SLA. Public CDN requests can be throttled or rejected under service policies.
  Phone downloads are anonymous HTTPS and do not each consume an authenticated REST API request.
- Deployment REST limits normally5,000 requests/hour authenticated,60/hour unauthenticated, plus
  secondary limits. No tester allowlist or assumed user count. These are service limits, not capacity
  promises. Observe failures and transfer times before increasing deployment scale.

Strong ETags and byte ranges permit safe resume when supplied; hashes and signatures remain
mandatory. Endpoint/catalogue configuration is independent of navigation and can move to funded
storage/CDN without changing journey logic. Device download permissions, roaming default OFF,
bounded waits, storage checks, cancellation and retry still apply.

Sources: [release limits](https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases),
[repository limits](https://docs.github.com/en/repositories/creating-and-managing-repositories/repository-limits),
[large files](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github),
[REST limits](https://docs.github.com/en/rest/using-the-rest-api/rate-limits-for-the-rest-api).
