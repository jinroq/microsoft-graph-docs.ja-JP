# <a name="list-devicecompliancepolicystates"></a><span data-ttu-id="51f42-101">deviceCompliancePolicyStates のリスト</span><span class="sxs-lookup"><span data-stu-id="51f42-101">List deviceCompliancePolicyStates</span></span>

> <span data-ttu-id="51f42-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="51f42-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51f42-103">[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="51f42-103">List properties and relationships of the [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51f42-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="51f42-104">Prerequisites</span></span>
<span data-ttu-id="51f42-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51f42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51f42-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51f42-107">Permission type</span></span>|<span data-ttu-id="51f42-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="51f42-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51f42-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51f42-109">Delegated (work or school account)</span></span>|<span data-ttu-id="51f42-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51f42-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="51f42-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51f42-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51f42-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51f42-112">Not supported.</span></span>|
|<span data-ttu-id="51f42-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51f42-113">Application</span></span>|<span data-ttu-id="51f42-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51f42-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51f42-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51f42-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
```

## <a name="request-headers"></a><span data-ttu-id="51f42-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51f42-116">Request headers</span></span>
|<span data-ttu-id="51f42-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51f42-117">Header</span></span>|<span data-ttu-id="51f42-118">値</span><span class="sxs-lookup"><span data-stu-id="51f42-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51f42-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="51f42-119">Authorization</span></span>|<span data-ttu-id="51f42-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="51f42-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="51f42-121">Accept</span><span class="sxs-lookup"><span data-stu-id="51f42-121">Accept</span></span>|<span data-ttu-id="51f42-122">application/json</span><span class="sxs-lookup"><span data-stu-id="51f42-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51f42-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="51f42-123">Request body</span></span>
<span data-ttu-id="51f42-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="51f42-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51f42-125">応答</span><span class="sxs-lookup"><span data-stu-id="51f42-125">Response</span></span>
<span data-ttu-id="51f42-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="51f42-126">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_deviceconfig_devicecompliancepolicystate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51f42-127">例</span><span class="sxs-lookup"><span data-stu-id="51f42-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="51f42-128">要求</span><span class="sxs-lookup"><span data-stu-id="51f42-128">Request</span></span>
<span data-ttu-id="51f42-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51f42-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
```

### <a name="response"></a><span data-ttu-id="51f42-130">応答</span><span class="sxs-lookup"><span data-stu-id="51f42-130">Response</span></span>
<span data-ttu-id="51f42-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51f42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1175

{
  "value": [
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
  ]
}
```



