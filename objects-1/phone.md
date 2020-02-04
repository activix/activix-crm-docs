# Phone

The representation of a phone is called a `Phone` object. Phones are identified by a unique incremental ID. Each `Lead` can only have one `Phone` of each type.

## The `Phone` Object

| **Attribute** | **Type** | **Description** |
| :--- | :--- | :--- |
| `id` | integer | Unique identifier for the phone. |
| `lead_id` | integer | ID of the lead associated with the phone. |
|  |  |  |
| `created_at` | string | [ISO datetime](https://en.wikipedia.org/wiki/ISO_8601) representing when the phone was created. |
| `updated_at` | string | [ISO datetime](https://en.wikipedia.org/wiki/ISO_8601) representing when the phone was last updated. |
|  |  |  |
| `extension` | integer | Extension of the phone. |
| `number` | string | Phone number in [E.164](https://www.twilio.com/docs/glossary/what-e164) format. |
| `type` | boolean | The type of phone. Possible values are **home**, **work** or **mobile**.  |
| `valid` | boolean | Determines if the phone number is valid _\(read only\)_. |
