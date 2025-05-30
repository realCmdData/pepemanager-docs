---
description: Get started with the Lurkr API and build your app with integrated leveling!
---

# 🗝️ API Introduction

## Guide

The Lurkr API (v2) is a RESTful API that enables seamless integration with Lurkr’s features from your own applications. This documentation will help you get started with making requests and handling responses.

## Quick Start

1. Create your API key in your [profile page](https://lurkr.gg/profile). Make sure to allow access to some servers.
2. Include the API key in the `X-API-Key` header
3. Make requests to the base URL: `https://api.lurkr.gg/v2`

Example request using cURL:

```url
curl -H "X-API-Key: your-api-key" https://api.lurkr.gg/v2/levels/{guildId}/users/{userId}
```

<sub>Make sure to replace</sub> <sub></sub><sub>`{guildId}`</sub> <sub></sub><sub>any</sub> <sub></sub><sub>`{userId}`</sub> <sub></sub><sub>with the actual guild and user IDs.</sub>

***

## Versioning

The current version of the API is v2. All endpoints are prefixed with the version number.

Base URL: `https://api.lurkr.gg/v2`

***

## Authentication

API requests are authenticated using API keys. These keys must be included in the `X-API-Key` header of every request.

### API Key Permissions

* There are read-only and read/write API keys:
  * **Read-only** keys can only fetch data, i.e. `GET` requests.
  * **Read/Write** keys can fetch and modify data, i.e. `GET`, `POST`, `PATCH`, `DELETE` requests.
* By default, API keys have no server access.
* Server access must be explicitly granted. Please note that you must either own the server or have Administrator permissions to grant access.

To create and manage your API keys, visit your [profile page](https://lurkr.gg/profile).

***

## Rate Limiting

The API enforces rate limits to ensure fair usage and system stability. You can make 120 requests per minute per API key.

### Rate Limit Headers

Each response includes the following headers to help you manage your API usage:

| Header                  | Description                                                                            |
| ----------------------- | -------------------------------------------------------------------------------------- |
| `X-RateLimit-Limit`     | Total number of requests allowed per minute                                            |
| `X-RateLimit-Remaining` | Number of requests remaining in the current time window                                |
| `X-RateLimit-Reset`     | Seconds until the rate limit resets                                                    |
| `Retry-After`           | Seconds to wait before making new requests (only included when rate limit is exceeded) |

### Handling Rate Limits

When you hit the rate limit, you’ll receive a `429 Too Many Requests` response. The `Retry-After` header will tell you how long to wait before making new requests.

***

## Error Handling

The API uses standard HTTP status codes to indicate success or failure of requests. All error responses include a JSON body with details about the error.

Example error response:

<pre><code>{    
<strong>    "message": "Invalid API key"
</strong>}
</code></pre>

Common error codes:

* `400`: Bad Request - Invalid parameters
* `401`: Unauthorized - Missing or invalid API key
* `403`: Forbidden - Insufficient permissions
* `404`: Not Found - Resource doesn’t exist
* `429`: Too Many Requests - Rate limit exceeded

***

## API Documentation

For detailed information about available endpoints, parameters, and response formats:

* [Interactive Swagger UI ](https://api.lurkr.gg/v2/docs)
* [OpenAPI Schema ](https://api.lurkr.gg/v2/docs/json)

***

## Best Practices

1. **Keep your API keys secure**
   * Read/Write keys are dangerous and can delete user from your server. Please be mindful when using / sharing them.
   * Rotate keys regularly. You can also set an expiration date when creating a key.
   * Store the keys in a secure location.
2. **Handle errors gracefully**
   * Implement proper error handling
   * Respect rate limits

***

## Final Words

And that's it! You've successfully created an API Key and learned the basic API usage with Lurkr!

If you require any more assistance with Lurkr, check out the rest of this documentation or join our support server to talk to an actual human!

{% embed url="https://lurkr.gg/support" %}

