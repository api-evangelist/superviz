# SuperViz (superviz)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

SuperViz provides real-time collaboration and data-synchronization infrastructure for web applications - presence, realtime data channels, video huddle/meetings, contextual comments, and mouse pointers. The product is SDK-first (@superviz/sdk and @superviz/react-sdk initialized with a developer key), supported by a REST API at api.superviz.com for participants, presence, channels, rooms, comments, and meetings, an event-driven realtime channel API, and webhooks.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/apis.yml)

## Tags

- Real Time
- Collaboration
- Presence
- Synchronization
- Video
- WebRTC
- SDK

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### SuperViz Participants API

Server-side REST endpoint that returns the list of participants currently connected to a given realtime channel, authenticated with the client_id and secret developer keys.

- **Human URL:** [https://docs.superviz.com/realtime/1.0/rest-api/presence](https://docs.superviz.com/realtime/1.0/rest-api/presence)
- **Base URL:** `https://api.superviz.com`

#### Tags

- Participants
- Presence
- Real Time

#### Properties

- [Documentation](https://docs.superviz.com/realtime/1.0/rest-api/presence)
- [API Reference](https://docs.superviz.com/realtime/1.0/rest-api/presence)
- [OpenAPI](openapi/superviz-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/superviz.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/superviz.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### SuperViz Channels API

Lists the realtime channels active for a room, used to introspect where presence and messages are flowing across a collaborative application.

- **Human URL:** [https://docs.superviz.com/realtime/1.0/rest-api/channels](https://docs.superviz.com/realtime/1.0/rest-api/channels)
- **Base URL:** `https://api.superviz.com`

#### Tags

- Channels
- Real Time
- Presence

#### Properties

- [Documentation](https://docs.superviz.com/realtime/1.0/rest-api/channels)
- [OpenAPI](openapi/superviz-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/superviz.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/superviz.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### SuperViz Realtime Data API

Publish (post) events with an arbitrary JSON payload to a named realtime channel from a backend, so servers can push synchronized data to connected SDK clients. The channel/event model is described as AsyncAPI alongside the REST publish endpoint.

- **Human URL:** [https://docs.superviz.com/realtime/1.0/rest-api/publish-message-to-channel](https://docs.superviz.com/realtime/1.0/rest-api/publish-message-to-channel)
- **Base URL:** `https://api.superviz.com`

#### Tags

- Real Time
- Events
- Pub Sub
- Synchronization

#### Properties

- [Documentation](https://docs.superviz.com/realtime/1.0/rest-api/publish-message-to-channel)
- [OpenAPI](openapi/superviz-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/superviz-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/superviz.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/superviz.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### SuperViz Rooms API

Collaboration REST surface for rooms - retrieve a room's participants and related collaboration context, with cursor-style pagination on list responses.

- **Human URL:** [https://docs.superviz.com/collaboration/rest-api/how-to-use](https://docs.superviz.com/collaboration/rest-api/how-to-use)
- **Base URL:** `https://api.superviz.com`

#### Tags

- Rooms
- Collaboration
- Participants

#### Properties

- [Documentation](https://docs.superviz.com/collaboration/rest-api/how-to-use)
- [OpenAPI](openapi/superviz-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/superviz.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/superviz.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### SuperViz Contextual Comments API

Reads the contextual comments (annotations pinned to elements of a web app or 3D scene) created through the Collaboration SDK, exposed server-side over REST for backend workflows.

- **Human URL:** [https://docs.superviz.com/collaboration/rest-api/how-to-use](https://docs.superviz.com/collaboration/rest-api/how-to-use)
- **Base URL:** `https://api.superviz.com`

#### Tags

- Comments
- Annotations
- Collaboration

#### Properties

- [Documentation](https://docs.superviz.com/collaboration/rest-api/how-to-use)
- [OpenAPI](openapi/superviz-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/superviz.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/superviz.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### SuperViz Meetings API

Retrieves video meeting (huddle) statistics - duration, minutes, price, recordings, and per-participant join detail - for meetings created with the Video SDK.

- **Human URL:** [https://docs.superviz.com/video-sdk/webhooks/meeting-stats](https://docs.superviz.com/video-sdk/webhooks/meeting-stats)
- **Base URL:** `https://api.superviz.com`

#### Tags

- Video
- Meetings
- Huddle

#### Properties

- [Documentation](https://docs.superviz.com/video-sdk/webhooks/meeting-stats)
- [OpenAPI](openapi/superviz-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/superviz.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/superviz.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### SuperViz Webhooks API

Outbound webhook notifications SuperViz POSTs to a preconfigured receiver when events occur - meeting stats available (MEETING_STATS), recording ready, and transcription ready. Modeled as AsyncAPI event messages.

- **Human URL:** [https://docs.superviz.com/video-sdk/webhooks/meeting-stats](https://docs.superviz.com/video-sdk/webhooks/meeting-stats)
- **Base URL:** `https://api.superviz.com`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.superviz.com/video-sdk/webhooks/meeting-stats)
- [OpenAPI](openapi/superviz-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/superviz-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/superviz.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/superviz.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### SuperViz Authentication API

Credential model for SuperViz - a developer key initializes the client SDK, while a Client ID plus Secret Key pair (from Dashboard > Developer > Keys) authenticates all server-side REST requests via client_id and secret headers.

- **Human URL:** [https://docs.superviz.com/getting-started/setting-up-your-account](https://docs.superviz.com/getting-started/setting-up-your-account)
- **Base URL:** `https://api.superviz.com`

#### Tags

- Authentication
- Keys
- Tokens

#### Properties

- [Documentation](https://docs.superviz.com/getting-started/setting-up-your-account)
- [OpenAPI](openapi/superviz-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/superviz.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/superviz.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/SuperViz)
- [LinkedIn](https://www.linkedin.com/company/superviz)
- [Website](https://superviz.com/)
- [Documentation](https://docs.superviz.com)
- [Plans](plans/superviz-plans-pricing.yml)
- [Rate Limits](rate-limits/superviz-rate-limits.yml)
- [Fin Ops](finops/superviz-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
