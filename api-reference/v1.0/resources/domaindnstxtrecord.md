# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="8bfb2-101">domainDnsTxtRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8bfb2-101">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="8bfb2-p101">テナント内の特定のドメインの DNS ゾーン ファイルに追加された TXT レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="8bfb2-p101">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="8bfb2-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="8bfb2-104">Methods</span></span>
<span data-ttu-id="8bfb2-p102">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bfb2-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8bfb2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bfb2-107">Properties</span></span>
| <span data-ttu-id="8bfb2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bfb2-108">Property</span></span>     | <span data-ttu-id="8bfb2-109">タイプ</span><span class="sxs-lookup"><span data-stu-id="8bfb2-109">Type</span></span>   |<span data-ttu-id="8bfb2-110">説明</span><span class="sxs-lookup"><span data-stu-id="8bfb2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bfb2-111">id</span><span class="sxs-lookup"><span data-stu-id="8bfb2-111">id</span></span>|<span data-ttu-id="8bfb2-112">文字列</span><span class="sxs-lookup"><span data-stu-id="8bfb2-112">String</span></span>| <span data-ttu-id="8bfb2-p103">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8bfb2-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="8bfb2-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="8bfb2-115">isOptional</span></span>|<span data-ttu-id="8bfb2-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="8bfb2-116">Boolean</span></span>| <span data-ttu-id="8bfb2-117">false の場合、ドメインが指定された Microsoft Online Services が適切に機能するには、TXT レコードが DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8bfb2-117">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="8bfb2-118">label</span><span class="sxs-lookup"><span data-stu-id="8bfb2-118">label</span></span>|<span data-ttu-id="8bfb2-119">文字列</span><span class="sxs-lookup"><span data-stu-id="8bfb2-119">String</span></span>| <span data-ttu-id="8bfb2-120">DNS ホストで TXT レコードの *name* プロパティを構成する場合に使用する値。</span><span class="sxs-lookup"><span data-stu-id="8bfb2-120">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="8bfb2-121">recordType</span><span class="sxs-lookup"><span data-stu-id="8bfb2-121">recordType</span></span>|<span data-ttu-id="8bfb2-122">文字列</span><span class="sxs-lookup"><span data-stu-id="8bfb2-122">String</span></span>| <span data-ttu-id="8bfb2-p104">DNS レコードの種類。この値は常に *Txt* です。キー</span><span class="sxs-lookup"><span data-stu-id="8bfb2-p104">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="8bfb2-126">supportedService</span><span class="sxs-lookup"><span data-stu-id="8bfb2-126">supportedService</span></span>|<span data-ttu-id="8bfb2-127">文字列</span><span class="sxs-lookup"><span data-stu-id="8bfb2-127">String</span></span>| <span data-ttu-id="8bfb2-128">Microsoft オンライン サービスまたはこの TXT レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="8bfb2-128">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="8bfb2-129">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="8bfb2-129">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="8bfb2-130">text</span><span class="sxs-lookup"><span data-stu-id="8bfb2-130">text</span></span>|<span data-ttu-id="8bfb2-131">文字列</span><span class="sxs-lookup"><span data-stu-id="8bfb2-131">String</span></span>| <span data-ttu-id="8bfb2-132">DNS ホストで *text* プロパティを設定するときに使用する値。</span><span class="sxs-lookup"><span data-stu-id="8bfb2-132">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="8bfb2-133">ttl</span><span class="sxs-lookup"><span data-stu-id="8bfb2-133">ttl</span></span>|<span data-ttu-id="8bfb2-134">Int32</span><span class="sxs-lookup"><span data-stu-id="8bfb2-134">Int32</span></span>| <span data-ttu-id="8bfb2-p105">DNS ホストで MX レコードの *Time To Live (ttl)* プロパティを設定するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="8bfb2-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="8bfb2-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8bfb2-137">Relationships</span></span>
<span data-ttu-id="8bfb2-138">なし</span><span class="sxs-lookup"><span data-stu-id="8bfb2-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8bfb2-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8bfb2-139">JSON representation</span></span>
<span data-ttu-id="8bfb2-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8bfb2-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
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