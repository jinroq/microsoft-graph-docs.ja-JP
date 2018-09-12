# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="78c20-101">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78c20-101">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="78c20-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="78c20-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78c20-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="78c20-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="78c20-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="78c20-104">Methods</span></span>
|<span data-ttu-id="78c20-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="78c20-105">Method</span></span>|<span data-ttu-id="78c20-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="78c20-106">Return Type</span></span>|<span data-ttu-id="78c20-107">説明</span><span class="sxs-lookup"><span data-stu-id="78c20-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="78c20-108">deviceComplianceUserOverview の取得</span><span class="sxs-lookup"><span data-stu-id="78c20-108">Get deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_get.md)|[<span data-ttu-id="78c20-109">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="78c20-109">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="78c20-110">[deviceCategory](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="78c20-110">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="78c20-111">deviceComplianceUserOverview の更新</span><span class="sxs-lookup"><span data-stu-id="78c20-111">Update deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_update.md)|[<span data-ttu-id="78c20-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="78c20-112">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="78c20-113">[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="78c20-113">Update the properties of a [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="78c20-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78c20-114">Properties</span></span>
|<span data-ttu-id="78c20-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78c20-115">Property</span></span>|<span data-ttu-id="78c20-116">型</span><span class="sxs-lookup"><span data-stu-id="78c20-116">Type</span></span>|<span data-ttu-id="78c20-117">説明</span><span class="sxs-lookup"><span data-stu-id="78c20-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78c20-118">id</span><span class="sxs-lookup"><span data-stu-id="78c20-118">id</span></span>|<span data-ttu-id="78c20-119">文字列</span><span class="sxs-lookup"><span data-stu-id="78c20-119">String</span></span>|<span data-ttu-id="78c20-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="78c20-120">Key of the entity.</span></span>|
|<span data-ttu-id="78c20-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="78c20-121">pendingCount</span></span>|<span data-ttu-id="78c20-122">Int32</span><span class="sxs-lookup"><span data-stu-id="78c20-122">Int32</span></span>|<span data-ttu-id="78c20-123">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="78c20-123">Number of pending Users</span></span>|
|<span data-ttu-id="78c20-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="78c20-124">notApplicableCount</span></span>|<span data-ttu-id="78c20-125">Int32</span><span class="sxs-lookup"><span data-stu-id="78c20-125">Int32</span></span>|<span data-ttu-id="78c20-126">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="78c20-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="78c20-127">successCount</span><span class="sxs-lookup"><span data-stu-id="78c20-127">successCount</span></span>|<span data-ttu-id="78c20-128">Int32</span><span class="sxs-lookup"><span data-stu-id="78c20-128">Int32</span></span>|<span data-ttu-id="78c20-129">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="78c20-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="78c20-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="78c20-130">errorCount</span></span>|<span data-ttu-id="78c20-131">Int32</span><span class="sxs-lookup"><span data-stu-id="78c20-131">Int32</span></span>|<span data-ttu-id="78c20-132">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="78c20-132">Number of error Users</span></span>|
|<span data-ttu-id="78c20-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="78c20-133">failedCount</span></span>|<span data-ttu-id="78c20-134">Int32</span><span class="sxs-lookup"><span data-stu-id="78c20-134">Int32</span></span>|<span data-ttu-id="78c20-135">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="78c20-135">Number of failed Users</span></span>|
|<span data-ttu-id="78c20-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="78c20-136">lastUpdateDateTime</span></span>|<span data-ttu-id="78c20-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78c20-137">DateTimeOffset</span></span>|<span data-ttu-id="78c20-138">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="78c20-138">Last update time</span></span>|
|<span data-ttu-id="78c20-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="78c20-139">configurationVersion</span></span>|<span data-ttu-id="78c20-140">Int32</span><span class="sxs-lookup"><span data-stu-id="78c20-140">Int32</span></span>|<span data-ttu-id="78c20-141">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="78c20-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="78c20-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="78c20-142">Relationships</span></span>
<span data-ttu-id="78c20-143">なし</span><span class="sxs-lookup"><span data-stu-id="78c20-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78c20-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78c20-144">JSON Representation</span></span>
<span data-ttu-id="78c20-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78c20-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
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








