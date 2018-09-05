# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="978c8-101">onPremisesProvisioningError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="978c8-101">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="978c8-102">内部設置型ディレクトリを Azure Active Directory に同期するときの[ユーザー](user.md)と[グループ](group.md)のエンティティのディレクトリ同期エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="978c8-102">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="978c8-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="978c8-103">Properties</span></span>

| <span data-ttu-id="978c8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="978c8-104">Property</span></span> | <span data-ttu-id="978c8-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="978c8-105">Type</span></span> | <span data-ttu-id="978c8-106">説明</span><span class="sxs-lookup"><span data-stu-id="978c8-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="978c8-107">category</span><span class="sxs-lookup"><span data-stu-id="978c8-107">category</span></span>|<span data-ttu-id="978c8-108">文字列</span><span class="sxs-lookup"><span data-stu-id="978c8-108">String</span></span>| <span data-ttu-id="978c8-109">事前設定時のエラーのカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="978c8-109">Category of the provisioning error.</span></span> <span data-ttu-id="978c8-110">注意: 現時点で使用可能な値は 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="978c8-110">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="978c8-111">使用可能な値: *PropertyConflict* - プロパティの値が一意でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="978c8-111">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="978c8-112">他のオブジェクトには、プロパティの同じ値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="978c8-112">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="978c8-113">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="978c8-113">occurredDateTime</span></span>|<span data-ttu-id="978c8-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="978c8-114">DateTimeOffset</span></span>| <span data-ttu-id="978c8-115">エラーが発生した日時。</span><span class="sxs-lookup"><span data-stu-id="978c8-115">The time at which the error occurred.</span></span> |
|<span data-ttu-id="978c8-116">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="978c8-116">propertyCausingError</span></span>|<span data-ttu-id="978c8-117">文字列</span><span class="sxs-lookup"><span data-stu-id="978c8-117">String</span></span>| <span data-ttu-id="978c8-118">エラーの原因となっているディレクトリのプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="978c8-118">Name of the directory property causing the error.</span></span> <span data-ttu-id="978c8-119">現在使用可能な値: *UserPrincipalName* または *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="978c8-119">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="978c8-120">value</span><span class="sxs-lookup"><span data-stu-id="978c8-120">value</span></span>|<span data-ttu-id="978c8-121">文字列</span><span class="sxs-lookup"><span data-stu-id="978c8-121">String</span></span>| <span data-ttu-id="978c8-122">エラーの原因となっているプロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="978c8-122">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="978c8-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="978c8-123">JSON representation</span></span>
<span data-ttu-id="978c8-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="978c8-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->