<span data-ttu-id="24556-p107">DNS ホストで CNAME レコードの Time To Live (TTL) のプロパティを構成するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="24556-p107">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span>| DNS ホストで CNAME レコードの Time To Live (TTL) のプロパティを構成するときに使用する値。null 許容ではありません |

## <span data-ttu-id="24556-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24556-139">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="24556-140">なし</span><span class="sxs-lookup"><span data-stu-id="24556-140">None</span></span>


## <span data-ttu-id="24556-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24556-141">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="24556-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24556-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->