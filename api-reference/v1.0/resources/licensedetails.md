# <a name="licensedetails-resource-type"></a><span data-ttu-id="2b11e-101">licenseDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b11e-101">licenseDetails resource type</span></span>

<span data-ttu-id="2b11e-102">ユーザーに割り当てられているライセンスに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2b11e-102">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="2b11e-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="2b11e-103">Methods</span></span>

| <span data-ttu-id="2b11e-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="2b11e-104">Method</span></span>           | <span data-ttu-id="2b11e-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2b11e-105">Return Type</span></span>    |<span data-ttu-id="2b11e-106">説明</span><span class="sxs-lookup"><span data-stu-id="2b11e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b11e-107">licenseDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2b11e-107">List licenseDetails</span></span>](../api/user_list_licensedetails.md) | <span data-ttu-id="2b11e-108">licenseDetails コレクション</span><span class="sxs-lookup"><span data-stu-id="2b11e-108">licenseDetails collection</span></span> |<span data-ttu-id="2b11e-109">ユーザーの licenseDetails オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="2b11e-109">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails_get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="2b11e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b11e-110">Properties</span></span>
| <span data-ttu-id="2b11e-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b11e-111">Property</span></span>     | <span data-ttu-id="2b11e-112">タイプ</span><span class="sxs-lookup"><span data-stu-id="2b11e-112">Type</span></span>   |<span data-ttu-id="2b11e-113">説明</span><span class="sxs-lookup"><span data-stu-id="2b11e-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b11e-114">ID</span><span class="sxs-lookup"><span data-stu-id="2b11e-114">id</span></span>|<span data-ttu-id="2b11e-115">文字列</span><span class="sxs-lookup"><span data-stu-id="2b11e-115">String</span></span>| <span data-ttu-id="2b11e-p101">ライセンス詳細オブジェクトの一意識別子。読み取り専用。キー。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="2b11e-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="2b11e-118">servicePlans</span><span class="sxs-lookup"><span data-stu-id="2b11e-118">servicePlans</span></span>|<span data-ttu-id="2b11e-119">[servicePlanInfo](serviceplaninfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2b11e-119">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="2b11e-p102">ライセンスが割り当てられたサービス プランに関する情報。読み取り専用。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="2b11e-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="2b11e-122">skuId</span><span class="sxs-lookup"><span data-stu-id="2b11e-122">skuId</span></span>|<span data-ttu-id="2b11e-123">Guid</span><span class="sxs-lookup"><span data-stu-id="2b11e-123">Guid</span></span>| <span data-ttu-id="2b11e-p103">サービス SKU の一意識別子 (GUID)。関連する [SubscribedSku](subscribedsku.md) オブジェクトの skuId プロパティと同じです。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="2b11e-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="2b11e-127">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="2b11e-127">skuPartNumber</span></span>|<span data-ttu-id="2b11e-128">文字列</span><span class="sxs-lookup"><span data-stu-id="2b11e-128">String</span></span>| <span data-ttu-id="2b11e-p104">一意の SKU 表示名です。関連する [SubscribedSku](subscribedsku.md) オブジェクトの skuPartNumber と同じです。例: "AAD_Premium"。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="2b11e-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="2b11e-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b11e-132">Relationships</span></span>
<span data-ttu-id="2b11e-133">なし</span><span class="sxs-lookup"><span data-stu-id="2b11e-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b11e-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b11e-134">JSON representation</span></span>
<span data-ttu-id="2b11e-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2b11e-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->