# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="f1db8-101">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1db8-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="f1db8-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1db8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1db8-103">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="f1db8-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="f1db8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1db8-104">Properties</span></span>
|<span data-ttu-id="f1db8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1db8-105">Property</span></span>|<span data-ttu-id="f1db8-106">型</span><span class="sxs-lookup"><span data-stu-id="f1db8-106">Type</span></span>|<span data-ttu-id="f1db8-107">説明</span><span class="sxs-lookup"><span data-stu-id="f1db8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1db8-108">setting</span><span class="sxs-lookup"><span data-stu-id="f1db8-108">setting</span></span>|<span data-ttu-id="f1db8-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f1db8-109">String</span></span>|<span data-ttu-id="f1db8-110">レポートされる設定値。</span><span class="sxs-lookup"><span data-stu-id="f1db8-110">The setting that is being reported</span></span>|
|<span data-ttu-id="f1db8-111">settingName</span><span class="sxs-lookup"><span data-stu-id="f1db8-111">settingName</span></span>|<span data-ttu-id="f1db8-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f1db8-112">String</span></span>|<span data-ttu-id="f1db8-113">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名</span><span class="sxs-lookup"><span data-stu-id="f1db8-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="f1db8-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1db8-114">instanceDisplayName</span></span>|<span data-ttu-id="f1db8-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f1db8-115">String</span></span>|<span data-ttu-id="f1db8-116">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="f1db8-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="f1db8-117">state</span><span class="sxs-lookup"><span data-stu-id="f1db8-117">state</span></span>|[<span data-ttu-id="f1db8-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f1db8-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="f1db8-119">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="f1db8-119">The compliance state of the setting.</span></span> <span data-ttu-id="f1db8-120">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="f1db8-120">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f1db8-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="f1db8-121">errorCode</span></span>|<span data-ttu-id="f1db8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f1db8-122">Int64</span></span>|<span data-ttu-id="f1db8-123">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="f1db8-123">Error code for the setting</span></span>|
|<span data-ttu-id="f1db8-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="f1db8-124">errorDescription</span></span>|<span data-ttu-id="f1db8-125">String</span><span class="sxs-lookup"><span data-stu-id="f1db8-125">String</span></span>|<span data-ttu-id="f1db8-126">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="f1db8-126">Error description</span></span>|
|<span data-ttu-id="f1db8-127">userId</span><span class="sxs-lookup"><span data-stu-id="f1db8-127">userId</span></span>|<span data-ttu-id="f1db8-128">String</span><span class="sxs-lookup"><span data-stu-id="f1db8-128">String</span></span>|<span data-ttu-id="f1db8-129">UserId</span><span class="sxs-lookup"><span data-stu-id="f1db8-129">UserId</span></span>|
|<span data-ttu-id="f1db8-130">userName</span><span class="sxs-lookup"><span data-stu-id="f1db8-130">userName</span></span>|<span data-ttu-id="f1db8-131">String</span><span class="sxs-lookup"><span data-stu-id="f1db8-131">String</span></span>|<span data-ttu-id="f1db8-132">UserName</span><span class="sxs-lookup"><span data-stu-id="f1db8-132">UserName</span></span>|
|<span data-ttu-id="f1db8-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="f1db8-133">userEmail</span></span>|<span data-ttu-id="f1db8-134">String</span><span class="sxs-lookup"><span data-stu-id="f1db8-134">String</span></span>|<span data-ttu-id="f1db8-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="f1db8-135">UserEmail</span></span>|
|<span data-ttu-id="f1db8-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1db8-136">userPrincipalName</span></span>|<span data-ttu-id="f1db8-137">String</span><span class="sxs-lookup"><span data-stu-id="f1db8-137">String</span></span>|<span data-ttu-id="f1db8-138">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f1db8-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="f1db8-139">ソース</span><span class="sxs-lookup"><span data-stu-id="f1db8-139">sources</span></span>|<span data-ttu-id="f1db8-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f1db8-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="f1db8-141">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="f1db8-141">Contributing policies</span></span>|
|<span data-ttu-id="f1db8-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="f1db8-142">currentValue</span></span>|<span data-ttu-id="f1db8-143">String</span><span class="sxs-lookup"><span data-stu-id="f1db8-143">String</span></span>|<span data-ttu-id="f1db8-144">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="f1db8-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1db8-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f1db8-145">Relationships</span></span>
<span data-ttu-id="f1db8-146">なし</span><span class="sxs-lookup"><span data-stu-id="f1db8-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1db8-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1db8-147">JSON Representation</span></span>
<span data-ttu-id="f1db8-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f1db8-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



