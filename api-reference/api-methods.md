# API Methods

## Api.sendMessage

{% code lineNumbers="true" fullWidth="false" %}
```javascript
Api.sendMessage({
    "text": "<b>Hello World</b>",
    "parse_mode": "HTML",
    "reply_markp": {
        "inline_keyboard": [
            [{"text": "Our Channel","url":"https://t.me/botsbus"}]
        ]
    }
})    
```
{% endcode %}

<table><thead><tr><th width="198">Parameter</th><th>Type</th><th width="155">Required</th><th>Description</th></tr></thead><tbody><tr><td>chat_id</td><td>Integer or String</td><td>Optional</td><td>Unique identifier for the target chat or username of the target channel (in the format <code>@channelusername</code>)</td></tr><tr><td>message_thread_id</td><td>Integer</td><td>Optional</td><td>Unique identifier for the target message thread (topic) of the forum; for forum supergroups only</td></tr><tr><td>text</td><td>String</td><td>Yes</td><td>Text of the message to be sent, 1-4096 characters after entities parsing</td></tr><tr><td>parse_mode</td><td>String</td><td>Optional</td><td>Mode for parsing entities in the message text. See <a href="https://core.telegram.org/bots/api#formatting-options">formatting options</a> for more details.</td></tr><tr><td>entities</td><td>Array of <a href="https://core.telegram.org/bots/api#messageentity">MessageEntity</a></td><td>Optional</td><td>A JSON-serialized list of special entities that appear in message text, which can be specified instead of <em>parse_mode</em></td></tr><tr><td>disable_web_page_preview</td><td>Boolean</td><td>Optional</td><td>Disables link previews for links in this message</td></tr><tr><td>disable_notification</td><td>Boolean</td><td>Optional</td><td>Sends the message <a href="https://telegram.org/blog/channels-2-0#silent-messages">silently</a>. Users will receive a notification with no sound.</td></tr><tr><td>protect_content</td><td>Boolean</td><td>Optional</td><td>Protects the contents of the sent message from forwarding and saving</td></tr><tr><td>reply_to_message_id</td><td>Integer</td><td>Optional</td><td>If the message is a reply, ID of the original message</td></tr><tr><td>allow_sending_without_reply</td><td>Boolean</td><td>Optional</td><td>Pass <em>True</em> if the message should be sent even if the specified replied-to message is not found</td></tr><tr><td>reply_markup</td><td><a href="https://core.telegram.org/bots/api#inlinekeyboardmarkup">InlineKeyboardMarkup</a> or <a href="https://core.telegram.org/bots/api#replykeyboardmarkup">ReplyKeyboardMarkup</a> or <a href="https://core.telegram.org/bots/api#replykeyboardremove">ReplyKeyboardRemove</a> or <a href="https://core.telegram.org/bots/api#forcereply">ForceReply</a></td><td>Optional</td><td>Additional interface options. A JSON-serialized object for an <a href="https://core.telegram.org/bots/features#inline-keyboards">inline keyboard</a>, <a href="https://core.telegram.org/bots/features#keyboards">custom reply keyboard</a>, instructions to remove reply keyboard or to force a reply from the user.</td></tr></tbody></table>
