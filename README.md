# SuperViz (superviz)

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
