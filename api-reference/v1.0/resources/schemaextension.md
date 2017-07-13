<span data-ttu-id="817cf-p106">スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。**contact**、**device**、**event**、**group**、**message**、**organization**、**post**、**user** のいずれかから選択します。</span><span class="sxs-lookup"><span data-stu-id="817cf-p106">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to. Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。**contact**、**device**、**event**、**group**、**message**、**organization**、**post**、**user** のいずれかから選択します。|

## <span data-ttu-id="817cf-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="817cf-166">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="817cf-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="817cf-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->