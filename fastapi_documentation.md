
# FastAPI Documentation

Version: 0.1.0  
OAS: 3.1

## Servers

- `/api`

### POST /make_toingg/

**Make Toingg**

#### Parameters

- `apiKey*`: string (query)

#### Request Body

- Content-Type: application/json

```json
{
  "campaign": "string",
  "name": "string",
  "phoneNumber": "string"
}
```

#### Responses

- **200**: Successful Response
  - Content-Type: application/json
  - Example Value: `"string"`
  
- **422**: Validation Error
  - Content-Type: application/json
  - Example Value:
    ```json
    {
      "detail": [
        {
          "loc": ["string", 0],
          "msg": "string",
          "type": "string"
        }
      ]
    }
    ```

### POST /make_batch_toingg/

**Make Batch Toingg**

#### Parameters

- `apiKey*`: string (query)

#### Request Body

- Content-Type: application/json

```json
{
  "campaign": "string",
  "numberList": {}
}
```

#### Responses

- **200**: Successful Response
  - Content-Type: application/json
  - Example Value: `"string"`
  
- **422**: Validation Error
  - Content-Type: application/json
  - Example Value:
    ```json
    {
      "detail": [
        {
          "loc": ["string", 0],
          "msg": "string",
          "type": "string"
        }
      ]
    }
    ```

### POST /send_sms/

**Send SMS**

#### Parameters

- `apiKey*`: string (query)

#### Request Body

- Content-Type: application/json

```json
{
  "name": "string",
  "phoneNumber": "string",
  "message": "string"
}
```

#### Responses

- **200**: Successful Response
  - Content-Type: application/json
  - Example Value: `"string"`
  
- **422**: Validation Error
  - Content-Type: application/json
  - Example Value:
    ```json
    {
      "detail": [
        {
          "loc": ["string", 0],
          "msg": "string",
          "type": "string"
        }
      ]
    }
    ```

### POST /hang_up_call/

**Hang Up Call**

#### Parameters

- `callSid*`: string (query)
- `apiKey*`: string (query)

#### Responses

- **200**: Successful Response
  - Content-Type: application/json
  - Example Value: `"string"`
  
- **422**: Validation Error
  - Content-Type: application/json
  - Example Value:
    ```json
    {
      "detail": [
        {
          "loc": ["string", 0],
          "msg": "string",
          "type": "string"
        }
      ]
    }
    ```

### POST /create-checkout-session/

**Create Checkout Session**

#### Request Body

- Content-Type: application/json

```json
{
  "apikey": "string"
}
```

#### Responses

- **200**: Successful Response
  - Content-Type: application/json
  - Example Value: `"string"`
  
- **422**: Validation Error
  - Content-Type: application/json
  - Example Value:
    ```json
    {
      "detail": [
        {
          "loc": ["string", 0],
          "msg": "string",
          "type": "string"
        }
      ]
    }
    ```

### POST /webhook/

**Stripe Webhook**

#### Responses

- **200**: Successful Response
  - Content-Type: application/json
  - Example Value: `"string"`
```

You can save this content into a Markdown file (e.g., `fastapi_documentation.md`) and use it for your documentation purposes.
