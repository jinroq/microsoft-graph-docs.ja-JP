# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="ad2f4-101">androidManagedAppProtections のリスト</span><span class="sxs-lookup"><span data-stu-id="ad2f4-101">List androidManagedAppProtections</span></span>

> <span data-ttu-id="ad2f4-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad2f4-103">[androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-103">List properties and relationships of the [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad2f4-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ad2f4-104">Prerequisites</span></span>
<span data-ttu-id="ad2f4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad2f4-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad2f4-107">Permission type</span></span>|<span data-ttu-id="ad2f4-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad2f4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad2f4-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad2f4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ad2f4-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad2f4-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ad2f4-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad2f4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad2f4-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-112">Not supported.</span></span>|
|<span data-ttu-id="ad2f4-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad2f4-113">Application</span></span>|<span data-ttu-id="ad2f4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad2f4-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad2f4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="ad2f4-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad2f4-116">Request headers</span></span>
|<span data-ttu-id="ad2f4-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad2f4-117">Header</span></span>|<span data-ttu-id="ad2f4-118">値</span><span class="sxs-lookup"><span data-stu-id="ad2f4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad2f4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad2f4-119">Authorization</span></span>|<span data-ttu-id="ad2f4-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ad2f4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ad2f4-121">Accept</span></span>|<span data-ttu-id="ad2f4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ad2f4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad2f4-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad2f4-123">Request body</span></span>
<span data-ttu-id="ad2f4-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad2f4-125">応答</span><span class="sxs-lookup"><span data-stu-id="ad2f4-125">Response</span></span>
<span data-ttu-id="ad2f4-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_mam_androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad2f4-127">例</span><span class="sxs-lookup"><span data-stu-id="ad2f4-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad2f4-128">要求</span><span class="sxs-lookup"><span data-stu-id="ad2f4-128">Request</span></span>
<span data-ttu-id="ad2f4-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="ad2f4-130">応答</span><span class="sxs-lookup"><span data-stu-id="ad2f4-130">Response</span></span>
<span data-ttu-id="ad2f4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2065

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
      "version": "Version value",
      "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
      "periodOnlineBeforeAccessCheck": "PT35.0018757S",
      "allowedInboundDataTransferSources": "managedApps",
      "allowedOutboundDataTransferDestinations": "managedApps",
      "organizationalCredentialsRequired": true,
      "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
      "dataBackupBlocked": true,
      "deviceComplianceRequired": true,
      "managedBrowserToOpenLinksRequired": true,
      "saveAsBlocked": true,
      "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
      "pinRequired": true,
      "maximumPinRetries": 1,
      "simplePinBlocked": true,
      "minimumPinLength": 0,
      "pinCharacterSet": "alphanumericAndSymbol",
      "periodBeforePinReset": "PT3M29.6631862S",
      "allowedDataStorageLocations": [
        "sharePoint"
      ],
      "contactSyncBlocked": true,
      "printBlocked": true,
      "fingerprintBlocked": true,
      "disableAppPinIfDevicePinIsSet": true,
      "minimumRequiredOsVersion": "Minimum Required Os Version value",
      "minimumWarningOsVersion": "Minimum Warning Os Version value",
      "minimumRequiredAppVersion": "Minimum Required App Version value",
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "isAssigned": true,
      "screenCaptureBlocked": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "encryptAppData": true,
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
    }
  ]
}
```



