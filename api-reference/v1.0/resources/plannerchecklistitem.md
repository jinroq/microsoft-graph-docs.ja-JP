<span data-ttu-id="f5e01-p104">チェックリストでの項目の相対順序を設定するのに使用します。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="f5e01-p104">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|チェックリストでの項目の相対順序を設定するのに使用します。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。|
|<span data-ttu-id="f5e01-125">title</span><span class="sxs-lookup"><span data-stu-id="f5e01-125">title</span></span>|<span data-ttu-id="f5e01-126">String</span><span class="sxs-lookup"><span data-stu-id="f5e01-126">String</span></span>|<span data-ttu-id="f5e01-127">チェックリスト項目のタイトル</span><span class="sxs-lookup"><span data-stu-id="f5e01-127">Title of the checklist item</span></span>|

## <span data-ttu-id="f5e01-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5e01-128">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="f5e01-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5e01-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->