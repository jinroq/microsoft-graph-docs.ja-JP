# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="e8a59-101">domainDnsMxRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8a59-101">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="e8a59-p101">テナント内の特定のドメインの DNS ゾーン ファイルに追加された MX レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="e8a59-p101">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="e8a59-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8a59-104">Methods</span></span>
<span data-ttu-id="e8a59-p102">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8a59-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="e8a59-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8a59-107">Properties</span></span>
| <span data-ttu-id="e8a59-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8a59-108">Property</span></span>     | <span data-ttu-id="e8a59-109">タイプ</span><span class="sxs-lookup"><span data-stu-id="e8a59-109">Type</span></span>   |<span data-ttu-id="e8a59-110">説明</span><span class="sxs-lookup"><span data-stu-id="e8a59-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8a59-111">id</span><span class="sxs-lookup"><span data-stu-id="e8a59-111">id</span></span>|<span data-ttu-id="e8a59-112">String</span><span class="sxs-lookup"><span data-stu-id="e8a59-112">String</span></span>| <span data-ttu-id="e8a59-p103">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e8a59-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="e8a59-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="e8a59-115">isOptional</span></span>|<span data-ttu-id="e8a59-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8a59-116">Boolean</span></span>| <span data-ttu-id="e8a59-117">False の場合、MX レコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8a59-117">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="e8a59-118">label</span><span class="sxs-lookup"><span data-stu-id="e8a59-118">label</span></span>|<span data-ttu-id="e8a59-119">String</span><span class="sxs-lookup"><span data-stu-id="e8a59-119">String</span></span>| <span data-ttu-id="e8a59-120">DNS ホストで MX レコードの *alias/host/name* プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="e8a59-120">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="e8a59-121">mailExchange</span><span class="sxs-lookup"><span data-stu-id="e8a59-121">mailExchange</span></span>|<span data-ttu-id="e8a59-122">String</span><span class="sxs-lookup"><span data-stu-id="e8a59-122">String</span></span>| <span data-ttu-id="e8a59-123">DNS ホストで MX レコードの *answer/destination/value* を構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="e8a59-123">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="e8a59-124">preference</span><span class="sxs-lookup"><span data-stu-id="e8a59-124">preference</span></span>|<span data-ttu-id="e8a59-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e8a59-125">Int32</span></span>| <span data-ttu-id="e8a59-126">DNS ホストで MX レコードの *Preference/Priority* プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="e8a59-126">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="e8a59-127">recordType</span><span class="sxs-lookup"><span data-stu-id="e8a59-127">recordType</span></span>|<span data-ttu-id="e8a59-128">String</span><span class="sxs-lookup"><span data-stu-id="e8a59-128">String</span></span>| <span data-ttu-id="e8a59-p104">DNS レコードの種類。この値は常に *Mx* です。キー</span><span class="sxs-lookup"><span data-stu-id="e8a59-p104">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="e8a59-132">supportedService</span><span class="sxs-lookup"><span data-stu-id="e8a59-132">supportedService</span></span>|<span data-ttu-id="e8a59-133">String</span><span class="sxs-lookup"><span data-stu-id="e8a59-133">String</span></span>| <span data-ttu-id="e8a59-134">Microsoft オンライン サービスまたはこの MX レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="e8a59-134">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="e8a59-135">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="e8a59-135">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="e8a59-136">ttl</span><span class="sxs-lookup"><span data-stu-id="e8a59-136">ttl</span></span>|<span data-ttu-id="e8a59-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e8a59-137">Int32</span></span>| <span data-ttu-id="e8a59-p105">DNS ホストで MX レコードの *Time To Live (ttl)* プロパティを設定するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="e8a59-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="e8a59-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8a59-140">Relationships</span></span>
<span data-ttu-id="e8a59-141">なし</span><span class="sxs-lookup"><span data-stu-id="e8a59-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8a59-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8a59-142">JSON representation</span></span>
<span data-ttu-id="e8a59-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8a59-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->