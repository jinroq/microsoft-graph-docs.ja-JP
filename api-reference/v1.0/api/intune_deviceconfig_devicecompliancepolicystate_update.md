# <a name="update-devicecompliancepolicystate"></a><span data-ttu-id="591ec-101">deviceCompliancePolicyState の更新</span><span class="sxs-lookup"><span data-stu-id="591ec-101">Update deviceCompliancePolicyState</span></span>

> <span data-ttu-id="591ec-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="591ec-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="591ec-103">[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="591ec-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="591ec-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="591ec-104">Prerequisites</span></span>
<span data-ttu-id="591ec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="591ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="591ec-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="591ec-107">Permission type</span></span>|<span data-ttu-id="591ec-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="591ec-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="591ec-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="591ec-109">Delegated (work or school account)</span></span>|<span data-ttu-id="591ec-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="591ec-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="591ec-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="591ec-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="591ec-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="591ec-112">Not supported.</span></span>|
|<span data-ttu-id="591ec-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="591ec-113">Application</span></span>|<span data-ttu-id="591ec-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="591ec-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="591ec-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="591ec-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /managedDevices/{managedDevicesId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
```

## <a name="request-headers"></a><span data-ttu-id="591ec-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="591ec-116">Request headers</span></span>
|<span data-ttu-id="591ec-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="591ec-117">Header</span></span>|<span data-ttu-id="591ec-118">値</span><span class="sxs-lookup"><span data-stu-id="591ec-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="591ec-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="591ec-119">Authorization</span></span>|<span data-ttu-id="591ec-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="591ec-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="591ec-121">Accept</span><span class="sxs-lookup"><span data-stu-id="591ec-121">Accept</span></span>|<span data-ttu-id="591ec-122">application/json</span><span class="sxs-lookup"><span data-stu-id="591ec-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="591ec-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="591ec-123">Request body</span></span>
<span data-ttu-id="591ec-124">要求本文で、[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="591ec-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object.</span></span>

<span data-ttu-id="591ec-125">次の表に、[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="591ec-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="591ec-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="591ec-126">Property</span></span>|<span data-ttu-id="591ec-127">型</span><span class="sxs-lookup"><span data-stu-id="591ec-127">Type</span></span>|<span data-ttu-id="591ec-128">説明</span><span class="sxs-lookup"><span data-stu-id="591ec-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="591ec-129">id</span><span class="sxs-lookup"><span data-stu-id="591ec-129">id</span></span>|<span data-ttu-id="591ec-130">String</span><span class="sxs-lookup"><span data-stu-id="591ec-130">String</span></span>|<span data-ttu-id="591ec-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="591ec-131">Name of the entity.</span></span>|
|<span data-ttu-id="591ec-132">settingStates</span><span class="sxs-lookup"><span data-stu-id="591ec-132">settingStates</span></span>|<span data-ttu-id="591ec-133">[deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="591ec-133">[deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md) collection</span></span>|<span data-ttu-id="591ec-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="591ec-134">Not yet documented</span></span>|
|<span data-ttu-id="591ec-135">displayName</span><span class="sxs-lookup"><span data-stu-id="591ec-135">displayName</span></span>|<span data-ttu-id="591ec-136">String</span><span class="sxs-lookup"><span data-stu-id="591ec-136">String</span></span>|<span data-ttu-id="591ec-137">この policyBase のポリシーの名前</span><span class="sxs-lookup"><span data-stu-id="591ec-137">The friendly name of the DLP policy for this event.</span></span>|
|<span data-ttu-id="591ec-138">version</span><span class="sxs-lookup"><span data-stu-id="591ec-138">version</span></span>|<span data-ttu-id="591ec-139">Int32</span><span class="sxs-lookup"><span data-stu-id="591ec-139">Int32</span></span>|<span data-ttu-id="591ec-140">ポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="591ec-140">The version of the policy</span></span>|
|<span data-ttu-id="591ec-141">platformType</span><span class="sxs-lookup"><span data-stu-id="591ec-141">PlatformType</span></span>|<span data-ttu-id="591ec-142">String</span><span class="sxs-lookup"><span data-stu-id="591ec-142">String</span></span>|<span data-ttu-id="591ec-143">ポリシーが適用されるプラットフォームの種類。可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="591ec-143">Platform type that the policy applies to Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="591ec-144">state</span><span class="sxs-lookup"><span data-stu-id="591ec-144">state</span></span>|<span data-ttu-id="591ec-145">String</span><span class="sxs-lookup"><span data-stu-id="591ec-145">String</span></span>|<span data-ttu-id="591ec-146">ポリシーのコンプライアンス対応状態。可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="591ec-146">The compliance state of the policy Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="591ec-147">settingCount</span><span class="sxs-lookup"><span data-stu-id="591ec-147">settingCount</span></span>|<span data-ttu-id="591ec-148">Int32</span><span class="sxs-lookup"><span data-stu-id="591ec-148">Int32</span></span>|<span data-ttu-id="591ec-149">ポリシーが保持する設定の数</span><span class="sxs-lookup"><span data-stu-id="591ec-149">Count of how many setting a policy holds</span></span>|



## <a name="response"></a><span data-ttu-id="591ec-150">応答</span><span class="sxs-lookup"><span data-stu-id="591ec-150">Response</span></span>
<span data-ttu-id="591ec-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="591ec-151">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="591ec-152">例</span><span class="sxs-lookup"><span data-stu-id="591ec-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="591ec-153">要求</span><span class="sxs-lookup"><span data-stu-id="591ec-153">Request</span></span>
<span data-ttu-id="591ec-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="591ec-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
Content-type: application/json
Content-length: 907

{
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
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

### <a name="response"></a><span data-ttu-id="591ec-155">応答</span><span class="sxs-lookup"><span data-stu-id="591ec-155">Response</span></span>
<span data-ttu-id="591ec-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="591ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1022

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "id": "2999e387-e387-2999-87e3-992987e39929",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
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



