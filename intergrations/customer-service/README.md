# Customer Service

## Version: 1

---

## POST /contacts/search

### Summary

Get a list of contacts for given filters.

---

### Request Parameters

| Name  | Located In | Description     | Required | Schema |
|------|-----------|----------------|----------|--------|
| Input | Payload   | Contact filters | Optional      | ```json
{
  "email": "user@wso2.com"
}
``` |

---

### Responses

#### ✅ 200 OK

**Description:** Successful response.

**Body**

```json
[
  {
    "id": "C001",
    "email": "user@wso2.com",
    "account": {
      "id": "A101"
    }
  },
  {
    "id": "C002",
    "email": "jane@wso2.com",
    "account": null
  }
]
