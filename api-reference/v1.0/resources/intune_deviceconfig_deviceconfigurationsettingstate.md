# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="f6e5a-101">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6e5a-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="f6e5a-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f6e5a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6e5a-103">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="f6e5a-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="f6e5a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6e5a-104">Properties</span></span>
|<span data-ttu-id="f6e5a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6e5a-105">Property</span></span>|<span data-ttu-id="f6e5a-106">型</span><span class="sxs-lookup"><span data-stu-id="f6e5a-106">Type</span></span>|<span data-ttu-id="f6e5a-107">説明</span><span class="sxs-lookup"><span data-stu-id="f6e5a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6e5a-108">setting</span><span class="sxs-lookup"><span data-stu-id="f6e5a-108">setting</span></span>|<span data-ttu-id="f6e5a-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6e5a-109">String</span></span>|<span data-ttu-id="f6e5a-110">レポートされる設定値。</span><span class="sxs-lookup"><span data-stu-id="f6e5a-110">The setting that is being reported</span></span>|
|<span data-ttu-id="f6e5a-111">settingName</span><span class="sxs-lookup"><span data-stu-id="f6e5a-111">settingName</span></span>|<span data-ttu-id="f6e5a-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6e5a-112">String</span></span>|<span data-ttu-id="f6e5a-113">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名</span><span class="sxs-lookup"><span data-stu-id="f6e5a-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="f6e5a-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f6e5a-114">instanceDisplayName</span></span>|<span data-ttu-id="f6e5a-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6e5a-115">String</span></span>|<span data-ttu-id="f6e5a-116">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="f6e5a-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="f6e5a-117">state</span><span class="sxs-lookup"><span data-stu-id="f6e5a-117">state</span></span>|<span data-ttu-id="f6e5a-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6e5a-118">String</span></span>|<span data-ttu-id="f6e5a-119">設定のコンプライアンス対応状態です。可能な値: `unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="f6e5a-119">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="f6e5a-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="f6e5a-120">errorCode</span></span>|<span data-ttu-id="f6e5a-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f6e5a-121">Int64</span></span>|<span data-ttu-id="f6e5a-122">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="f6e5a-122">Error code for the setting</span></span>|
|<span data-ttu-id="f6e5a-123">errorDescription</span><span class="sxs-lookup"><span data-stu-id="f6e5a-123">error_description</span></span>|<span data-ttu-id="f6e5a-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6e5a-124">String</span></span>|<span data-ttu-id="f6e5a-125">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="f6e5a-125">Error Description</span></span>|
|<span data-ttu-id="f6e5a-126">userId</span><span class="sxs-lookup"><span data-stu-id="f6e5a-126">userId</span></span>|<span data-ttu-id="f6e5a-127">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6e5a-127">String</span></span>|<span data-ttu-id="f6e5a-128">UserId</span><span class="sxs-lookup"><span data-stu-id="f6e5a-128">UserId</span></span>|
|<span data-ttu-id="f6e5a-129">userName</span><span class="sxs-lookup"><span data-stu-id="f6e5a-129">Username</span></span>|<span data-ttu-id="f6e5a-130">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6e5a-130">String</span></span>|<span data-ttu-id="f6e5a-131">UserName</span><span class="sxs-lookup"><span data-stu-id="f6e5a-131">UserName</span></span>|
|<span data-ttu-id="f6e5a-132">userEmail</span><span class="sxs-lookup"><span data-stu-id="f6e5a-132">?user_email=...</span></span>|<span data-ttu-id="f6e5a-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6e5a-133">String</span></span>|<span data-ttu-id="f6e5a-134">UserEmail</span><span class="sxs-lookup"><span data-stu-id="f6e5a-134">?user_email=...</span></span>|
|<span data-ttu-id="f6e5a-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6e5a-135">userPrincipalName</span></span>|<span data-ttu-id="f6e5a-136">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6e5a-136">String</span></span>|<span data-ttu-id="f6e5a-137">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f6e5a-137">userPrincipalName</span></span>|
|<span data-ttu-id="f6e5a-138">sources</span><span class="sxs-lookup"><span data-stu-id="f6e5a-138">Sources</span></span>|<span data-ttu-id="f6e5a-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f6e5a-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="f6e5a-140">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="f6e5a-140">Contributing policies</span></span>|
|<span data-ttu-id="f6e5a-141">currentValue</span><span class="sxs-lookup"><span data-stu-id="f6e5a-141">currentValue</span></span>|<span data-ttu-id="f6e5a-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6e5a-142">String</span></span>|<span data-ttu-id="f6e5a-143">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="f6e5a-143">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6e5a-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f6e5a-144">Relationships</span></span>
<span data-ttu-id="f6e5a-145">なし</span><span class="sxs-lookup"><span data-stu-id="f6e5a-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f6e5a-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6e5a-146">JSON Representation</span></span>
<span data-ttu-id="f6e5a-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f6e5a-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



