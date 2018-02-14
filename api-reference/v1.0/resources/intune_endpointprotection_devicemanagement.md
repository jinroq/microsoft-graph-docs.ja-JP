# <a name="devicemanagement-resource-type"></a><span data-ttu-id="3258b-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3258b-101">deviceManagement resource type</span></span>

> <span data-ttu-id="3258b-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3258b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3258b-103">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="3258b-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="3258b-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="3258b-104">Methods</span></span>
|<span data-ttu-id="3258b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="3258b-105">Method</span></span>|<span data-ttu-id="3258b-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3258b-106">Return Type</span></span>|<span data-ttu-id="3258b-107">説明</span><span class="sxs-lookup"><span data-stu-id="3258b-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3258b-108">deviceManagement の取得</span><span class="sxs-lookup"><span data-stu-id="3258b-108">Get deviceManagement</span></span>](../api/intune_endpointprotection_devicemanagement_get.md)|[<span data-ttu-id="3258b-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3258b-109">deviceManagement</span></span>](../resources/intune_endpointprotection_devicemanagement.md)|<span data-ttu-id="3258b-110">[deviceManagement](../resources/intune_endpointprotection_devicemanagement.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3258b-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_endpointprotection_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="3258b-111">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="3258b-111">Update deviceManagement</span></span>](../api/intune_endpointprotection_devicemanagement_update.md)|[<span data-ttu-id="3258b-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3258b-112">deviceManagement</span></span>](../resources/intune_endpointprotection_devicemanagement.md)|<span data-ttu-id="3258b-113">[deviceManagement](../resources/intune_endpointprotection_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3258b-113">Update the properties of a [calendar](../resources/intune_endpointprotection_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3258b-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3258b-114">Properties</span></span>
|<span data-ttu-id="3258b-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3258b-115">Property</span></span>|<span data-ttu-id="3258b-116">型</span><span class="sxs-lookup"><span data-stu-id="3258b-116">Type</span></span>|<span data-ttu-id="3258b-117">説明</span><span class="sxs-lookup"><span data-stu-id="3258b-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3258b-118">id</span><span class="sxs-lookup"><span data-stu-id="3258b-118">id</span></span>|<span data-ttu-id="3258b-119">文字列</span><span class="sxs-lookup"><span data-stu-id="3258b-119">String</span></span>|<span data-ttu-id="3258b-120">一意識別子</span><span class="sxs-lookup"><span data-stu-id="3258b-120">Unique Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="3258b-121">関係</span><span class="sxs-lookup"><span data-stu-id="3258b-121">Relationships</span></span>
<span data-ttu-id="3258b-122">なし</span><span class="sxs-lookup"><span data-stu-id="3258b-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3258b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3258b-123">JSON Representation</span></span>
<span data-ttu-id="3258b-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3258b-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



