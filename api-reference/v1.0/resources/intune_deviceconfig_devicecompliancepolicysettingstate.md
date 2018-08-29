# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="500e3-101">deviceCompliancePolicySettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="500e3-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="500e3-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="500e3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="500e3-103">特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="500e3-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="500e3-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="500e3-104">Properties</span></span>
|<span data-ttu-id="500e3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="500e3-105">Property</span></span>|<span data-ttu-id="500e3-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="500e3-106">Type</span></span>|<span data-ttu-id="500e3-107">説明</span><span class="sxs-lookup"><span data-stu-id="500e3-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="500e3-108">setting</span><span class="sxs-lookup"><span data-stu-id="500e3-108">setting</span></span>|<span data-ttu-id="500e3-109">文字列</span><span class="sxs-lookup"><span data-stu-id="500e3-109">String</span></span>|<span data-ttu-id="500e3-110">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="500e3-110">The setting that is being reported</span></span>|
|<span data-ttu-id="500e3-111">settingName</span><span class="sxs-lookup"><span data-stu-id="500e3-111">settingName</span></span>|<span data-ttu-id="500e3-112">文字列</span><span class="sxs-lookup"><span data-stu-id="500e3-112">String</span></span>|<span data-ttu-id="500e3-113">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="500e3-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="500e3-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="500e3-114">instanceDisplayName</span></span>|<span data-ttu-id="500e3-115">文字列</span><span class="sxs-lookup"><span data-stu-id="500e3-115">String</span></span>|<span data-ttu-id="500e3-116">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="500e3-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="500e3-117">state</span><span class="sxs-lookup"><span data-stu-id="500e3-117">state</span></span>|[<span data-ttu-id="500e3-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="500e3-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="500e3-119">設定のコンプライアンス状態です。</span><span class="sxs-lookup"><span data-stu-id="500e3-119">The compliance state of the setting Possible values are: , , , , , , .</span></span> <span data-ttu-id="500e3-120">指定できる値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="500e3-120">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="500e3-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="500e3-121">errorCode</span></span>|<span data-ttu-id="500e3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="500e3-122">Int64</span></span>|<span data-ttu-id="500e3-123">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="500e3-123">Error code for the setting</span></span>|
|<span data-ttu-id="500e3-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="500e3-124">errorDescription</span></span>|<span data-ttu-id="500e3-125">文字列</span><span class="sxs-lookup"><span data-stu-id="500e3-125">String</span></span>|<span data-ttu-id="500e3-126">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="500e3-126">Error description</span></span>|
|<span data-ttu-id="500e3-127">userId</span><span class="sxs-lookup"><span data-stu-id="500e3-127">userId</span></span>|<span data-ttu-id="500e3-128">文字列</span><span class="sxs-lookup"><span data-stu-id="500e3-128">String</span></span>|<span data-ttu-id="500e3-129">UserId</span><span class="sxs-lookup"><span data-stu-id="500e3-129">UserId</span></span>|
|<span data-ttu-id="500e3-130">userName</span><span class="sxs-lookup"><span data-stu-id="500e3-130">userName</span></span>|<span data-ttu-id="500e3-131">文字列</span><span class="sxs-lookup"><span data-stu-id="500e3-131">String</span></span>|<span data-ttu-id="500e3-132">UserName</span><span class="sxs-lookup"><span data-stu-id="500e3-132">UserName</span></span>|
|<span data-ttu-id="500e3-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="500e3-133">userEmail</span></span>|<span data-ttu-id="500e3-134">文字列</span><span class="sxs-lookup"><span data-stu-id="500e3-134">String</span></span>|<span data-ttu-id="500e3-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="500e3-135">UserEmail</span></span>|
|<span data-ttu-id="500e3-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="500e3-136">userPrincipalName</span></span>|<span data-ttu-id="500e3-137">文字列</span><span class="sxs-lookup"><span data-stu-id="500e3-137">String</span></span>|<span data-ttu-id="500e3-138">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="500e3-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="500e3-139">ソース</span><span class="sxs-lookup"><span data-stu-id="500e3-139">sources</span></span>|<span data-ttu-id="500e3-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="500e3-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="500e3-141">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="500e3-141">Contributing policies</span></span>|
|<span data-ttu-id="500e3-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="500e3-142">currentValue</span></span>|<span data-ttu-id="500e3-143">文字列</span><span class="sxs-lookup"><span data-stu-id="500e3-143">String</span></span>|<span data-ttu-id="500e3-144">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="500e3-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="500e3-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="500e3-145">Relationships</span></span>
<span data-ttu-id="500e3-146">なし</span><span class="sxs-lookup"><span data-stu-id="500e3-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="500e3-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="500e3-147">JSON Representation</span></span>
<span data-ttu-id="500e3-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="500e3-148">Here is a JSON representation of the resource.</span></span>
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



