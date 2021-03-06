# Contact Channels Object

Field | Data Type | Description
--- | --- | ---
id | string | Unique identifier
display_name | string | One of HOME, BUSINESS, or MOBILE.  Can be null, even when channel is a phone number.
value | string | Uniquely identifying value of the channel. For example, for channels with type 'Phone Number' this would be the actual phone number
formatted_value | string | Locally-formatted version of the value string
country | string | ISO 3166-1 alpha-2 country code
is_default | boolean | Whether this channel is the global default for this Contact
is_default_for_type | boolean | Whether this channel is the default for its type for this Contact
block_inbound | boolean | Whether this channel is blocked from inbound messages
block_outbound | boolean | Whether this channel is blocked from outbound messages
channel_type | object | [Channel Type]

[Channel Type]: /channel_types/README.md
