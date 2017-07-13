<span data-ttu-id="e4313-p122">メッセージに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e4313-p122">The collection of single-value extended properties defined for the message. Read-only. Nullable.</span></span>| メッセージに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|


## <span data-ttu-id="e4313-330">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4313-330">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="e4313-331">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e4313-331">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```

## <span data-ttu-id="e4313-332">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4313-332">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="e4313-333">メールボックス設定を取得する</span><span class="sxs-lookup"><span data-stu-id="e4313-333">Get mailbox settings</span></span>](../api/user_get_mailboxsettings.md) 
- [<span data-ttu-id="e4313-334">メールボックス設定を更新する</span><span class="sxs-lookup"><span data-stu-id="e4313-334">Update mailbox settings</span></span>](../api/user_update_mailboxsettings.md)
- [<span data-ttu-id="e4313-335">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="e4313-335">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="e4313-336">フォルダー内のメッセージへの増分変更を取得する</span><span class="sxs-lookup"><span data-stu-id="e4313-336">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)
- [<span data-ttu-id="e4313-337">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="e4313-337">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e4313-338">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="e4313-338">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="e4313-339">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="e4313-339">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
