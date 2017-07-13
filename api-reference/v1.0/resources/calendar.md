<span data-ttu-id="60a40-p111">予定表に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="60a40-p111">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>| 予定表に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|

## <span data-ttu-id="60a40-206">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60a40-206">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="60a40-207">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="60a40-207">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
