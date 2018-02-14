# <a name="devicecategory-resource-type"></a><span data-ttu-id="6ff9c-101">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ff9c-101">deviceCategory resource type</span></span>

> <span data-ttu-id="6ff9c-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ff9c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ff9c-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6ff9c-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="6ff9c-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ff9c-104">Methods</span></span>
|<span data-ttu-id="6ff9c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ff9c-105">Method</span></span>|<span data-ttu-id="6ff9c-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6ff9c-106">Return Type</span></span>|<span data-ttu-id="6ff9c-107">説明</span><span class="sxs-lookup"><span data-stu-id="6ff9c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6ff9c-108">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="6ff9c-108">Get deviceCategory</span></span>](../api/intune_devices_devicecategory_get.md)|[<span data-ttu-id="6ff9c-109">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6ff9c-109">deviceCategory</span></span>](../resources/intune_devices_devicecategory.md)|<span data-ttu-id="6ff9c-110">[deviceCategory](../resources/intune_devices_devicecategory.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6ff9c-110">Read properties and relationships of [plannerPlanDetails](../resources/intune_devices_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="6ff9c-111">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="6ff9c-111">Update deviceCategory</span></span>](../api/intune_devices_devicecategory_update.md)|[<span data-ttu-id="6ff9c-112">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6ff9c-112">deviceCategory</span></span>](../resources/intune_devices_devicecategory.md)|<span data-ttu-id="6ff9c-113">[deviceCategory](../resources/intune_devices_devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6ff9c-113">Update the properties of a [calendar](../resources/intune_devices_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ff9c-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff9c-114">Properties</span></span>
|<span data-ttu-id="6ff9c-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff9c-115">Property</span></span>|<span data-ttu-id="6ff9c-116">型</span><span class="sxs-lookup"><span data-stu-id="6ff9c-116">Type</span></span>|<span data-ttu-id="6ff9c-117">説明</span><span class="sxs-lookup"><span data-stu-id="6ff9c-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff9c-118">id</span><span class="sxs-lookup"><span data-stu-id="6ff9c-118">id</span></span>|<span data-ttu-id="6ff9c-119">文字列</span><span class="sxs-lookup"><span data-stu-id="6ff9c-119">String</span></span>|<span data-ttu-id="6ff9c-120">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6ff9c-120">Unique identifier for the device category.</span></span> <span data-ttu-id="6ff9c-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6ff9c-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ff9c-122">関係</span><span class="sxs-lookup"><span data-stu-id="6ff9c-122">Relationships</span></span>
<span data-ttu-id="6ff9c-123">なし</span><span class="sxs-lookup"><span data-stu-id="6ff9c-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ff9c-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ff9c-124">JSON Representation</span></span>
<span data-ttu-id="6ff9c-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ff9c-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)"
}
```



