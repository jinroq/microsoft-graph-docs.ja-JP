# <a name="devicemanagement-resource-type"></a><span data-ttu-id="2e21f-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e21f-101">deviceManagement resource type</span></span>

> <span data-ttu-id="2e21f-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e21f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e21f-103">すべてのデバイス アプリの管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="2e21f-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="2e21f-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="2e21f-104">Methods</span></span>
|<span data-ttu-id="2e21f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2e21f-105">Method</span></span>|<span data-ttu-id="2e21f-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2e21f-106">Return Type</span></span>|<span data-ttu-id="2e21f-107">説明</span><span class="sxs-lookup"><span data-stu-id="2e21f-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2e21f-108">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2e21f-108">Get deviceManagement</span></span>](../api/intune_auditing_devicemanagement_get.md)|[<span data-ttu-id="2e21f-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2e21f-109">deviceManagement</span></span>](../resources/intune_auditing_devicemanagement.md)|<span data-ttu-id="2e21f-110">[deviceManagement](../resources/intune_auditing_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2e21f-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_auditing_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="2e21f-111">Update deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2e21f-111">Update deviceManagement</span></span>](../api/intune_auditing_devicemanagement_update.md)|[<span data-ttu-id="2e21f-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2e21f-112">deviceManagement</span></span>](../resources/intune_auditing_devicemanagement.md)|<span data-ttu-id="2e21f-113">[deviceManagement](../resources/intune_auditing_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2e21f-113">Update the properties of a [calendar](../resources/intune_auditing_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2e21f-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e21f-114">Properties</span></span>
|<span data-ttu-id="2e21f-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e21f-115">Property</span></span>|<span data-ttu-id="2e21f-116">型</span><span class="sxs-lookup"><span data-stu-id="2e21f-116">Type</span></span>|<span data-ttu-id="2e21f-117">説明</span><span class="sxs-lookup"><span data-stu-id="2e21f-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e21f-118">id</span><span class="sxs-lookup"><span data-stu-id="2e21f-118">id</span></span>|<span data-ttu-id="2e21f-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2e21f-119">String</span></span>|<span data-ttu-id="2e21f-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2e21f-120">Name of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e21f-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e21f-121">Relationships</span></span>
|<span data-ttu-id="2e21f-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e21f-122">Relationship</span></span>|<span data-ttu-id="2e21f-123">型</span><span class="sxs-lookup"><span data-stu-id="2e21f-123">Type</span></span>|<span data-ttu-id="2e21f-124">説明</span><span class="sxs-lookup"><span data-stu-id="2e21f-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e21f-125">auditEvents</span><span class="sxs-lookup"><span data-stu-id="2e21f-125">auditEvents</span></span>|<span data-ttu-id="2e21f-126">[auditEvent](../resources/intune_auditing_auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2e21f-126">[auditEvent](../resources/intune_auditing_auditevent.md) collection</span></span>|<span data-ttu-id="2e21f-127">監査イベント</span><span class="sxs-lookup"><span data-stu-id="2e21f-127">The Audit Events</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e21f-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e21f-128">JSON Representation</span></span>
<span data-ttu-id="2e21f-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2e21f-129">Here is a JSON representation of the resource.</span></span>
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



