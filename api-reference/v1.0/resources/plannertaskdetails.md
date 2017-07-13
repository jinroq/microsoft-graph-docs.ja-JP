<span data-ttu-id="290d7-p103">タスクに表示されるプレビューの種類を設定します。使用可能な値: `automatic`、`noPreview`、`checklist`、`description`、`reference`。`automatic` に設定すると、タスクを表示しているアプリによって表示するプレビューが選択されます。</span><span class="sxs-lookup"><span data-stu-id="290d7-p103">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|タスクに表示されるプレビューの種類を設定します。使用可能な値: `automatic`、`noPreview`、`checklist`、`description`、`reference`。`automatic` に設定すると、タスクを表示しているアプリによって表示するプレビューが選択されます。|
|<span data-ttu-id="290d7-135">references</span><span class="sxs-lookup"><span data-stu-id="290d7-135">references</span></span>|[<span data-ttu-id="290d7-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="290d7-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="290d7-137">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="290d7-137">The collection of references on the task.</span></span>|

## <span data-ttu-id="290d7-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="290d7-138">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="290d7-139">なし</span><span class="sxs-lookup"><span data-stu-id="290d7-139">None</span></span>


## <span data-ttu-id="290d7-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="290d7-140">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="290d7-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="290d7-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->