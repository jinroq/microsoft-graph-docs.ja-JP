# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="86644-101">deviceCompliancePolicySettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86644-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="86644-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="86644-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86644-103">特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="86644-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="86644-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86644-104">Properties</span></span>
|<span data-ttu-id="86644-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86644-105">Property</span></span>|<span data-ttu-id="86644-106">型</span><span class="sxs-lookup"><span data-stu-id="86644-106">Type</span></span>|<span data-ttu-id="86644-107">説明</span><span class="sxs-lookup"><span data-stu-id="86644-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86644-108">setting</span><span class="sxs-lookup"><span data-stu-id="86644-108">setting</span></span>|<span data-ttu-id="86644-109">String</span><span class="sxs-lookup"><span data-stu-id="86644-109">String</span></span>|<span data-ttu-id="86644-110">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="86644-110">The setting that is being reported</span></span>|
|<span data-ttu-id="86644-111">settingName</span><span class="sxs-lookup"><span data-stu-id="86644-111">settingName</span></span>|<span data-ttu-id="86644-112">String</span><span class="sxs-lookup"><span data-stu-id="86644-112">String</span></span>|<span data-ttu-id="86644-113">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="86644-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="86644-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="86644-114">instanceDisplayName</span></span>|<span data-ttu-id="86644-115">String</span><span class="sxs-lookup"><span data-stu-id="86644-115">String</span></span>|<span data-ttu-id="86644-116">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="86644-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="86644-117">state</span><span class="sxs-lookup"><span data-stu-id="86644-117">state</span></span>|[<span data-ttu-id="86644-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="86644-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="86644-119">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="86644-119">The compliance state of the setting.</span></span> <span data-ttu-id="86644-120">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="86644-120">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="86644-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="86644-121">errorCode</span></span>|<span data-ttu-id="86644-122">Int64</span><span class="sxs-lookup"><span data-stu-id="86644-122">Int64</span></span>|<span data-ttu-id="86644-123">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="86644-123">Error code for the setting</span></span>|
|<span data-ttu-id="86644-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="86644-124">errorDescription</span></span>|<span data-ttu-id="86644-125">String</span><span class="sxs-lookup"><span data-stu-id="86644-125">String</span></span>|<span data-ttu-id="86644-126">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="86644-126">Error description</span></span>|
|<span data-ttu-id="86644-127">userId</span><span class="sxs-lookup"><span data-stu-id="86644-127">userId</span></span>|<span data-ttu-id="86644-128">String</span><span class="sxs-lookup"><span data-stu-id="86644-128">String</span></span>|<span data-ttu-id="86644-129">UserId</span><span class="sxs-lookup"><span data-stu-id="86644-129">UserId</span></span>|
|<span data-ttu-id="86644-130">userName</span><span class="sxs-lookup"><span data-stu-id="86644-130">userName</span></span>|<span data-ttu-id="86644-131">String</span><span class="sxs-lookup"><span data-stu-id="86644-131">String</span></span>|<span data-ttu-id="86644-132">UserName</span><span class="sxs-lookup"><span data-stu-id="86644-132">UserName</span></span>|
|<span data-ttu-id="86644-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="86644-133">userEmail</span></span>|<span data-ttu-id="86644-134">String</span><span class="sxs-lookup"><span data-stu-id="86644-134">String</span></span>|<span data-ttu-id="86644-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="86644-135">UserEmail</span></span>|
|<span data-ttu-id="86644-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="86644-136">userPrincipalName</span></span>|<span data-ttu-id="86644-137">String</span><span class="sxs-lookup"><span data-stu-id="86644-137">String</span></span>|<span data-ttu-id="86644-138">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="86644-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="86644-139">ソース</span><span class="sxs-lookup"><span data-stu-id="86644-139">sources</span></span>|<span data-ttu-id="86644-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="86644-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="86644-141">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="86644-141">Contributing policies</span></span>|
|<span data-ttu-id="86644-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="86644-142">currentValue</span></span>|<span data-ttu-id="86644-143">String</span><span class="sxs-lookup"><span data-stu-id="86644-143">String</span></span>|<span data-ttu-id="86644-144">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="86644-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="86644-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86644-145">Relationships</span></span>
<span data-ttu-id="86644-146">なし</span><span class="sxs-lookup"><span data-stu-id="86644-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="86644-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86644-147">JSON Representation</span></span>
<span data-ttu-id="86644-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="86644-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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



