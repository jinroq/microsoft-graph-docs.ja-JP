# <a name="verifieddomain-resource-type"></a><span data-ttu-id="22beb-101">verifiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22beb-101">verifiedDomain resource type</span></span>

<span data-ttu-id="22beb-p101">テナントのドメインを指定します。[組織](organization.md) エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="22beb-p101">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="22beb-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22beb-104">Properties</span></span>
| <span data-ttu-id="22beb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22beb-105">Property</span></span>     | <span data-ttu-id="22beb-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="22beb-106">Type</span></span>   |<span data-ttu-id="22beb-107">説明</span><span class="sxs-lookup"><span data-stu-id="22beb-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22beb-108">capabilities</span><span class="sxs-lookup"><span data-stu-id="22beb-108">capabilities</span></span>|<span data-ttu-id="22beb-109">String</span><span class="sxs-lookup"><span data-stu-id="22beb-109">String</span></span>|<span data-ttu-id="22beb-110">「電子メール」、「OfficeCommunicationsOnline」など。</span><span class="sxs-lookup"><span data-stu-id="22beb-110">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="22beb-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="22beb-111">isDefault</span></span>|<span data-ttu-id="22beb-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="22beb-112">Boolean</span></span>|                <span data-ttu-id="22beb-113">これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="22beb-113">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="22beb-114">isInitial</span><span class="sxs-lookup"><span data-stu-id="22beb-114">isInitial</span></span>|<span data-ttu-id="22beb-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="22beb-115">Boolean</span></span>|<span data-ttu-id="22beb-116">これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="22beb-116">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="22beb-117">name</span><span class="sxs-lookup"><span data-stu-id="22beb-117">name</span></span>|<span data-ttu-id="22beb-118">String</span><span class="sxs-lookup"><span data-stu-id="22beb-118">String</span></span>|<span data-ttu-id="22beb-119">ドメイン名。「contoso.onmicrosoft.com」など。</span><span class="sxs-lookup"><span data-stu-id="22beb-119">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="22beb-120">type</span><span class="sxs-lookup"><span data-stu-id="22beb-120">type</span></span>|<span data-ttu-id="22beb-121">String</span><span class="sxs-lookup"><span data-stu-id="22beb-121">String</span></span>|<span data-ttu-id="22beb-122">「管理対象」など。</span><span class="sxs-lookup"><span data-stu-id="22beb-122">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22beb-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22beb-123">JSON representation</span></span>

<span data-ttu-id="22beb-124">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="22beb-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
