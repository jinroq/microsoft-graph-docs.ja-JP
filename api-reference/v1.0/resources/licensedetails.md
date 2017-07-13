<span data-ttu-id="b1c30-p104">一意の SKU 表示名です。関連する [SubscribedSku](subscribedsku.md) オブジェクトの skuPartNumber と同じです。例: "AAD_Premium"。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="b1c30-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span>| 一意の SKU 表示名です。関連する [SubscribedSku](subscribedsku.md) オブジェクトの skuPartNumber と同じです。例: "AAD_Premium"。読み取り専用 |

## <span data-ttu-id="b1c30-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b1c30-132">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="b1c30-133">なし</span><span class="sxs-lookup"><span data-stu-id="b1c30-133">None</span></span>

## <span data-ttu-id="b1c30-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1c30-134">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="b1c30-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b1c30-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->