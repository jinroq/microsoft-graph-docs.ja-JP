<span data-ttu-id="b087d-p107">mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b087d-p107">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>| mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|


## <span data-ttu-id="b087d-200">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b087d-200">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="b087d-201">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b087d-201">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,

  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```

## <span data-ttu-id="b087d-202">関連項目</span><span class="sxs-lookup"><span data-stu-id="b087d-202">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="b087d-203">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="b087d-203">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="b087d-204">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="b087d-204">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
