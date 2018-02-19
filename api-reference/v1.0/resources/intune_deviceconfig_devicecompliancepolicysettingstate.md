# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="04f4f-101">deviceCompliancePolicySettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04f4f-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="04f4f-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04f4f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04f4f-103">特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="04f4f-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="04f4f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04f4f-104">Properties</span></span>
|<span data-ttu-id="04f4f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04f4f-105">Property</span></span>|<span data-ttu-id="04f4f-106">型</span><span class="sxs-lookup"><span data-stu-id="04f4f-106">Type</span></span>|<span data-ttu-id="04f4f-107">説明</span><span class="sxs-lookup"><span data-stu-id="04f4f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04f4f-108">setting</span><span class="sxs-lookup"><span data-stu-id="04f4f-108">setting</span></span>|<span data-ttu-id="04f4f-109">String</span><span class="sxs-lookup"><span data-stu-id="04f4f-109">String</span></span>|<span data-ttu-id="04f4f-110">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="04f4f-110">The setting that is being reported</span></span>|
|<span data-ttu-id="04f4f-111">settingName</span><span class="sxs-lookup"><span data-stu-id="04f4f-111">settingName</span></span>|<span data-ttu-id="04f4f-112">String</span><span class="sxs-lookup"><span data-stu-id="04f4f-112">String</span></span>|<span data-ttu-id="04f4f-113">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="04f4f-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="04f4f-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="04f4f-114">instanceDisplayName</span></span>|<span data-ttu-id="04f4f-115">String</span><span class="sxs-lookup"><span data-stu-id="04f4f-115">String</span></span>|<span data-ttu-id="04f4f-116">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="04f4f-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="04f4f-117">state</span><span class="sxs-lookup"><span data-stu-id="04f4f-117">state</span></span>|<span data-ttu-id="04f4f-118">String</span><span class="sxs-lookup"><span data-stu-id="04f4f-118">String</span></span>|<span data-ttu-id="04f4f-119">設定のコンプライアンス対応状態です。可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="04f4f-119">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="04f4f-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="04f4f-120">errorCode</span></span>|<span data-ttu-id="04f4f-121">Int64</span><span class="sxs-lookup"><span data-stu-id="04f4f-121">Int64</span></span>|<span data-ttu-id="04f4f-122">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="04f4f-122">Error code for the setting</span></span>|
|<span data-ttu-id="04f4f-123">errorDescription</span><span class="sxs-lookup"><span data-stu-id="04f4f-123">error_description</span></span>|<span data-ttu-id="04f4f-124">String</span><span class="sxs-lookup"><span data-stu-id="04f4f-124">String</span></span>|<span data-ttu-id="04f4f-125">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="04f4f-125">Error Description</span></span>|
|<span data-ttu-id="04f4f-126">userId</span><span class="sxs-lookup"><span data-stu-id="04f4f-126">userId</span></span>|<span data-ttu-id="04f4f-127">String</span><span class="sxs-lookup"><span data-stu-id="04f4f-127">String</span></span>|<span data-ttu-id="04f4f-128">UserId</span><span class="sxs-lookup"><span data-stu-id="04f4f-128">UserId</span></span>|
|<span data-ttu-id="04f4f-129">userName</span><span class="sxs-lookup"><span data-stu-id="04f4f-129">Username</span></span>|<span data-ttu-id="04f4f-130">String</span><span class="sxs-lookup"><span data-stu-id="04f4f-130">String</span></span>|<span data-ttu-id="04f4f-131">UserName</span><span class="sxs-lookup"><span data-stu-id="04f4f-131">UserName</span></span>|
|<span data-ttu-id="04f4f-132">userEmail</span><span class="sxs-lookup"><span data-stu-id="04f4f-132">?user_email=...</span></span>|<span data-ttu-id="04f4f-133">String</span><span class="sxs-lookup"><span data-stu-id="04f4f-133">String</span></span>|<span data-ttu-id="04f4f-134">UserEmail</span><span class="sxs-lookup"><span data-stu-id="04f4f-134">?user_email=...</span></span>|
|<span data-ttu-id="04f4f-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="04f4f-135">userPrincipalName</span></span>|<span data-ttu-id="04f4f-136">String</span><span class="sxs-lookup"><span data-stu-id="04f4f-136">String</span></span>|<span data-ttu-id="04f4f-137">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="04f4f-137">userPrincipalName</span></span>|
|<span data-ttu-id="04f4f-138">ソース</span><span class="sxs-lookup"><span data-stu-id="04f4f-138">Sources</span></span>|<span data-ttu-id="04f4f-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="04f4f-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="04f4f-140">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="04f4f-140">Contributing policies</span></span>|
|<span data-ttu-id="04f4f-141">currentValue</span><span class="sxs-lookup"><span data-stu-id="04f4f-141">currentValue</span></span>|<span data-ttu-id="04f4f-142">String</span><span class="sxs-lookup"><span data-stu-id="04f4f-142">String</span></span>|<span data-ttu-id="04f4f-143">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="04f4f-143">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="04f4f-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="04f4f-144">Relationships</span></span>
<span data-ttu-id="04f4f-145">なし</span><span class="sxs-lookup"><span data-stu-id="04f4f-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04f4f-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04f4f-146">JSON Representation</span></span>
<span data-ttu-id="04f4f-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04f4f-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



