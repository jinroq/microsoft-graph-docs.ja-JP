# <a name="get-iosvppapp"></a><span data-ttu-id="949e7-101">Get iosVppApp</span><span class="sxs-lookup"><span data-stu-id="949e7-101">Get iosVppApp</span></span>

> <span data-ttu-id="949e7-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="949e7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="949e7-103">[iosVppApp](../resources/intune_apps_iosvppapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="949e7-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="949e7-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="949e7-104">Prerequisites</span></span>
<span data-ttu-id="949e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="949e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="949e7-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="949e7-107">Permission type</span></span>|<span data-ttu-id="949e7-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="949e7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="949e7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="949e7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="949e7-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="949e7-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="949e7-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="949e7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="949e7-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="949e7-112">Not supported.</span></span>|
|<span data-ttu-id="949e7-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="949e7-113">Application</span></span>|<span data-ttu-id="949e7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="949e7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="949e7-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="949e7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="949e7-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="949e7-116">Optional query parameters</span></span>
<span data-ttu-id="949e7-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="949e7-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="949e7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="949e7-118">Request headers</span></span>
|<span data-ttu-id="949e7-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="949e7-119">Header</span></span>|<span data-ttu-id="949e7-120">値</span><span class="sxs-lookup"><span data-stu-id="949e7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="949e7-121">承認</span><span class="sxs-lookup"><span data-stu-id="949e7-121">Authorization</span></span>|<span data-ttu-id="949e7-122">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="949e7-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="949e7-123">承諾</span><span class="sxs-lookup"><span data-stu-id="949e7-123">Accept</span></span>|<span data-ttu-id="949e7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="949e7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="949e7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="949e7-125">Request body</span></span>
<span data-ttu-id="949e7-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="949e7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="949e7-127">応答</span><span class="sxs-lookup"><span data-stu-id="949e7-127">Response</span></span>
<span data-ttu-id="949e7-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosVppApp](../resources/intune_apps_iosvppapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="949e7-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="949e7-129">例</span><span class="sxs-lookup"><span data-stu-id="949e7-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="949e7-130">要求</span><span class="sxs-lookup"><span data-stu-id="949e7-130">Request</span></span>
<span data-ttu-id="949e7-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="949e7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="949e7-132">応答</span><span class="sxs-lookup"><span data-stu-id="949e7-132">Response</span></span>
<span data-ttu-id="949e7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="949e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppApp",
    "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "publishingState": "processing",
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    },
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "vppTokenOrganizationName": "Vpp Token Organization Name value",
    "vppTokenAccountType": "education",
    "vppTokenAppleId": "Vpp Token Apple Id value",
    "bundleId": "Bundle Id value"
  }
}
```



