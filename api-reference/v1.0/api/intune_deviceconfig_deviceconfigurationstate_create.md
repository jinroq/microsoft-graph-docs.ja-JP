# <a name="create-deviceconfigurationstate"></a><span data-ttu-id="2dfbd-101">deviceConfigurationState の作成</span><span class="sxs-lookup"><span data-stu-id="2dfbd-101">Create deviceConfigurationState</span></span>

> <span data-ttu-id="2dfbd-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2dfbd-103">新しい [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-103">Create a new [plannerBucket](../resources/intune_deviceconfig_deviceconfigurationstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2dfbd-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2dfbd-104">Prerequisites</span></span>
<span data-ttu-id="2dfbd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2dfbd-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2dfbd-107">Permission type</span></span>|<span data-ttu-id="2dfbd-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2dfbd-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dfbd-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2dfbd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2dfbd-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dfbd-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2dfbd-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2dfbd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dfbd-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-112">Not supported.</span></span>|
|<span data-ttu-id="2dfbd-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2dfbd-113">Application</span></span>|<span data-ttu-id="2dfbd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dfbd-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2dfbd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /managedDevices/{managedDevicesId}/deviceConfigurationStates
```

## <a name="request-headers"></a><span data-ttu-id="2dfbd-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2dfbd-116">Request headers</span></span>
|<span data-ttu-id="2dfbd-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2dfbd-117">Header</span></span>|<span data-ttu-id="2dfbd-118">値</span><span class="sxs-lookup"><span data-stu-id="2dfbd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2dfbd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2dfbd-119">Authorization</span></span>|<span data-ttu-id="2dfbd-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2dfbd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2dfbd-121">Accept</span></span>|<span data-ttu-id="2dfbd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2dfbd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dfbd-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2dfbd-123">Request body</span></span>
<span data-ttu-id="2dfbd-124">要求本文で、deviceConfigurationState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="2dfbd-125">次の表に、deviceConfigurationState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="2dfbd-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2dfbd-126">Property</span></span>|<span data-ttu-id="2dfbd-127">型</span><span class="sxs-lookup"><span data-stu-id="2dfbd-127">Type</span></span>|<span data-ttu-id="2dfbd-128">説明</span><span class="sxs-lookup"><span data-stu-id="2dfbd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dfbd-129">id</span><span class="sxs-lookup"><span data-stu-id="2dfbd-129">id</span></span>|<span data-ttu-id="2dfbd-130">String</span><span class="sxs-lookup"><span data-stu-id="2dfbd-130">String</span></span>|<span data-ttu-id="2dfbd-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-131">Name of the entity.</span></span>|
|<span data-ttu-id="2dfbd-132">settingStates</span><span class="sxs-lookup"><span data-stu-id="2dfbd-132">settingStates</span></span>|<span data-ttu-id="2dfbd-133">[deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2dfbd-133">[deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md) collection</span></span>|<span data-ttu-id="2dfbd-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2dfbd-134">Not yet documented</span></span>|
|<span data-ttu-id="2dfbd-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2dfbd-135">displayName</span></span>|<span data-ttu-id="2dfbd-136">String</span><span class="sxs-lookup"><span data-stu-id="2dfbd-136">String</span></span>|<span data-ttu-id="2dfbd-137">この policyBase のポリシーの名前</span><span class="sxs-lookup"><span data-stu-id="2dfbd-137">The friendly name of the DLP policy for this event.</span></span>|
|<span data-ttu-id="2dfbd-138">version</span><span class="sxs-lookup"><span data-stu-id="2dfbd-138">version</span></span>|<span data-ttu-id="2dfbd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2dfbd-139">Int32</span></span>|<span data-ttu-id="2dfbd-140">ポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="2dfbd-140">The version of the policy</span></span>|
|<span data-ttu-id="2dfbd-141">platformType</span><span class="sxs-lookup"><span data-stu-id="2dfbd-141">PlatformType</span></span>|<span data-ttu-id="2dfbd-142">String</span><span class="sxs-lookup"><span data-stu-id="2dfbd-142">String</span></span>|<span data-ttu-id="2dfbd-143">ポリシーが適用されるプラットフォームの種類。可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-143">Platform type that the policy applies to Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="2dfbd-144">state</span><span class="sxs-lookup"><span data-stu-id="2dfbd-144">state</span></span>|<span data-ttu-id="2dfbd-145">String</span><span class="sxs-lookup"><span data-stu-id="2dfbd-145">String</span></span>|<span data-ttu-id="2dfbd-146">ポリシーのコンプライアンス対応状態。可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-146">The compliance state of the policy Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="2dfbd-147">settingCount</span><span class="sxs-lookup"><span data-stu-id="2dfbd-147">settingCount</span></span>|<span data-ttu-id="2dfbd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2dfbd-148">Int32</span></span>|<span data-ttu-id="2dfbd-149">ポリシーが保持する設定の数</span><span class="sxs-lookup"><span data-stu-id="2dfbd-149">Count of how many setting a policy holds</span></span>|



## <a name="response"></a><span data-ttu-id="2dfbd-150">応答</span><span class="sxs-lookup"><span data-stu-id="2dfbd-150">Response</span></span>
<span data-ttu-id="2dfbd-151">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-151">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_deviceconfigurationstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dfbd-152">例</span><span class="sxs-lookup"><span data-stu-id="2dfbd-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="2dfbd-153">要求</span><span class="sxs-lookup"><span data-stu-id="2dfbd-153">Request</span></span>
<span data-ttu-id="2dfbd-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceConfigurationStates
Content-type: application/json
Content-length: 967

{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "iOS",
  "state": "notApplicable",
  "settingCount": 12
}
```

### <a name="response"></a><span data-ttu-id="2dfbd-155">応答</span><span class="sxs-lookup"><span data-stu-id="2dfbd-155">Response</span></span>
<span data-ttu-id="2dfbd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2dfbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1016

{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "11692784-2784-1169-8427-691184276911",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "iOS",
  "state": "notApplicable",
  "settingCount": 12
}
```



