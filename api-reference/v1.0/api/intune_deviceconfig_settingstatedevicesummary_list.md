# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="2aeba-101">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="2aeba-101">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="2aeba-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2aeba-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2aeba-103">[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2aeba-103">List properties and relationships of the [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2aeba-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2aeba-104">Prerequisites</span></span>
<span data-ttu-id="2aeba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2aeba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2aeba-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2aeba-107">Permission type</span></span>|<span data-ttu-id="2aeba-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2aeba-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2aeba-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2aeba-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2aeba-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2aeba-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2aeba-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2aeba-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2aeba-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2aeba-112">Not supported.</span></span>|
|<span data-ttu-id="2aeba-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2aeba-113">Application</span></span>|<span data-ttu-id="2aeba-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2aeba-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2aeba-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2aeba-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="2aeba-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2aeba-116">Request headers</span></span>
|<span data-ttu-id="2aeba-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2aeba-117">Header</span></span>|<span data-ttu-id="2aeba-118">値</span><span class="sxs-lookup"><span data-stu-id="2aeba-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2aeba-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2aeba-119">Authorization</span></span>|<span data-ttu-id="2aeba-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2aeba-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2aeba-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2aeba-121">Accept</span></span>|<span data-ttu-id="2aeba-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2aeba-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2aeba-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2aeba-123">Request body</span></span>
<span data-ttu-id="2aeba-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2aeba-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2aeba-125">応答</span><span class="sxs-lookup"><span data-stu-id="2aeba-125">Response</span></span>
<span data-ttu-id="2aeba-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2aeba-126">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_deviceconfig_settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2aeba-127">例</span><span class="sxs-lookup"><span data-stu-id="2aeba-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="2aeba-128">要求</span><span class="sxs-lookup"><span data-stu-id="2aeba-128">Request</span></span>
<span data-ttu-id="2aeba-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2aeba-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="2aeba-130">応答</span><span class="sxs-lookup"><span data-stu-id="2aeba-130">Response</span></span>
<span data-ttu-id="2aeba-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2aeba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```



