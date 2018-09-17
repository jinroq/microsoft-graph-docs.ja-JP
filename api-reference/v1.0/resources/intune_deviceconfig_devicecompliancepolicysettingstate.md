# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="fde5d-101">deviceCompliancePolicySettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fde5d-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="fde5d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fde5d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fde5d-103">特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="fde5d-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="fde5d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fde5d-104">Properties</span></span>
|<span data-ttu-id="fde5d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fde5d-105">Property</span></span>|<span data-ttu-id="fde5d-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="fde5d-106">Type</span></span>|<span data-ttu-id="fde5d-107">説明</span><span class="sxs-lookup"><span data-stu-id="fde5d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fde5d-108">setting</span><span class="sxs-lookup"><span data-stu-id="fde5d-108">setting</span></span>|<span data-ttu-id="fde5d-109">文字列</span><span class="sxs-lookup"><span data-stu-id="fde5d-109">String</span></span>|<span data-ttu-id="fde5d-110">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="fde5d-110">The setting that is being reported</span></span>|
|<span data-ttu-id="fde5d-111">settingName</span><span class="sxs-lookup"><span data-stu-id="fde5d-111">settingName</span></span>|<span data-ttu-id="fde5d-112">文字列</span><span class="sxs-lookup"><span data-stu-id="fde5d-112">String</span></span>|<span data-ttu-id="fde5d-113">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="fde5d-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="fde5d-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="fde5d-114">instanceDisplayName</span></span>|<span data-ttu-id="fde5d-115">文字列</span><span class="sxs-lookup"><span data-stu-id="fde5d-115">String</span></span>|<span data-ttu-id="fde5d-116">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="fde5d-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="fde5d-117">state</span><span class="sxs-lookup"><span data-stu-id="fde5d-117">state</span></span>|[<span data-ttu-id="fde5d-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="fde5d-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="fde5d-p101">設定のコンプライアンスの状態です。使用可能な値は `unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="fde5d-p101">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="fde5d-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="fde5d-121">errorCode</span></span>|<span data-ttu-id="fde5d-122">Int64</span><span class="sxs-lookup"><span data-stu-id="fde5d-122">Int64</span></span>|<span data-ttu-id="fde5d-123">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="fde5d-123">Error code for the setting</span></span>|
|<span data-ttu-id="fde5d-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="fde5d-124">errorDescription</span></span>|<span data-ttu-id="fde5d-125">文字列</span><span class="sxs-lookup"><span data-stu-id="fde5d-125">String</span></span>|<span data-ttu-id="fde5d-126">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="fde5d-126">Error description</span></span>|
|<span data-ttu-id="fde5d-127">userId</span><span class="sxs-lookup"><span data-stu-id="fde5d-127">userId</span></span>|<span data-ttu-id="fde5d-128">文字列</span><span class="sxs-lookup"><span data-stu-id="fde5d-128">String</span></span>|<span data-ttu-id="fde5d-129">UserId</span><span class="sxs-lookup"><span data-stu-id="fde5d-129">UserId</span></span>|
|<span data-ttu-id="fde5d-130">userName</span><span class="sxs-lookup"><span data-stu-id="fde5d-130">userName</span></span>|<span data-ttu-id="fde5d-131">文字列</span><span class="sxs-lookup"><span data-stu-id="fde5d-131">String</span></span>|<span data-ttu-id="fde5d-132">UserName</span><span class="sxs-lookup"><span data-stu-id="fde5d-132">UserName</span></span>|
|<span data-ttu-id="fde5d-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="fde5d-133">userEmail</span></span>|<span data-ttu-id="fde5d-134">文字列</span><span class="sxs-lookup"><span data-stu-id="fde5d-134">String</span></span>|<span data-ttu-id="fde5d-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="fde5d-135">UserEmail</span></span>|
|<span data-ttu-id="fde5d-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fde5d-136">userPrincipalName</span></span>|<span data-ttu-id="fde5d-137">文字列</span><span class="sxs-lookup"><span data-stu-id="fde5d-137">String</span></span>|<span data-ttu-id="fde5d-138">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="fde5d-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="fde5d-139">ソース</span><span class="sxs-lookup"><span data-stu-id="fde5d-139">sources</span></span>|<span data-ttu-id="fde5d-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fde5d-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="fde5d-141">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="fde5d-141">Contributing policies</span></span>|
|<span data-ttu-id="fde5d-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="fde5d-142">currentValue</span></span>|<span data-ttu-id="fde5d-143">文字列</span><span class="sxs-lookup"><span data-stu-id="fde5d-143">String</span></span>|<span data-ttu-id="fde5d-144">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="fde5d-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="fde5d-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fde5d-145">Relationships</span></span>
<span data-ttu-id="fde5d-146">なし</span><span class="sxs-lookup"><span data-stu-id="fde5d-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fde5d-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fde5d-147">JSON Representation</span></span>
<span data-ttu-id="fde5d-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fde5d-148">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}-->
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








