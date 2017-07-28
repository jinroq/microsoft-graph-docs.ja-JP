<span data-ttu-id="7c983-p103">サービス プランを割り当てることができるオブジェクト。可能な値:</span><span class="sxs-lookup"><span data-stu-id="7c983-p103">The object the service plan can be assigned to. Possible values:</span></span>|サービス プランを割り当てることができるオブジェクト。可能な値:<br/><span data-ttu-id="7c983-127">User - サービス プランを個別のユーザーに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="7c983-127">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="7c983-128">Company - サービス プランをテナント全体に割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="7c983-128">"Company" - service plan can be assigned to the entire tenant.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7c983-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7c983-129">JSON representation</span></span>

<span data-ttu-id="7c983-130">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7c983-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
