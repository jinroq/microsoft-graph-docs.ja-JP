# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="d3159-101">managedDeviceMobileAppConfigurationUserSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d3159-101">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="d3159-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3159-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3159-103">MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d3159-103">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="d3159-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3159-104">Methods</span></span>
|<span data-ttu-id="d3159-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3159-105">Method</span></span>|<span data-ttu-id="d3159-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d3159-106">Return Type</span></span>|<span data-ttu-id="d3159-107">説明</span><span class="sxs-lookup"><span data-stu-id="d3159-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d3159-108">managedDeviceMobileAppConfigurationUserSummary の取得</span><span class="sxs-lookup"><span data-stu-id="d3159-108">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_get.md)|[<span data-ttu-id="d3159-109">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="d3159-109">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="d3159-110">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d3159-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="d3159-111">managedDeviceMobileAppConfigurationUserSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d3159-111">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_update.md)|[<span data-ttu-id="d3159-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="d3159-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="d3159-113">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d3159-113">Update the properties of a [calendar](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3159-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3159-114">Properties</span></span>
|<span data-ttu-id="d3159-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3159-115">Property</span></span>|<span data-ttu-id="d3159-116">型</span><span class="sxs-lookup"><span data-stu-id="d3159-116">Type</span></span>|<span data-ttu-id="d3159-117">説明</span><span class="sxs-lookup"><span data-stu-id="d3159-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3159-118">id</span><span class="sxs-lookup"><span data-stu-id="d3159-118">id</span></span>|<span data-ttu-id="d3159-119">String</span><span class="sxs-lookup"><span data-stu-id="d3159-119">String</span></span>|<span data-ttu-id="d3159-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d3159-120">Name of the entity.</span></span>|
|<span data-ttu-id="d3159-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d3159-121">pendingCount</span></span>|<span data-ttu-id="d3159-122">Int32</span><span class="sxs-lookup"><span data-stu-id="d3159-122">Int32</span></span>|<span data-ttu-id="d3159-123">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="d3159-123">Number of pending Users</span></span>|
|<span data-ttu-id="d3159-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d3159-124">notApplicableCount</span></span>|<span data-ttu-id="d3159-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d3159-125">Int32</span></span>|<span data-ttu-id="d3159-126">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d3159-126">Number of not applicable devices</span></span>|
|<span data-ttu-id="d3159-127">successCount</span><span class="sxs-lookup"><span data-stu-id="d3159-127">successCount</span></span>|<span data-ttu-id="d3159-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d3159-128">Int32</span></span>|<span data-ttu-id="d3159-129">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="d3159-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="d3159-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="d3159-130">errorCount</span></span>|<span data-ttu-id="d3159-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d3159-131">Int32</span></span>|<span data-ttu-id="d3159-132">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="d3159-132">Number of error Users</span></span>|
|<span data-ttu-id="d3159-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="d3159-133">failedCount</span></span>|<span data-ttu-id="d3159-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d3159-134">Int32</span></span>|<span data-ttu-id="d3159-135">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="d3159-135">Number of failed Users</span></span>|
|<span data-ttu-id="d3159-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d3159-136">lastUpdateDateTime</span></span>|<span data-ttu-id="d3159-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3159-137">DateTimeOffset</span></span>|<span data-ttu-id="d3159-138">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="d3159-138">Last update time</span></span>|
|<span data-ttu-id="d3159-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d3159-139">configurationVersion</span></span>|<span data-ttu-id="d3159-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d3159-140">Int32</span></span>|<span data-ttu-id="d3159-141">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="d3159-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3159-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d3159-142">Relationships</span></span>
<span data-ttu-id="d3159-143">なし</span><span class="sxs-lookup"><span data-stu-id="d3159-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d3159-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3159-144">JSON Representation</span></span>
<span data-ttu-id="d3159-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d3159-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
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



