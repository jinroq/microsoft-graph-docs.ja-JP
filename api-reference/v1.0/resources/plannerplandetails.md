<span data-ttu-id="41eb0-p103">この計画を共有するユーザー ID を設定します。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。</span><span class="sxs-lookup"><span data-stu-id="41eb0-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|この計画を共有するユーザー ID を設定します。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。 |

## <span data-ttu-id="41eb0-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41eb0-132">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="41eb0-133">なし</span><span class="sxs-lookup"><span data-stu-id="41eb0-133">None</span></span>


## <span data-ttu-id="41eb0-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41eb0-134">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="41eb0-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="41eb0-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->