<span data-ttu-id="cfabf-p104">タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="cfabf-p104">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。|

## <span data-ttu-id="cfabf-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cfabf-133">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="cfabf-134">なし</span><span class="sxs-lookup"><span data-stu-id="cfabf-134">None</span></span>


## <span data-ttu-id="cfabf-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cfabf-135">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="cfabf-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cfabf-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->