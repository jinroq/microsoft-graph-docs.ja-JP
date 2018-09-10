# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="7f0fb-101">windowsPhone81GeneralConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="7f0fb-101">List windowsPhone81GeneralConfigurations</span></span>

> <span data-ttu-id="7f0fb-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7f0fb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f0fb-103">[windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7f0fb-103">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f0fb-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f0fb-104">Prerequisites</span></span>
<span data-ttu-id="7f0fb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f0fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7f0fb-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f0fb-107">Permission type</span></span>|<span data-ttu-id="7f0fb-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f0fb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f0fb-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f0fb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7f0fb-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f0fb-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7f0fb-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f0fb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f0fb-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f0fb-112">Not supported.</span></span>|
|<span data-ttu-id="7f0fb-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f0fb-113">Application</span></span>|<span data-ttu-id="7f0fb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f0fb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f0fb-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f0fb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7f0fb-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f0fb-116">Request headers</span></span>
|<span data-ttu-id="7f0fb-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f0fb-117">Header</span></span>|<span data-ttu-id="7f0fb-118">値</span><span class="sxs-lookup"><span data-stu-id="7f0fb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f0fb-119">承認</span><span class="sxs-lookup"><span data-stu-id="7f0fb-119">Authorization</span></span>|<span data-ttu-id="7f0fb-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7f0fb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f0fb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7f0fb-121">Accept</span></span>|<span data-ttu-id="7f0fb-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="7f0fb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f0fb-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f0fb-123">Request body</span></span>
<span data-ttu-id="7f0fb-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f0fb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f0fb-125">応答</span><span class="sxs-lookup"><span data-stu-id="7f0fb-125">Response</span></span>
<span data-ttu-id="7f0fb-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7f0fb-126">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f0fb-127">例</span><span class="sxs-lookup"><span data-stu-id="7f0fb-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f0fb-128">要求</span><span class="sxs-lookup"><span data-stu-id="7f0fb-128">Request</span></span>
<span data-ttu-id="7f0fb-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f0fb-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="7f0fb-130">応答</span><span class="sxs-lookup"><span data-stu-id="7f0fb-130">Response</span></span>
<span data-ttu-id="7f0fb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f0fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1842

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
      "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "applyOnlyToWindowsPhone81": true,
      "appsBlockCopyPaste": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockWifiTethering": true,
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "diagnosticDataBlockSubmission": true,
      "emailBlockAddingAccounts": true,
      "locationServicesBlocked": true,
      "microsoftAccountBlocked": true,
      "nfcBlocked": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true,
      "screenCaptureBlocked": true,
      "storageBlockRemovableStorage": true,
      "storageRequireEncryption": true,
      "webBrowserBlocked": true,
      "wifiBlocked": true,
      "wifiBlockAutomaticConnectHotspots": true,
      "wifiBlockHotspotReporting": true,
      "windowsStoreBlocked": true
    }
  ]
}
```








