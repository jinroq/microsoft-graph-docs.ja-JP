# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="9b3f7-101">domainDnsSrvRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b3f7-101">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="9b3f7-p101">テナント内の特定のドメインの DNS ゾーン ファイルに追加された SRV レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-p101">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="9b3f7-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b3f7-104">Methods</span></span>
<span data-ttu-id="9b3f7-p102">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="9b3f7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b3f7-107">Properties</span></span>
| <span data-ttu-id="9b3f7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b3f7-108">Property</span></span>     | <span data-ttu-id="9b3f7-109">タイプ</span><span class="sxs-lookup"><span data-stu-id="9b3f7-109">Type</span></span>   |<span data-ttu-id="9b3f7-110">説明</span><span class="sxs-lookup"><span data-stu-id="9b3f7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b3f7-111">ID</span><span class="sxs-lookup"><span data-stu-id="9b3f7-111">id</span></span>|<span data-ttu-id="9b3f7-112">文字列</span><span class="sxs-lookup"><span data-stu-id="9b3f7-112">String</span></span>| <span data-ttu-id="9b3f7-p103">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="9b3f7-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="9b3f7-115">isOptional</span></span>|<span data-ttu-id="9b3f7-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="9b3f7-116">Boolean</span></span>| <span data-ttu-id="9b3f7-117">False の場合、SRV レコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-117">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="9b3f7-118">ラベル</span><span class="sxs-lookup"><span data-stu-id="9b3f7-118">label</span></span>|<span data-ttu-id="9b3f7-119">文字列</span><span class="sxs-lookup"><span data-stu-id="9b3f7-119">String</span></span>| <span data-ttu-id="9b3f7-120">DNS ホストで SRV レコードの *name* プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-120">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9b3f7-121">nameTarget</span><span class="sxs-lookup"><span data-stu-id="9b3f7-121">nameTarget</span></span>|<span data-ttu-id="9b3f7-122">文字列</span><span class="sxs-lookup"><span data-stu-id="9b3f7-122">String</span></span>| <span data-ttu-id="9b3f7-123">DNS ホストで SRV レコードの *Target* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-123">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9b3f7-124">ポート</span><span class="sxs-lookup"><span data-stu-id="9b3f7-124">port</span></span>|<span data-ttu-id="9b3f7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9b3f7-125">Int32</span></span>| <span data-ttu-id="9b3f7-126">DNS ホストで SRV レコードの *port* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-126">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9b3f7-127">優先度</span><span class="sxs-lookup"><span data-stu-id="9b3f7-127">priority</span></span>|<span data-ttu-id="9b3f7-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9b3f7-128">Int32</span></span>| <span data-ttu-id="9b3f7-129">DNS ホストで SRV レコードの *priority* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-129">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9b3f7-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9b3f7-130">protocol</span></span>|<span data-ttu-id="9b3f7-131">文字列</span><span class="sxs-lookup"><span data-stu-id="9b3f7-131">String</span></span>| <span data-ttu-id="9b3f7-132">DNS ホストで SRV レコードの *protocol* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-132">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9b3f7-133">recordType</span><span class="sxs-lookup"><span data-stu-id="9b3f7-133">recordType</span></span>|<span data-ttu-id="9b3f7-134">文字列</span><span class="sxs-lookup"><span data-stu-id="9b3f7-134">String</span></span>|  <span data-ttu-id="9b3f7-p104">DNS レコードの種類。この値は常に *Srv* です。キー</span><span class="sxs-lookup"><span data-stu-id="9b3f7-p104">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="9b3f7-138">サービス</span><span class="sxs-lookup"><span data-stu-id="9b3f7-138">service</span></span>|<span data-ttu-id="9b3f7-139">文字列</span><span class="sxs-lookup"><span data-stu-id="9b3f7-139">String</span></span>| <span data-ttu-id="9b3f7-140">DNS ホストで SRV レコードの *service* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-140">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="9b3f7-141">supportedService</span><span class="sxs-lookup"><span data-stu-id="9b3f7-141">supportedService</span></span>|<span data-ttu-id="9b3f7-142">文字列</span><span class="sxs-lookup"><span data-stu-id="9b3f7-142">String</span></span>| <span data-ttu-id="9b3f7-143">Microsoft オンライン サービスまたはこの SRV レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-143">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="9b3f7-144">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="9b3f7-144">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="9b3f7-145">ttl</span><span class="sxs-lookup"><span data-stu-id="9b3f7-145">ttl</span></span>|<span data-ttu-id="9b3f7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9b3f7-146">Int32</span></span>| <span data-ttu-id="9b3f7-p105">DNS ホストで SRV レコードの *Time to Live (TTL)* のプロパティを構成するときに使用する値です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="9b3f7-p105">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="9b3f7-149">ウェイト</span><span class="sxs-lookup"><span data-stu-id="9b3f7-149">weight</span></span>|<span data-ttu-id="9b3f7-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9b3f7-150">Int32</span></span>| <span data-ttu-id="9b3f7-151">DNS ホストで SRV レコードの *weight* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-151">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9b3f7-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b3f7-152">Relationships</span></span>
<span data-ttu-id="9b3f7-153">なし</span><span class="sxs-lookup"><span data-stu-id="9b3f7-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9b3f7-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b3f7-154">JSON representation</span></span>
<span data-ttu-id="9b3f7-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b3f7-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
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