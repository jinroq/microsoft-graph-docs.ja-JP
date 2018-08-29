# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="f70e6-101">plannerOrderHintsByAssignee リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f70e6-101">plannerOrderHintsByAssignee resource type</span></span>

<span data-ttu-id="f70e6-p101">**plannerOrderHintsByAssignee** には、タスク ボードの [割り当て先ユーザー/グループ] ビューのタスクの順序を示す、[plannerTask](plannerTask.md) リソースの担当者の[順序に関するヒント](planner_order_hint_format.md)が含まれます。この型はオープン型です。プロパティは、タスクに割り当てられているユーザーの ID で、値は順序のヒントです。</span><span class="sxs-lookup"><span data-stu-id="f70e6-p101">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner_order_hint_format.md) for assignees in a [plannerTask](plannerTask.md) resource, to indicate the order of the task in Assigned To view of the Task Board. This type is an open type. The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="f70e6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f70e6-105">Properties</span></span>
<span data-ttu-id="f70e6-p102">クライアントは、オープン型のプロパティを定義できます。この場合、クライアントは、タスクに割り当てられているユーザーの ID をプロパティ名として指定し、有効な[順序のヒント](planner_order_hint_format.md)を値として指定する必要があります。プロパティは、この型から削除できません。サービスは、含まれている [plannerTask](plannerTask.md) の割り当てが更新されると、値を自動的に削除します</span><span class="sxs-lookup"><span data-stu-id="f70e6-p102">Properties of an Open Type can be defined by the client. In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner_order_hint_format.md) as the value. Properties cannot be removed from this type. The service will automatically remove values as the assignments on the containing [plannerTask](plannerTask.md) are updated.</span></span>

<span data-ttu-id="f70e6-110">例:</span><span class="sxs-lookup"><span data-stu-id="f70e6-110">Example:</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->