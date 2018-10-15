# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="2a315-101">managedDeviceMobileAppConfigurationUserSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a315-101">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="2a315-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a315-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a315-103">MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a315-103">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="2a315-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a315-104">Methods</span></span>
|<span data-ttu-id="2a315-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a315-105">Method</span></span>|<span data-ttu-id="2a315-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2a315-106">Return Type</span></span>|<span data-ttu-id="2a315-107">説明</span><span class="sxs-lookup"><span data-stu-id="2a315-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2a315-108">managedDeviceMobileAppConfigurationUserSummary の取得</span><span class="sxs-lookup"><span data-stu-id="2a315-108">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_get.md)|[<span data-ttu-id="2a315-109">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="2a315-109">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="2a315-110">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2a315-110">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="2a315-111">managedDeviceMobileAppConfigurationUserSummary の更新</span><span class="sxs-lookup"><span data-stu-id="2a315-111">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_update.md)|[<span data-ttu-id="2a315-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="2a315-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="2a315-113">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2a315-113">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a315-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a315-114">Properties</span></span>
|<span data-ttu-id="2a315-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a315-115">Property</span></span>|<span data-ttu-id="2a315-116">型</span><span class="sxs-lookup"><span data-stu-id="2a315-116">Type</span></span>|<span data-ttu-id="2a315-117">説明</span><span class="sxs-lookup"><span data-stu-id="2a315-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a315-118">ID</span><span class="sxs-lookup"><span data-stu-id="2a315-118">id</span></span>|<span data-ttu-id="2a315-119">文字列</span><span class="sxs-lookup"><span data-stu-id="2a315-119">String</span></span>|<span data-ttu-id="2a315-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2a315-120">Key of the entity.</span></span>|
|<span data-ttu-id="2a315-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="2a315-121">pendingCount</span></span>|<span data-ttu-id="2a315-122">Int32</span><span class="sxs-lookup"><span data-stu-id="2a315-122">Int32</span></span>|<span data-ttu-id="2a315-123">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="2a315-123">Number of pending Users</span></span>|
|<span data-ttu-id="2a315-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="2a315-124">notApplicableCount</span></span>|<span data-ttu-id="2a315-125">Int32</span><span class="sxs-lookup"><span data-stu-id="2a315-125">Int32</span></span>|<span data-ttu-id="2a315-126">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="2a315-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="2a315-127">successCount</span><span class="sxs-lookup"><span data-stu-id="2a315-127">successCount</span></span>|<span data-ttu-id="2a315-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2a315-128">Int32</span></span>|<span data-ttu-id="2a315-129">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="2a315-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="2a315-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="2a315-130">errorCount</span></span>|<span data-ttu-id="2a315-131">Int32</span><span class="sxs-lookup"><span data-stu-id="2a315-131">Int32</span></span>|<span data-ttu-id="2a315-132">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="2a315-132">Number of error Users</span></span>|
|<span data-ttu-id="2a315-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="2a315-133">failedCount</span></span>|<span data-ttu-id="2a315-134">Int32</span><span class="sxs-lookup"><span data-stu-id="2a315-134">Int32</span></span>|<span data-ttu-id="2a315-135">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="2a315-135">Number of failed Users</span></span>|
|<span data-ttu-id="2a315-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2a315-136">lastUpdateDateTime</span></span>|<span data-ttu-id="2a315-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a315-137">DateTimeOffset</span></span>|<span data-ttu-id="2a315-138">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="2a315-138">Last update time</span></span>|
|<span data-ttu-id="2a315-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="2a315-139">configurationVersion</span></span>|<span data-ttu-id="2a315-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2a315-140">Int32</span></span>|<span data-ttu-id="2a315-141">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="2a315-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a315-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a315-142">Relationships</span></span>
<span data-ttu-id="2a315-143">なし</span><span class="sxs-lookup"><span data-stu-id="2a315-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a315-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a315-144">JSON Representation</span></span>
<span data-ttu-id="2a315-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2a315-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}-->
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








