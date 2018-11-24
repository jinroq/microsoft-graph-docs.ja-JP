# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="c82ce-101">ManagedDeviceMobileAppConfigurationDeviceStatus を取得します。</span><span class="sxs-lookup"><span data-stu-id="c82ce-101">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="c82ce-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c82ce-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c82ce-103">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c82ce-103">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c82ce-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="c82ce-104">Prerequisites</span></span>
<span data-ttu-id="c82ce-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c82ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c82ce-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c82ce-107">Permission type</span></span>|<span data-ttu-id="c82ce-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c82ce-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c82ce-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c82ce-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c82ce-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82ce-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c82ce-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c82ce-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c82ce-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c82ce-112">Not supported.</span></span>|
|<span data-ttu-id="c82ce-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c82ce-113">Application</span></span>|<span data-ttu-id="c82ce-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c82ce-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c82ce-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c82ce-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c82ce-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c82ce-116">Optional query parameters</span></span>
<span data-ttu-id="c82ce-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c82ce-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c82ce-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c82ce-118">Request headers</span></span>
|<span data-ttu-id="c82ce-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c82ce-119">Header</span></span>|<span data-ttu-id="c82ce-120">値</span><span class="sxs-lookup"><span data-stu-id="c82ce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c82ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c82ce-121">Authorization</span></span>|<span data-ttu-id="c82ce-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c82ce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c82ce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c82ce-123">Accept</span></span>|<span data-ttu-id="c82ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c82ce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c82ce-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c82ce-125">Request body</span></span>
<span data-ttu-id="c82ce-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c82ce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c82ce-127">応答</span><span class="sxs-lookup"><span data-stu-id="c82ce-127">Response</span></span>
<span data-ttu-id="c82ce-128">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c82ce-128">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c82ce-129">例</span><span class="sxs-lookup"><span data-stu-id="c82ce-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c82ce-130">要求</span><span class="sxs-lookup"><span data-stu-id="c82ce-130">Request</span></span>
<span data-ttu-id="c82ce-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c82ce-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="c82ce-132">応答</span><span class="sxs-lookup"><span data-stu-id="c82ce-132">Response</span></span>
<span data-ttu-id="c82ce-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c82ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
    "id": "477d3651-3651-477d-5136-7d4751367d47",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



