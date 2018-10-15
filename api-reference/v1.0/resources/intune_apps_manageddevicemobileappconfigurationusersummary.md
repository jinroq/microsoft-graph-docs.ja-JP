# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="610d5-101">managedDeviceMobileAppConfigurationUserSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="610d5-101">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="610d5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="610d5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="610d5-103">MDM モバイル アプリ構成のユーザー状態の要約に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="610d5-103">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="610d5-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="610d5-104">Methods</span></span>
|<span data-ttu-id="610d5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="610d5-105">Method</span></span>|<span data-ttu-id="610d5-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="610d5-106">Return Type</span></span>|<span data-ttu-id="610d5-107">説明</span><span class="sxs-lookup"><span data-stu-id="610d5-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="610d5-108">managedDeviceMobileAppConfigurationUserSummary の取得</span><span class="sxs-lookup"><span data-stu-id="610d5-108">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_get.md)|[<span data-ttu-id="610d5-109">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="610d5-109">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="610d5-110">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="610d5-110">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="610d5-111">managedDeviceMobileAppConfigurationUserSummary の更新</span><span class="sxs-lookup"><span data-stu-id="610d5-111">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune_apps_manageddevicemobileappconfigurationusersummary_update.md)|[<span data-ttu-id="610d5-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="610d5-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="610d5-113">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="610d5-113">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="610d5-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="610d5-114">Properties</span></span>
|<span data-ttu-id="610d5-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="610d5-115">Property</span></span>|<span data-ttu-id="610d5-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="610d5-116">Type</span></span>|<span data-ttu-id="610d5-117">説明</span><span class="sxs-lookup"><span data-stu-id="610d5-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="610d5-118">id</span><span class="sxs-lookup"><span data-stu-id="610d5-118">id</span></span>|<span data-ttu-id="610d5-119">文字列</span><span class="sxs-lookup"><span data-stu-id="610d5-119">String</span></span>|<span data-ttu-id="610d5-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="610d5-120">Key of the entity.</span></span>|
|<span data-ttu-id="610d5-121">pendingCount</span><span class="sxs-lookup"><span data-stu-id="610d5-121">pendingCount</span></span>|<span data-ttu-id="610d5-122">Int32</span><span class="sxs-lookup"><span data-stu-id="610d5-122">Int32</span></span>|<span data-ttu-id="610d5-123">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="610d5-123">Number of pending Users</span></span>|
|<span data-ttu-id="610d5-124">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="610d5-124">notApplicableCount</span></span>|<span data-ttu-id="610d5-125">Int32</span><span class="sxs-lookup"><span data-stu-id="610d5-125">Int32</span></span>|<span data-ttu-id="610d5-126">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="610d5-126">Number of not applicable users.</span></span>|
|<span data-ttu-id="610d5-127">successCount</span><span class="sxs-lookup"><span data-stu-id="610d5-127">successCount</span></span>|<span data-ttu-id="610d5-128">Int32</span><span class="sxs-lookup"><span data-stu-id="610d5-128">Int32</span></span>|<span data-ttu-id="610d5-129">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="610d5-129">Number of succeeded Users</span></span>|
|<span data-ttu-id="610d5-130">errorCount</span><span class="sxs-lookup"><span data-stu-id="610d5-130">errorCount</span></span>|<span data-ttu-id="610d5-131">Int32</span><span class="sxs-lookup"><span data-stu-id="610d5-131">Int32</span></span>|<span data-ttu-id="610d5-132">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="610d5-132">Number of error Users</span></span>|
|<span data-ttu-id="610d5-133">failedCount</span><span class="sxs-lookup"><span data-stu-id="610d5-133">failedCount</span></span>|<span data-ttu-id="610d5-134">Int32</span><span class="sxs-lookup"><span data-stu-id="610d5-134">Int32</span></span>|<span data-ttu-id="610d5-135">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="610d5-135">Number of failed Users</span></span>|
|<span data-ttu-id="610d5-136">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="610d5-136">lastUpdateDateTime</span></span>|<span data-ttu-id="610d5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="610d5-137">DateTimeOffset</span></span>|<span data-ttu-id="610d5-138">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="610d5-138">Last update time</span></span>|
|<span data-ttu-id="610d5-139">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="610d5-139">configurationVersion</span></span>|<span data-ttu-id="610d5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="610d5-140">Int32</span></span>|<span data-ttu-id="610d5-141">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="610d5-141">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="610d5-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="610d5-142">Relationships</span></span>
<span data-ttu-id="610d5-143">なし</span><span class="sxs-lookup"><span data-stu-id="610d5-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="610d5-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="610d5-144">JSON Representation</span></span>
<span data-ttu-id="610d5-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="610d5-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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



