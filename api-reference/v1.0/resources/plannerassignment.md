<span data-ttu-id="8076c-p103">タスクの担当者を並べ替えるために使用するヒント。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="8076c-p103">Hint used to order assignees in a task. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|タスクの担当者を並べ替えるために使用するヒント。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。|

## <span data-ttu-id="8076c-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8076c-120">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="8076c-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8076c-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->