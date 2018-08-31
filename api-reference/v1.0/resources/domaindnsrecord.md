# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="dfda4-101">domainDnsRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfda4-101">domainDnsRecord resource type</span></span>

<span data-ttu-id="dfda4-p101">テナント内の各ドメインでは、Microsoft オンライン サービスでドメインを使用できるようにするために、DNS レコードをそのドメインの DNS ゾーン ファイルに追加しなければならない場合があります。**DomainDnsRecord** エンティティはこのような DNS レコードの表示に使用されます。[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) エンティティのベース エンティティ。</span><span class="sxs-lookup"><span data-stu-id="dfda4-p101">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="dfda4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="dfda4-105">Methods</span></span>
<span data-ttu-id="dfda4-p102">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="dfda4-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="dfda4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfda4-108">Properties</span></span>
| <span data-ttu-id="dfda4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfda4-109">Property</span></span>     | <span data-ttu-id="dfda4-110">タイプ</span><span class="sxs-lookup"><span data-stu-id="dfda4-110">Type</span></span>   |<span data-ttu-id="dfda4-111">説明</span><span class="sxs-lookup"><span data-stu-id="dfda4-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfda4-112">ID</span><span class="sxs-lookup"><span data-stu-id="dfda4-112">id</span></span>|<span data-ttu-id="dfda4-113">文字列</span><span class="sxs-lookup"><span data-stu-id="dfda4-113">String</span></span>| <span data-ttu-id="dfda4-p103">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dfda4-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="dfda4-116">isOptional</span><span class="sxs-lookup"><span data-stu-id="dfda4-116">isOptional</span></span>|<span data-ttu-id="dfda4-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="dfda4-117">Boolean</span></span>| <span data-ttu-id="dfda4-118">False の場合、このレコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dfda4-118">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="dfda4-119">ラベル</span><span class="sxs-lookup"><span data-stu-id="dfda4-119">label</span></span>|<span data-ttu-id="dfda4-120">文字列</span><span class="sxs-lookup"><span data-stu-id="dfda4-120">String</span></span>| <span data-ttu-id="dfda4-121">DNS ホストで DNS レコードの名前を設定するときに使用する値。</span><span class="sxs-lookup"><span data-stu-id="dfda4-121">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="dfda4-122">recordType</span><span class="sxs-lookup"><span data-stu-id="dfda4-122">recordType</span></span>|<span data-ttu-id="dfda4-123">文字列</span><span class="sxs-lookup"><span data-stu-id="dfda4-123">String</span></span>| <span data-ttu-id="dfda4-124">このエンティティが表す DNS レコードの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="dfda4-124">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="dfda4-125">値は次のいずれかを指定できます。*CName*、*Mx*、*Srv*、*Txt*</span><span class="sxs-lookup"><span data-stu-id="dfda4-125">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="dfda4-126">キー</span><span class="sxs-lookup"><span data-stu-id="dfda4-126">Key</span></span> |
|<span data-ttu-id="dfda4-127">supportedService</span><span class="sxs-lookup"><span data-stu-id="dfda4-127">supportedService</span></span>|<span data-ttu-id="dfda4-128">文字列</span><span class="sxs-lookup"><span data-stu-id="dfda4-128">String</span></span>| <span data-ttu-id="dfda4-129">Microsoft オンライン サービスまたはこの DNS レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="dfda4-129">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="dfda4-130">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="dfda4-130">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="dfda4-131">ttl</span><span class="sxs-lookup"><span data-stu-id="dfda4-131">ttl</span></span>|<span data-ttu-id="dfda4-132">Int32</span><span class="sxs-lookup"><span data-stu-id="dfda4-132">Int32</span></span>| <span data-ttu-id="dfda4-p104">DNS ホストの DNS レコードの Time to Live (TTL) のプロパティを構成するときに使用する値です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="dfda4-p104">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="dfda4-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dfda4-135">Relationships</span></span>
<span data-ttu-id="dfda4-136">なし</span><span class="sxs-lookup"><span data-stu-id="dfda4-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfda4-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfda4-137">JSON representation</span></span>
<span data-ttu-id="dfda4-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dfda4-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
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
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->