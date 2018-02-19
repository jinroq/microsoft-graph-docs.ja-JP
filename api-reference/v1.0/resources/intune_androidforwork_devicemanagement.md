# <a name="devicemanagement-resource-type"></a><span data-ttu-id="1df51-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1df51-101">deviceManagement resource type</span></span>

> <span data-ttu-id="1df51-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1df51-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1df51-103">デバイス管理下で Android for Work 設定機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="1df51-103">Singleton entity that acts as a container for Android for Work settings functionality under device management.</span></span>
## <a name="methods"></a><span data-ttu-id="1df51-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="1df51-104">Methods</span></span>
|<span data-ttu-id="1df51-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1df51-105">Method</span></span>|<span data-ttu-id="1df51-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1df51-106">Return Type</span></span>|<span data-ttu-id="1df51-107">説明</span><span class="sxs-lookup"><span data-stu-id="1df51-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1df51-108">deviceManagement の取得</span><span class="sxs-lookup"><span data-stu-id="1df51-108">Get deviceManagement</span></span>](../api/intune_androidforwork_devicemanagement_get.md)|[<span data-ttu-id="1df51-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1df51-109">deviceManagement</span></span>](../resources/intune_androidforwork_devicemanagement.md)|<span data-ttu-id="1df51-110">[deviceManagement](../resources/intune_androidforwork_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1df51-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_androidforwork_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="1df51-111">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="1df51-111">Update deviceManagement</span></span>](../api/intune_androidforwork_devicemanagement_update.md)|[<span data-ttu-id="1df51-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1df51-112">deviceManagement</span></span>](../resources/intune_androidforwork_devicemanagement.md)|<span data-ttu-id="1df51-113">[deviceManagement](../resources/intune_androidforwork_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1df51-113">Update the properties of a [calendar](../resources/intune_androidforwork_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1df51-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1df51-114">Properties</span></span>
|<span data-ttu-id="1df51-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1df51-115">Property</span></span>|<span data-ttu-id="1df51-116">型</span><span class="sxs-lookup"><span data-stu-id="1df51-116">Type</span></span>|<span data-ttu-id="1df51-117">説明</span><span class="sxs-lookup"><span data-stu-id="1df51-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1df51-118">id</span><span class="sxs-lookup"><span data-stu-id="1df51-118">id</span></span>|<span data-ttu-id="1df51-119">String</span><span class="sxs-lookup"><span data-stu-id="1df51-119">String</span></span>|<span data-ttu-id="1df51-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1df51-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="1df51-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1df51-121">Relationships</span></span>
|<span data-ttu-id="1df51-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1df51-122">Relationship</span></span>|<span data-ttu-id="1df51-123">型</span><span class="sxs-lookup"><span data-stu-id="1df51-123">Type</span></span>|<span data-ttu-id="1df51-124">説明</span><span class="sxs-lookup"><span data-stu-id="1df51-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1df51-125">androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="1df51-125">androidForWorkSettings</span></span>|[<span data-ttu-id="1df51-126">androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="1df51-126">androidForWorkSettings</span></span>](../resources/intune_androidforwork_androidforworksettings.md)|<span data-ttu-id="1df51-127">単一の Android for Work 設定エンティティです。</span><span class="sxs-lookup"><span data-stu-id="1df51-127">The singleton Android for Work settings entity.</span></span>|
|<span data-ttu-id="1df51-128">androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="1df51-128">androidForWorkAppConfigurationSchemas</span></span>|<span data-ttu-id="1df51-129">[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1df51-129">[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) collection</span></span>|<span data-ttu-id="1df51-130">Android for Work アプリの構成スキーマ アイテムのエンティティです。</span><span class="sxs-lookup"><span data-stu-id="1df51-130">Android for Work app configuration schema entities.</span></span>|
|<span data-ttu-id="1df51-131">androidForWorkEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="1df51-131">androidForWorkEnrollmentProfiles</span></span>|<span data-ttu-id="1df51-132">[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1df51-132">[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) collection</span></span>|<span data-ttu-id="1df51-133">Android for Work 登録プロファイルのエンティティです。</span><span class="sxs-lookup"><span data-stu-id="1df51-133">Android for Work enrollment profile entities.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1df51-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1df51-134">JSON Representation</span></span>
<span data-ttu-id="1df51-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1df51-135">Here is a JSON representation of the resource.</span></span>
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



