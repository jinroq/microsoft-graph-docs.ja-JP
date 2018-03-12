# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="ce980-101">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="ce980-101">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="ce980-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce980-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce980-103">[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ce980-103">List properties and relationships of the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce980-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ce980-104">Prerequisites</span></span>
<span data-ttu-id="ce980-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce980-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce980-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce980-107">Permission type</span></span>|<span data-ttu-id="ce980-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce980-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce980-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce980-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ce980-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce980-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ce980-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce980-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce980-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce980-112">Not supported.</span></span>|
|<span data-ttu-id="ce980-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce980-113">Application</span></span>|<span data-ttu-id="ce980-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce980-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce980-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce980-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="ce980-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce980-116">Request headers</span></span>
|<span data-ttu-id="ce980-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce980-117">Header</span></span>|<span data-ttu-id="ce980-118">値</span><span class="sxs-lookup"><span data-stu-id="ce980-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce980-119">承認</span><span class="sxs-lookup"><span data-stu-id="ce980-119">Authorization</span></span>|<span data-ttu-id="ce980-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="ce980-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce980-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ce980-121">Accept</span></span>|<span data-ttu-id="ce980-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ce980-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce980-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce980-123">Request body</span></span>
<span data-ttu-id="ce980-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce980-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce980-125">応答</span><span class="sxs-lookup"><span data-stu-id="ce980-125">Response</span></span>
<span data-ttu-id="ce980-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ce980-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/intune_deviceconfig_devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce980-127">例</span><span class="sxs-lookup"><span data-stu-id="ce980-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce980-128">要求</span><span class="sxs-lookup"><span data-stu-id="ce980-128">Request</span></span>
<span data-ttu-id="ce980-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce980-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="ce980-130">応答</span><span class="sxs-lookup"><span data-stu-id="ce980-130">Response</span></span>
<span data-ttu-id="ce980-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce980-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "deviceModel": "Device Model value",
      "state": "notApplicable",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
    }
  ]
}
```



