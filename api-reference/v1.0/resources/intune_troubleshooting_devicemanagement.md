# <a name="devicemanagement-resource-type"></a><span data-ttu-id="ef3bb-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef3bb-101">deviceManagement resource type</span></span>

> <span data-ttu-id="ef3bb-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef3bb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef3bb-103">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="ef3bb-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="ef3bb-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef3bb-104">Methods</span></span>
|<span data-ttu-id="ef3bb-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef3bb-105">Method</span></span>|<span data-ttu-id="ef3bb-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ef3bb-106">Return Type</span></span>|<span data-ttu-id="ef3bb-107">説明</span><span class="sxs-lookup"><span data-stu-id="ef3bb-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ef3bb-108">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ef3bb-108">Get deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_get.md)|[<span data-ttu-id="ef3bb-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ef3bb-109">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="ef3bb-110">[deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ef3bb-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="ef3bb-111">Update deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ef3bb-111">Update deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_update.md)|[<span data-ttu-id="ef3bb-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ef3bb-112">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="ef3bb-113">[deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ef3bb-113">Update the properties of a [calendar](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ef3bb-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef3bb-114">Properties</span></span>
|<span data-ttu-id="ef3bb-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef3bb-115">Property</span></span>|<span data-ttu-id="ef3bb-116">型</span><span class="sxs-lookup"><span data-stu-id="ef3bb-116">Type</span></span>|<span data-ttu-id="ef3bb-117">説明</span><span class="sxs-lookup"><span data-stu-id="ef3bb-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef3bb-118">id</span><span class="sxs-lookup"><span data-stu-id="ef3bb-118">id</span></span>|<span data-ttu-id="ef3bb-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ef3bb-119">String</span></span>|<span data-ttu-id="ef3bb-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef3bb-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef3bb-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef3bb-121">Relationships</span></span>
|<span data-ttu-id="ef3bb-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef3bb-122">Relationship</span></span>|<span data-ttu-id="ef3bb-123">型</span><span class="sxs-lookup"><span data-stu-id="ef3bb-123">Type</span></span>|<span data-ttu-id="ef3bb-124">説明</span><span class="sxs-lookup"><span data-stu-id="ef3bb-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef3bb-125">troubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="ef3bb-125">troubleshootingEvents</span></span>|<span data-ttu-id="ef3bb-126">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ef3bb-126">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="ef3bb-127">テナントのトラブルシューティング イベントの一覧です。</span><span class="sxs-lookup"><span data-stu-id="ef3bb-127">The list of troubleshooting events for the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef3bb-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef3bb-128">JSON Representation</span></span>
<span data-ttu-id="ef3bb-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ef3bb-129">Here is a JSON representation of the resource.</span></span>
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



