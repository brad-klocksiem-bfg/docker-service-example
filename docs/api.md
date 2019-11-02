# API

The following RESTful API endpoints are available:

| Method | EndPoint | Description                                    |
|------|---------|---------------------------------------------------|
| GET  | /       | Returns index of all commands                     |
| POST | /create | Creates a new entry, requires content, returns id |
| POST | /delete | Deletes an entry, required id                     |
| POST | /modify | Modifies an entry, requires id and content        |

Payloads should contain the following:

```json
{
    "id": INT,
    "content": STR
}
```

# Integration