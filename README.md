# Scalable URL Shortener service (Spec Driven AI assisted Prototype)

A scalable URL shortening platform that converts long URLs into compact, shareable links while providing analytics and reliable redirection.

## Features

- Shorten long URLs
- Redirect users to original URLs
- Track click analytics
- Persistent URL storage
- Scalable and cloud-ready architecture

## Tech Stack

- Python (FastAPI)
- PostgreSQL
- SQLAlchemy
- Pytest
- Docker

## API Endpoints

| Method | Endpoint | Description |
|----------|----------|-------------|
| POST | `/api/v1/urls` | Create short URL |
| GET | `/{shortCode}` | Redirect to original URL |
| GET | `/api/v1/analytics/{shortCode}` | Retrieve analytics |

## Example

**Request**

```json
{
  "url": "https://www.example.com"
}
```

**Response**

```json
{
  "shortCode": "aB12Cd",
  "shortUrl": "https://short.ly/aB12Cd"
}
```

## Project Goals

- Low-latency redirects
- High availability
- Horizontal scalability
- Reliable analytics
- Clean and maintainable codebase

## Project Structure

```text
src/
├── api/
├── services/
├── models/
├── repositories/
└── tests/
```

## Roadmap

- [ ] URL shortening API
- [ ] Redirect service
- [ ] Analytics tracking
- [ ] Redis caching
- [ ] Docker support
- [ ] CI/CD pipeline

## License

MIT License
