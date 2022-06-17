## Clearout Instant Email Verification cURL API V1

Instant verification API can be seamlessly integrated into your signup or onboarding process with just a single request. Use this API to verify Email Address without going through queue.

### POST
```
https://api.clearout.io/v2/email_verify/instant
```

### cURL
```curl
curl -X POST 'https://api.clearout.io/v2/email_verify/instant' \
-H 'Authorization: REPLACE_WITH_YOUR_API_TOKEN' \
-H 'Content-Type: application/json' \
-d '{ "email": "us@clearout.io" }'
```

#### Header
| **Field**         | **Type**          | **Description**                              |
| :-------------    | :-------------:   | :-----                                       |
| Content-Type      | String            | Default value: application/json              |
| Authorization     | String            | Default value: REPLACE_WITH_YOUR_API_TOKEN   |

#### Parameter
| **Field**           | **Type**          | **Description**                                                        |
| :-------------      | :-------------:   | :-----                                                                 |
| email               | String            | An email address to verify                                             |
| timeout `optional`  | Number            | Request wait time (in milliseconds), Maximum allowed wait time should not exceed **180,000 milliseconds** Default value: 130,000|   
