# <a name="devicemanagement-resource-type"></a><span data-ttu-id="dcda3-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dcda3-101">deviceManagement resource type</span></span>

> <span data-ttu-id="dcda3-102">**重要:**Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dcda3-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dcda3-103">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcda3-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dcda3-104">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dcda3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dcda3-105">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="dcda3-105">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="dcda3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="dcda3-106">Methods</span></span>
|<span data-ttu-id="dcda3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="dcda3-107">Method</span></span>|<span data-ttu-id="dcda3-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dcda3-108">Return Type</span></span>|<span data-ttu-id="dcda3-109">説明</span><span class="sxs-lookup"><span data-stu-id="dcda3-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dcda3-110">deviceManagement の取得</span><span class="sxs-lookup"><span data-stu-id="dcda3-110">Get deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_get.md)|[<span data-ttu-id="dcda3-111">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="dcda3-111">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="dcda3-112">[deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dcda3-112">Read properties and relationships of the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="dcda3-113">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="dcda3-113">Update deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_update.md)|[<span data-ttu-id="dcda3-114">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="dcda3-114">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="dcda3-115">[deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dcda3-115">Update the properties of a [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dcda3-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcda3-116">Properties</span></span>
|<span data-ttu-id="dcda3-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcda3-117">Property</span></span>|<span data-ttu-id="dcda3-118">型</span><span class="sxs-lookup"><span data-stu-id="dcda3-118">Type</span></span>|<span data-ttu-id="dcda3-119">説明</span><span class="sxs-lookup"><span data-stu-id="dcda3-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcda3-120">id</span><span class="sxs-lookup"><span data-stu-id="dcda3-120">id</span></span>|<span data-ttu-id="dcda3-121">String</span><span class="sxs-lookup"><span data-stu-id="dcda3-121">String</span></span>|<span data-ttu-id="dcda3-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dcda3-122">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcda3-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dcda3-123">Relationships</span></span>
|<span data-ttu-id="dcda3-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dcda3-124">Relationship</span></span>|<span data-ttu-id="dcda3-125">型</span><span class="sxs-lookup"><span data-stu-id="dcda3-125">Type</span></span>|<span data-ttu-id="dcda3-126">説明</span><span class="sxs-lookup"><span data-stu-id="dcda3-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcda3-127">troubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="dcda3-127">troubleshootingEvents</span></span>|<span data-ttu-id="dcda3-128">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dcda3-128">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="dcda3-129">テナントのトラブルシューティング イベントの一覧です。</span><span class="sxs-lookup"><span data-stu-id="dcda3-129">The list of troubleshooting events for the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dcda3-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dcda3-130">JSON Representation</span></span>
<span data-ttu-id="dcda3-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dcda3-131">Here is a JSON representation of the resource.</span></span>
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



