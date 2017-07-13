<span data-ttu-id="1c474-p108">招待状作成の一環として作成されたユーザー。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="1c474-p108">The user created as part of the invitation creation. Read-Only</span></span>|招待状作成の一環として作成されたユーザー。読み取り専用|

## <span data-ttu-id="1c474-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1c474-165">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="1c474-166">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1c474-166">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.invitations" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",

  "invitedUser": [{"@odata.type": "microsoft.graph.user"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
