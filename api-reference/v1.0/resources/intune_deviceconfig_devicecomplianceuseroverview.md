# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="f924f-101">deviceComplianceUserOverview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f924f-101">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="f924f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f924f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f924f-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f924f-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="f924f-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="f924f-104">Methods</span></span>
|<span data-ttu-id="f924f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f924f-105">Method</span></span>|<span data-ttu-id="f924f-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f924f-106">Return Type</span></span>|<span data-ttu-id="f924f-107">説明</span><span class="sxs-lookup"><span data-stu-id="f924f-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f924f-108">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f924f-108">Get deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_get.md)|[<span data-ttu-id="f924f-109">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f924f-109">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="f924f-110">[deviceCategory](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f924f-110">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="f924f-111">Update deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f924f-111">Update deviceComplianceUserOverview</span></span>](../api/intune_deviceconfig_devicecomplianceuseroverview_update.md)|[<span data-ttu-id="f924f-112">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f924f-112">deviceComplianceUserOverview</span></span>](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|<span data-ttu-id="f924f-113">[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f924f-113">Update the properties of a [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f924f-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f924f-114">Properties</span></span>
|<span data-ttu-id="f924f-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f924f-115">Property</span></span>|<span data-ttu-id="f924f-116">型</span><span class="sxs-lookup"><span data-stu-id="f924f-116">Type</span></span>|<span data-ttu-id="f924f-117">説明</span><span class="sxs-lookup"><span data-stu-id="f924f-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f924f-118">id</span><span class="sxs-lookup"><span data-stu-id="f924f-118">id</span></span>|<span data-ttu-id="f924f-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f924f-119">String</span></span>|<span data-ttu-id="f924f-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f924f-120">Key of the entity.</span></span>|
|<span data-ttu-id="f924f-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f924f-121">pendingCount</span></span>|<span data-ttu-id="f924f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f924f-122">Int32</span></span>|<span data-ttu-id="f924f-123">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f924f-123">Number of pending Users</span></span>|
|<span data-ttu-id="f924f-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f924f-124">notApplicableCount</span></span>|<span data-ttu-id="f924f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f924f-125">Int32</span></span>|<span data-ttu-id="f924f-126">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f924f-126">Number of not applicable users</span></span>|
|<span data-ttu-id="f924f-127">successCount</span><span class="sxs-lookup"><span data-stu-id="f924f-127">successCount</span></span>|<span data-ttu-id="f924f-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f924f-128">Int32</span></span>|<span data-ttu-id="f924f-129">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f924f-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="f924f-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="f924f-130">errorCount</span></span>|<span data-ttu-id="f924f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f924f-131">Int32</span></span>|<span data-ttu-id="f924f-132">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f924f-132">Number of error Users</span></span>|
|<span data-ttu-id="f924f-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="f924f-133">failedCount</span></span>|<span data-ttu-id="f924f-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f924f-134">Int32</span></span>|<span data-ttu-id="f924f-135">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="f924f-135">Number of failed Users</span></span>|
|<span data-ttu-id="f924f-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f924f-136">lastUpdateDateTime</span></span>|<span data-ttu-id="f924f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f924f-137">DateTimeOffset</span></span>|<span data-ttu-id="f924f-138">最終更新日時</span><span class="sxs-lookup"><span data-stu-id="f924f-138">Last update time</span></span>|
|<span data-ttu-id="f924f-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f924f-139">configurationVersion</span></span>|<span data-ttu-id="f924f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f924f-140">Int32</span></span>|<span data-ttu-id="f924f-141">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="f924f-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="f924f-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f924f-142">Relationships</span></span>
<span data-ttu-id="f924f-143">なし</span><span class="sxs-lookup"><span data-stu-id="f924f-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f924f-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f924f-144">JSON Representation</span></span>
<span data-ttu-id="f924f-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f924f-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}
-->
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



