# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="b871e-101">androidGeneralDeviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="b871e-101">List androidGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="b871e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b871e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b871e-103">[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b871e-103">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b871e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b871e-104">Prerequisites</span></span>
<span data-ttu-id="b871e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b871e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b871e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b871e-107">Permission type</span></span>|<span data-ttu-id="b871e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b871e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b871e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b871e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b871e-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b871e-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b871e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b871e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b871e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b871e-112">Not supported.</span></span>|
|<span data-ttu-id="b871e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b871e-113">Application</span></span>|<span data-ttu-id="b871e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b871e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b871e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b871e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b871e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b871e-116">Request headers</span></span>
|<span data-ttu-id="b871e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b871e-117">Header</span></span>|<span data-ttu-id="b871e-118">値</span><span class="sxs-lookup"><span data-stu-id="b871e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b871e-119">承認</span><span class="sxs-lookup"><span data-stu-id="b871e-119">Authorization</span></span>|<span data-ttu-id="b871e-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b871e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b871e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b871e-121">Accept</span></span>|<span data-ttu-id="b871e-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="b871e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b871e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b871e-123">Request body</span></span>
<span data-ttu-id="b871e-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b871e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b871e-125">応答</span><span class="sxs-lookup"><span data-stu-id="b871e-125">Response</span></span>
<span data-ttu-id="b871e-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b871e-126">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b871e-127">例</span><span class="sxs-lookup"><span data-stu-id="b871e-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="b871e-128">要求</span><span class="sxs-lookup"><span data-stu-id="b871e-128">Request</span></span>
<span data-ttu-id="b871e-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b871e-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b871e-130">応答</span><span class="sxs-lookup"><span data-stu-id="b871e-130">Response</span></span>
<span data-ttu-id="b871e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b871e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3618

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
      "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "appsBlockClipboardSharing": true,
      "appsBlockCopyPaste": true,
      "appsBlockYouTube": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockDataRoaming": true,
      "cellularBlockMessaging": true,
      "cellularBlockVoiceRoaming": true,
      "cellularBlockWiFiTethering": true,
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
      "locationServicesBlocked": true,
      "googleAccountBlockAutoSync": true,
      "googlePlayStoreBlocked": true,
      "kioskModeBlockSleepButton": true,
      "kioskModeBlockVolumeButtons": true,
      "kioskModeApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "nfcBlocked": true,
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockTrustAgents": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphabetic",
      "passwordRequired": true,
      "powerOffBlocked": true,
      "factoryResetBlocked": true,
      "screenCaptureBlocked": true,
      "deviceSharingAllowed": true,
      "storageBlockGoogleBackup": true,
      "storageBlockRemovableStorage": true,
      "storageRequireDeviceEncryption": true,
      "storageRequireRemovableStorageEncryption": true,
      "voiceAssistantBlocked": true,
      "voiceDialingBlocked": true,
      "webBrowserBlockPopups": true,
      "webBrowserBlockAutofill": true,
      "webBrowserBlockJavaScript": true,
      "webBrowserBlocked": true,
      "webBrowserCookieSettings": "blockAlways",
      "wiFiBlocked": true,
      "appsInstallAllowList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsLaunchBlockList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsHideList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "securityRequireVerifyApps": true
    }
  ]
}
```








