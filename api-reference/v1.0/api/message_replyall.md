# message: replyAll

Reply to all recipients of a message. The message is then saved in the Sent Items folder.

## Prerequisites
One of the following **scopes** is required to execute this API:
*Mail.Send*
## HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/<id>/replyAll
POST /users/<id | userPrincipalName>/messages/<id>/replyAll
POST /me/mailFolders/<id>/messages/<id>/replyAll
POST /users/<id | userPrincipalName>/mailFolders/<id>/messages/<id>/replyAll
```
## Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer <token>. Required. |
| Content-Type | string  | Nature of the data in the body of an entity. Required. |

## Request body
In the request body, provide a JSON object with the following parameters.

| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|
|comment|String|A comment to include. Can be an empty string.|

## Response
If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.

## Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/<id>/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```


##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
