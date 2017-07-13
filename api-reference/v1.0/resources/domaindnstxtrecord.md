<span data-ttu-id="02912-p105">DNS ホストで MX レコードの *Time To Live (ttl)* プロパティを設定するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="02912-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span>| DNS ホストで MX レコードの *Time To Live (ttl)* プロパティを設定するときに使用する値。null 許容ではありません |

## <span data-ttu-id="02912-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="02912-137">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="02912-138">なし</span><span class="sxs-lookup"><span data-stu-id="02912-138">None</span></span>


## <span data-ttu-id="02912-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02912-139">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="02912-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="02912-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->