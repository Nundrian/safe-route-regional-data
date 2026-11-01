# SAFE ROUTE signed regional data distribution

Public, account-free downloads of existing signed revision-2 OSM-derived data for Malta/Gozo,
the United Kingdom, Tasmania and Latvia. This is data distribution, not a GraphHopper compute
service or a release of the Android application. No user journeys, preferences, traces, accounts
or route state are stored here. Independent users receive the same immutable archives.

The initial public catalogue offers four full-region archives. The application retains its
local-cell, buffered-corridor, alternative, prefetch and native-graph policies. Until finer
packages are added to this public catalogue, acquisition uses the actual full-region granularity:
there is unavoidable full-region download overhead, including1.71GB for the UK. Wi-Fi/mobile/
roaming and storage preferences still apply. No arbitrary cropping of BRouter graph files occurs.
The separately prepared1,784-package set is not falsely advertised as wholly public here.

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

This uses public **GitHub Releases**, not GitHub Pages, LFS, Packages, Actions or Codespaces.
Current [release documentation](https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases)
permits up to1,000 assets per release and individual files under2GiB. These four archives total
1,941,903,475bytes. GitHub does not publish a total release-size or bandwidth quota on that page;
this is **not** a promise of unlimited throughput, concurrency, availability or immunity from
abuse/rate limiting. No request-rate or concurrent-download SLA is established. Public HTTPS
delivery may redirect to GitHub's asset CDN. Clients retain hash/signature verification, bounded
network waits, cancellation, resume where permitted and retry/backoff on failures.

Deployment uses authenticated REST calls with account/secondary rate limits; ordinary app downloads
use public asset URLs and require no GitHub account/token. No metered compute, LFS, Actions or
Packages allowance is enabled. If measured demand outgrows this service, the signed catalogue and
package origin are configurable independently of navigation, and can move to appropriately funded
object storage/CDN without rewriting journey state or routing logic. No user count is assumed.
