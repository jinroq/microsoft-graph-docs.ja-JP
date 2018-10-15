# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="27ff6-101">domainDnsCnameRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27ff6-101">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="27ff6-p101">テナント内の特定のドメインの DNS ゾーン ファイルに追加された CNAME レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="27ff6-p101">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="27ff6-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="27ff6-104">Methods</span></span>
<span data-ttu-id="27ff6-p102">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="27ff6-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="27ff6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27ff6-107">Properties</span></span>
| <span data-ttu-id="27ff6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27ff6-108">Property</span></span>     | <span data-ttu-id="27ff6-109">タイプ</span><span class="sxs-lookup"><span data-stu-id="27ff6-109">Type</span></span>   |<span data-ttu-id="27ff6-110">説明</span><span class="sxs-lookup"><span data-stu-id="27ff6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27ff6-111">canonicalName</span><span class="sxs-lookup"><span data-stu-id="27ff6-111">canonicalName</span></span>|<span data-ttu-id="27ff6-112">文字列</span><span class="sxs-lookup"><span data-stu-id="27ff6-112">String</span></span>| <span data-ttu-id="27ff6-p103">CNAME レコードの正規名。DNS ホストで CNAME レコードを構成するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="27ff6-p103">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="27ff6-115">id</span><span class="sxs-lookup"><span data-stu-id="27ff6-115">id</span></span>|<span data-ttu-id="27ff6-116">文字列</span><span class="sxs-lookup"><span data-stu-id="27ff6-116">String</span></span>| <span data-ttu-id="27ff6-p104">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="27ff6-p104">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="27ff6-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="27ff6-119">isOptional</span></span>|<span data-ttu-id="27ff6-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="27ff6-120">Boolean</span></span>| <span data-ttu-id="27ff6-p105">false の場合、ドメインが指定された Microsoft Online Services が適切に機能するには、CNAME レコードが DNS ホストで顧客によって構成されている必要があります。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="27ff6-p105">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="27ff6-123">label</span><span class="sxs-lookup"><span data-stu-id="27ff6-123">label</span></span>|<span data-ttu-id="27ff6-124">文字列</span><span class="sxs-lookup"><span data-stu-id="27ff6-124">String</span></span>| <span data-ttu-id="27ff6-125">DNS ホストで CNAME レコードの*エイリアス/ホスト/名前*を構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="27ff6-125">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="27ff6-126">recordType</span><span class="sxs-lookup"><span data-stu-id="27ff6-126">recordType</span></span>|<span data-ttu-id="27ff6-127">文字列</span><span class="sxs-lookup"><span data-stu-id="27ff6-127">String</span></span>| <span data-ttu-id="27ff6-p106">DNS レコードの種類。この値は常に *CName* です。キー</span><span class="sxs-lookup"><span data-stu-id="27ff6-p106">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="27ff6-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="27ff6-131">supportedService</span></span>|<span data-ttu-id="27ff6-132">文字列</span><span class="sxs-lookup"><span data-stu-id="27ff6-132">String</span></span>| <span data-ttu-id="27ff6-133">Microsoft オンライン サービスまたはこの CNAME レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="27ff6-133">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="27ff6-134">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="27ff6-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="27ff6-135">ttl</span><span class="sxs-lookup"><span data-stu-id="27ff6-135">ttl</span></span>|<span data-ttu-id="27ff6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="27ff6-136">Int32</span></span>| <span data-ttu-id="27ff6-p107">DNS ホストで CNAME レコードの Time To Live (TTL) のプロパティを構成するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="27ff6-p107">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="27ff6-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="27ff6-139">Relationships</span></span>
<span data-ttu-id="27ff6-140">なし</span><span class="sxs-lookup"><span data-stu-id="27ff6-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="27ff6-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27ff6-141">JSON representation</span></span>
<span data-ttu-id="27ff6-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="27ff6-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
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