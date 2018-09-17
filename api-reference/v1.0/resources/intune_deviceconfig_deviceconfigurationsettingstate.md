# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="1cd92-101">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1cd92-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="1cd92-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1cd92-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cd92-103">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="1cd92-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="1cd92-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cd92-104">Properties</span></span>
|<span data-ttu-id="1cd92-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cd92-105">Property</span></span>|<span data-ttu-id="1cd92-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="1cd92-106">Type</span></span>|<span data-ttu-id="1cd92-107">説明</span><span class="sxs-lookup"><span data-stu-id="1cd92-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd92-108">文字列</span><span class="sxs-lookup"><span data-stu-id="1cd92-108">setting</span></span>|<span data-ttu-id="1cd92-109">文字列</span><span class="sxs-lookup"><span data-stu-id="1cd92-109">String</span></span>|<span data-ttu-id="1cd92-110">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="1cd92-110">The setting that is being reported</span></span>|
|<span data-ttu-id="1cd92-111">settingName</span><span class="sxs-lookup"><span data-stu-id="1cd92-111">settingName</span></span>|<span data-ttu-id="1cd92-112">文字列</span><span class="sxs-lookup"><span data-stu-id="1cd92-112">String</span></span>|<span data-ttu-id="1cd92-113">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="1cd92-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="1cd92-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1cd92-114">instanceDisplayName</span></span>|<span data-ttu-id="1cd92-115">文字列</span><span class="sxs-lookup"><span data-stu-id="1cd92-115">String</span></span>|<span data-ttu-id="1cd92-116">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="1cd92-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="1cd92-117">都道府県</span><span class="sxs-lookup"><span data-stu-id="1cd92-117">state</span></span>|[<span data-ttu-id="1cd92-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1cd92-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="1cd92-p101">設定のコンプライアンスの状態です。使用可能な値は `unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="1cd92-p101">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="1cd92-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="1cd92-121">errorCode</span></span>|<span data-ttu-id="1cd92-122">Int64</span><span class="sxs-lookup"><span data-stu-id="1cd92-122">Int64</span></span>|<span data-ttu-id="1cd92-123">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="1cd92-123">Error code for the setting</span></span>|
|<span data-ttu-id="1cd92-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="1cd92-124">errorDescription</span></span>|<span data-ttu-id="1cd92-125">文字列</span><span class="sxs-lookup"><span data-stu-id="1cd92-125">String</span></span>|<span data-ttu-id="1cd92-126">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="1cd92-126">Error description</span></span>|
|<span data-ttu-id="1cd92-127">userId</span><span class="sxs-lookup"><span data-stu-id="1cd92-127">userId</span></span>|<span data-ttu-id="1cd92-128">文字列</span><span class="sxs-lookup"><span data-stu-id="1cd92-128">String</span></span>|<span data-ttu-id="1cd92-129">UserId</span><span class="sxs-lookup"><span data-stu-id="1cd92-129">UserId</span></span>|
|<span data-ttu-id="1cd92-130">userName</span><span class="sxs-lookup"><span data-stu-id="1cd92-130">userName</span></span>|<span data-ttu-id="1cd92-131">文字列</span><span class="sxs-lookup"><span data-stu-id="1cd92-131">String</span></span>|<span data-ttu-id="1cd92-132">userName</span><span class="sxs-lookup"><span data-stu-id="1cd92-132">UserName</span></span>|
|<span data-ttu-id="1cd92-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="1cd92-133">userEmail</span></span>|<span data-ttu-id="1cd92-134">文字列</span><span class="sxs-lookup"><span data-stu-id="1cd92-134">String</span></span>|<span data-ttu-id="1cd92-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="1cd92-135">UserEmail</span></span>|
|<span data-ttu-id="1cd92-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1cd92-136">userPrincipalName</span></span>|<span data-ttu-id="1cd92-137">文字列</span><span class="sxs-lookup"><span data-stu-id="1cd92-137">String</span></span>|<span data-ttu-id="1cd92-138">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="1cd92-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="1cd92-139">ソース</span><span class="sxs-lookup"><span data-stu-id="1cd92-139">sources</span></span>|<span data-ttu-id="1cd92-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1cd92-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="1cd92-141">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="1cd92-141">Contributing policies</span></span>|
|<span data-ttu-id="1cd92-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="1cd92-142">currentValue</span></span>|<span data-ttu-id="1cd92-143">文字列</span><span class="sxs-lookup"><span data-stu-id="1cd92-143">String</span></span>|<span data-ttu-id="1cd92-144">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="1cd92-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cd92-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1cd92-145">Relationships</span></span>
<span data-ttu-id="1cd92-146">なし</span><span class="sxs-lookup"><span data-stu-id="1cd92-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1cd92-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1cd92-147">JSON Representation</span></span>
<span data-ttu-id="1cd92-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1cd92-148">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}-->
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








