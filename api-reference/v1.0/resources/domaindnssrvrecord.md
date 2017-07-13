<span data-ttu-id="834b6-p105">DNS ホストで SRV レコードの *Time to Live (TTL)* のプロパティを構成するときに使用する値です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="834b6-p105">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span>| DNS ホストで SRV レコードの *Time to Live (TTL)* のプロパティを構成するときに使用する値です。null 許容ではありません |
|<span data-ttu-id="834b6-149">weight</span><span class="sxs-lookup"><span data-stu-id="834b6-149">weight</span></span>|<span data-ttu-id="834b6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="834b6-150">Int32</span></span>| <span data-ttu-id="834b6-151">DNS ホストで SRV レコードの *weight* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="834b6-151">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <span data-ttu-id="834b6-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="834b6-152">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="834b6-153">なし</span><span class="sxs-lookup"><span data-stu-id="834b6-153">None</span></span>


## <span data-ttu-id="834b6-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="834b6-154">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="834b6-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="834b6-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->