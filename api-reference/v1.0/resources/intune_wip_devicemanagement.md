# <a name="devicemanagement-resource-type"></a><span data-ttu-id="3ef28-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3ef28-101">deviceManagement resource type</span></span>

> <span data-ttu-id="3ef28-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ef28-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ef28-103">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="3ef28-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="3ef28-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="3ef28-104">Methods</span></span>
|<span data-ttu-id="3ef28-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="3ef28-105">Method</span></span>|<span data-ttu-id="3ef28-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3ef28-106">Return Type</span></span>|<span data-ttu-id="3ef28-107">説明</span><span class="sxs-lookup"><span data-stu-id="3ef28-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3ef28-108">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3ef28-108">Get deviceManagement</span></span>](../api/intune_wip_devicemanagement_get.md)|[<span data-ttu-id="3ef28-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3ef28-109">deviceManagement</span></span>](../resources/intune_wip_devicemanagement.md)|<span data-ttu-id="3ef28-110">[deviceManagement](../resources/intune_wip_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3ef28-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_wip_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="3ef28-111">Update deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3ef28-111">Update deviceManagement</span></span>](../api/intune_wip_devicemanagement_update.md)|[<span data-ttu-id="3ef28-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3ef28-112">deviceManagement</span></span>](../resources/intune_wip_devicemanagement.md)|<span data-ttu-id="3ef28-113">[deviceManagement](../resources/intune_wip_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3ef28-113">Update the properties of a [calendar](../resources/intune_wip_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ef28-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ef28-114">Properties</span></span>
|<span data-ttu-id="3ef28-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ef28-115">Property</span></span>|<span data-ttu-id="3ef28-116">型</span><span class="sxs-lookup"><span data-stu-id="3ef28-116">Type</span></span>|<span data-ttu-id="3ef28-117">説明</span><span class="sxs-lookup"><span data-stu-id="3ef28-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ef28-118">id</span><span class="sxs-lookup"><span data-stu-id="3ef28-118">id</span></span>|<span data-ttu-id="3ef28-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3ef28-119">String</span></span>|<span data-ttu-id="3ef28-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3ef28-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ef28-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3ef28-121">Relationships</span></span>
|<span data-ttu-id="3ef28-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3ef28-122">Relationship</span></span>|<span data-ttu-id="3ef28-123">型</span><span class="sxs-lookup"><span data-stu-id="3ef28-123">Type</span></span>|<span data-ttu-id="3ef28-124">説明</span><span class="sxs-lookup"><span data-stu-id="3ef28-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ef28-125">windowsInformationProtectionAppLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="3ef28-125">windowsInformationProtectionAppLearningSummaries</span></span>|<span data-ttu-id="3ef28-126">[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3ef28-126">[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) collection</span></span>|<span data-ttu-id="3ef28-127">Windows 情報保護アプリの学習概要。</span><span class="sxs-lookup"><span data-stu-id="3ef28-127">The windows information protection app learning summaries.</span></span>|
|<span data-ttu-id="3ef28-128">windowsInformationProtectionNetworkLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="3ef28-128">windowsInformationProtectionNetworkLearningSummaries</span></span>|<span data-ttu-id="3ef28-129">[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3ef28-129">[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) collection</span></span>|<span data-ttu-id="3ef28-130">Windows 情報保護ネットワークの学習概要。</span><span class="sxs-lookup"><span data-stu-id="3ef28-130">The windows information protection network learning summaries.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ef28-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3ef28-131">JSON Representation</span></span>
<span data-ttu-id="3ef28-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3ef28-132">Here is a JSON representation of the resource.</span></span>
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



