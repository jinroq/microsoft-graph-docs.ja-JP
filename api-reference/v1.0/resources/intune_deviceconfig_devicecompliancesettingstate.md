# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="1dfbf-101">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="1dfbf-101">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="1dfbf-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1dfbf-103">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-103">Device compliance setting State for a given device.</span></span>
## <a name="methods"></a><span data-ttu-id="1dfbf-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="1dfbf-104">Methods</span></span>
|<span data-ttu-id="1dfbf-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1dfbf-105">Method</span></span>|<span data-ttu-id="1dfbf-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1dfbf-106">Return Type</span></span>|<span data-ttu-id="1dfbf-107">説明</span><span class="sxs-lookup"><span data-stu-id="1dfbf-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1dfbf-108">deviceComplianceSettingStates のリスト</span><span class="sxs-lookup"><span data-stu-id="1dfbf-108">List deviceComplianceSettingStates</span></span>](../api/intune_deviceconfig_devicecompliancesettingstate_list.md)|<span data-ttu-id="1dfbf-109">[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1dfbf-109">[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="1dfbf-110">[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-110">List properties and relationships of the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="1dfbf-111">deviceComplianceSettingState の取得</span><span class="sxs-lookup"><span data-stu-id="1dfbf-111">Get deviceComplianceSettingState</span></span>](../api/intune_deviceconfig_devicecompliancesettingstate_get.md)|[<span data-ttu-id="1dfbf-112">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1dfbf-112">deviceComplianceSettingState</span></span>](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|<span data-ttu-id="1dfbf-113">[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-113">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="1dfbf-114">deviceComplianceSettingState の作成</span><span class="sxs-lookup"><span data-stu-id="1dfbf-114">Create deviceComplianceSettingState</span></span>](../api/intune_deviceconfig_devicecompliancesettingstate_create.md)|[<span data-ttu-id="1dfbf-115">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1dfbf-115">deviceComplianceSettingState</span></span>](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|<span data-ttu-id="1dfbf-116">新しい [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-116">Create a new [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="1dfbf-117">deviceComplianceSettingState の削除</span><span class="sxs-lookup"><span data-stu-id="1dfbf-117">Delete deviceComplianceSettingState</span></span>](../api/intune_deviceconfig_devicecompliancesettingstate_delete.md)|<span data-ttu-id="1dfbf-118">なし</span><span class="sxs-lookup"><span data-stu-id="1dfbf-118">None</span></span>|<span data-ttu-id="1dfbf-119">[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-119">Deletes a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="1dfbf-120">deviceComplianceSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="1dfbf-120">Update deviceComplianceSettingState</span></span>](../api/intune_deviceconfig_devicecompliancesettingstate_update.md)|[<span data-ttu-id="1dfbf-121">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1dfbf-121">deviceComplianceSettingState</span></span>](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|<span data-ttu-id="1dfbf-122">[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-122">Update the properties of a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1dfbf-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dfbf-123">Properties</span></span>
|<span data-ttu-id="1dfbf-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dfbf-124">Property</span></span>|<span data-ttu-id="1dfbf-125">タイプ</span><span class="sxs-lookup"><span data-stu-id="1dfbf-125">Type</span></span>|<span data-ttu-id="1dfbf-126">説明</span><span class="sxs-lookup"><span data-stu-id="1dfbf-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dfbf-127">ID</span><span class="sxs-lookup"><span data-stu-id="1dfbf-127">id</span></span>|<span data-ttu-id="1dfbf-128">文字列</span><span class="sxs-lookup"><span data-stu-id="1dfbf-128">String</span></span>|<span data-ttu-id="1dfbf-129">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="1dfbf-129">Key of the entity</span></span>|
|<span data-ttu-id="1dfbf-130">setting</span><span class="sxs-lookup"><span data-stu-id="1dfbf-130">setting</span></span>|<span data-ttu-id="1dfbf-131">文字列</span><span class="sxs-lookup"><span data-stu-id="1dfbf-131">String</span></span>|<span data-ttu-id="1dfbf-132">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-132">The setting class name and property name.</span></span>|
|<span data-ttu-id="1dfbf-133">settingName</span><span class="sxs-lookup"><span data-stu-id="1dfbf-133">settingName</span></span>|<span data-ttu-id="1dfbf-134">文字列</span><span class="sxs-lookup"><span data-stu-id="1dfbf-134">String</span></span>|<span data-ttu-id="1dfbf-135">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-135">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="1dfbf-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="1dfbf-136">deviceId</span></span>|<span data-ttu-id="1dfbf-137">文字列</span><span class="sxs-lookup"><span data-stu-id="1dfbf-137">String</span></span>|<span data-ttu-id="1dfbf-138">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-138">The Device Id that is being reported</span></span>|
|<span data-ttu-id="1dfbf-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="1dfbf-139">deviceName</span></span>|<span data-ttu-id="1dfbf-140">文字列</span><span class="sxs-lookup"><span data-stu-id="1dfbf-140">String</span></span>|<span data-ttu-id="1dfbf-141">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-141">The Device Name that is being reported</span></span>|
|<span data-ttu-id="1dfbf-142">userId</span><span class="sxs-lookup"><span data-stu-id="1dfbf-142">userId</span></span>|<span data-ttu-id="1dfbf-143">文字列</span><span class="sxs-lookup"><span data-stu-id="1dfbf-143">String</span></span>|<span data-ttu-id="1dfbf-144">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="1dfbf-144">The user Id that is being reported</span></span>|
|<span data-ttu-id="1dfbf-145">userEmail</span><span class="sxs-lookup"><span data-stu-id="1dfbf-145">userEmail</span></span>|<span data-ttu-id="1dfbf-146">文字列</span><span class="sxs-lookup"><span data-stu-id="1dfbf-146">String</span></span>|<span data-ttu-id="1dfbf-147">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-147">The User email address that is being reported</span></span>|
|<span data-ttu-id="1dfbf-148">userName</span><span class="sxs-lookup"><span data-stu-id="1dfbf-148">userName</span></span>|<span data-ttu-id="1dfbf-149">文字列</span><span class="sxs-lookup"><span data-stu-id="1dfbf-149">String</span></span>|<span data-ttu-id="1dfbf-150">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="1dfbf-150">The User Name that is being reported</span></span>|
|<span data-ttu-id="1dfbf-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1dfbf-151">userPrincipalName</span></span>|<span data-ttu-id="1dfbf-152">文字列</span><span class="sxs-lookup"><span data-stu-id="1dfbf-152">String</span></span>|<span data-ttu-id="1dfbf-153">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="1dfbf-153">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="1dfbf-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1dfbf-154">deviceModel</span></span>|<span data-ttu-id="1dfbf-155">文字列</span><span class="sxs-lookup"><span data-stu-id="1dfbf-155">String</span></span>|<span data-ttu-id="1dfbf-156">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="1dfbf-156">The device model that is being reported</span></span>|
|<span data-ttu-id="1dfbf-157">state</span><span class="sxs-lookup"><span data-stu-id="1dfbf-157">state</span></span>|[<span data-ttu-id="1dfbf-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1dfbf-158">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="1dfbf-p101">設定のコンプライアンスの状態です。使用可能な値は `unknown`、 `notApplicable`、 `compliant`、 `remediated`、 `nonCompliant`、 `error`、 `conflict`、 `notAssigned`です。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-p101">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="1dfbf-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1dfbf-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1dfbf-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dfbf-162">DateTimeOffset</span></span>|<span data-ttu-id="1dfbf-163">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="1dfbf-163">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dfbf-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1dfbf-164">Relationships</span></span>
<span data-ttu-id="1dfbf-165">なし</span><span class="sxs-lookup"><span data-stu-id="1dfbf-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1dfbf-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1dfbf-166">JSON Representation</span></span>
<span data-ttu-id="1dfbf-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1dfbf-167">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```








