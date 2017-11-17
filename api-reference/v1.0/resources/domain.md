<span data-ttu-id="0f258-p114">検証レコードやサービス構成のレコードなど、ディレクトリ内のドメインと他のオブジェクト間のリレーションシップは、ナビゲーション プロパティを介して公開されます。要求でこれらのナビゲーション プロパティを対象にすれば、そのリレーションシップを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="0f258-p114">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties. You can read these relationships by targeting these navigation properties in your requests.</span></span>

検証レコードやサービス構成のレコードなど、ディレクトリ内のドメインと他のオブジェクト間のリレーションシップは、ナビゲーション プロパティを介して公開されます。要求でこれらのナビゲーション プロパティを対象にすれば、そのリレーションシップを読み取ることができます。

| <span data-ttu-id="0f258-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0f258-199">Relationship</span></span> | <span data-ttu-id="0f258-200">型</span><span class="sxs-lookup"><span data-stu-id="0f258-200">Type</span></span> |<span data-ttu-id="0f258-201">説明</span><span class="sxs-lookup"><span data-stu-id="0f258-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f258-202">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="0f258-202">domainNameReferences</span></span>|<span data-ttu-id="0f258-203">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="0f258-203">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="0f258-204">読み取り専用、Null 許容型</span><span class="sxs-lookup"><span data-stu-id="0f258-204">Read-only, Nullable</span></span>|
|<span data-ttu-id="0f258-205">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="0f258-205">serviceConfigurationRecords</span></span>|<span data-ttu-id="0f258-206">[domainDnsRecord](domaindnsrecord.md) collection</span><span class="sxs-lookup"><span data-stu-id="0f258-206">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="0f258-207">ドメインを Microsoft Online Services で使用する前に、顧客がそのドメインの DNS ゾーン ファイルに追加する DNS レコードです。</span><span class="sxs-lookup"><span data-stu-id="0f258-207">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="0f258-208">読み取り専用、Null 許容型</span><span class="sxs-lookup"><span data-stu-id="0f258-208">Read-only, Nullable</span></span> |
|<span data-ttu-id="0f258-209">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="0f258-209">verificationDnsRecords</span></span>|<span data-ttu-id="0f258-210">[domainDnsRecord](domaindnsrecord.md) collection</span><span class="sxs-lookup"><span data-stu-id="0f258-210">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="0f258-211">顧客が Azure AD のドメイン所有権の確認を完了する前に、顧客がそのドメインの DNS ゾーン ファイルに追加する DNS レコード。</span><span class="sxs-lookup"><span data-stu-id="0f258-211">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="0f258-212">読み取り専用、Null 許容型</span><span class="sxs-lookup"><span data-stu-id="0f258-212">Read-only, Nullable</span></span>|

## <span data-ttu-id="0f258-213">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f258-213">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="0f258-214">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f258-214">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->