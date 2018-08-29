# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="9f1a3-101">deviceConfigurationUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f1a3-101">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="9f1a3-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9f1a3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f1a3-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9f1a3-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="9f1a3-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f1a3-104">Methods</span></span>
|<span data-ttu-id="9f1a3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f1a3-105">Method</span></span>|<span data-ttu-id="9f1a3-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9f1a3-106">Return Type</span></span>|<span data-ttu-id="9f1a3-107">説明</span><span class="sxs-lookup"><span data-stu-id="9f1a3-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f1a3-108">deviceConfigurationUserOverview の取得</span><span class="sxs-lookup"><span data-stu-id="9f1a3-108">Get deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_get.md)|[<span data-ttu-id="9f1a3-109">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="9f1a3-109">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="9f1a3-110">[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9f1a3-110">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="9f1a3-111">deviceConfigurationUserOverview の更新</span><span class="sxs-lookup"><span data-stu-id="9f1a3-111">Update deviceConfigurationUserOverview</span></span>](../api/intune_deviceconfig_deviceconfigurationuseroverview_update.md)|[<span data-ttu-id="9f1a3-112">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="9f1a3-112">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="9f1a3-113">[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9f1a3-113">Update the properties of a [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f1a3-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f1a3-114">Properties</span></span>
|<span data-ttu-id="9f1a3-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f1a3-115">Property</span></span>|<span data-ttu-id="9f1a3-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="9f1a3-116">Type</span></span>|<span data-ttu-id="9f1a3-117">説明</span><span class="sxs-lookup"><span data-stu-id="9f1a3-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f1a3-118">ID</span><span class="sxs-lookup"><span data-stu-id="9f1a3-118">id</span></span>|<span data-ttu-id="9f1a3-119">文字列</span><span class="sxs-lookup"><span data-stu-id="9f1a3-119">String</span></span>|<span data-ttu-id="9f1a3-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9f1a3-120">Key of the entity.</span></span>|
|<span data-ttu-id="9f1a3-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="9f1a3-121">pendingCount</span></span>|<span data-ttu-id="9f1a3-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9f1a3-122">Int32</span></span>|<span data-ttu-id="9f1a3-123">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9f1a3-123">Number of pending Users</span></span>|
|<span data-ttu-id="9f1a3-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9f1a3-124">notApplicableCount</span></span>|<span data-ttu-id="9f1a3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9f1a3-125">Int32</span></span>|<span data-ttu-id="9f1a3-126">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9f1a3-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="9f1a3-127">successCount</span><span class="sxs-lookup"><span data-stu-id="9f1a3-127">successCount</span></span>|<span data-ttu-id="9f1a3-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9f1a3-128">Int32</span></span>|<span data-ttu-id="9f1a3-129">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9f1a3-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="9f1a3-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="9f1a3-130">errorCount</span></span>|<span data-ttu-id="9f1a3-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9f1a3-131">Int32</span></span>|<span data-ttu-id="9f1a3-132">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9f1a3-132">Number of error Users</span></span>|
|<span data-ttu-id="9f1a3-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="9f1a3-133">failedCount</span></span>|<span data-ttu-id="9f1a3-134">Int32</span><span class="sxs-lookup"><span data-stu-id="9f1a3-134">Int32</span></span>|<span data-ttu-id="9f1a3-135">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="9f1a3-135">Number of failed Users</span></span>|
|<span data-ttu-id="9f1a3-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="9f1a3-136">lastUpdateDateTime</span></span>|<span data-ttu-id="9f1a3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f1a3-137">DateTimeOffset</span></span>|<span data-ttu-id="9f1a3-138">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="9f1a3-138">Last update time</span></span>|
|<span data-ttu-id="9f1a3-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="9f1a3-139">configurationVersion</span></span>|<span data-ttu-id="9f1a3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9f1a3-140">Int32</span></span>|<span data-ttu-id="9f1a3-141">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="9f1a3-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f1a3-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f1a3-142">Relationships</span></span>
<span data-ttu-id="9f1a3-143">なし</span><span class="sxs-lookup"><span data-stu-id="9f1a3-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f1a3-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f1a3-144">JSON Representation</span></span>
<span data-ttu-id="9f1a3-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f1a3-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



