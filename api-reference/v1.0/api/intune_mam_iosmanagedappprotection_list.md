# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="ee443-101">iosManagedAppProtections のリスト</span><span class="sxs-lookup"><span data-stu-id="ee443-101">List iosManagedAppProtections</span></span>

> <span data-ttu-id="ee443-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee443-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee443-103">[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ee443-103">List properties and relationships of the [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee443-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee443-104">Prerequisites</span></span>
<span data-ttu-id="ee443-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ee443-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee443-107">Permission type</span></span>|<span data-ttu-id="ee443-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee443-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee443-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee443-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ee443-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee443-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ee443-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee443-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee443-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee443-112">Not supported.</span></span>|
|<span data-ttu-id="ee443-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee443-113">Application</span></span>|<span data-ttu-id="ee443-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee443-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee443-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee443-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="ee443-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee443-116">Request headers</span></span>
|<span data-ttu-id="ee443-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee443-117">Header</span></span>|<span data-ttu-id="ee443-118">値</span><span class="sxs-lookup"><span data-stu-id="ee443-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee443-119">承認</span><span class="sxs-lookup"><span data-stu-id="ee443-119">Authorization</span></span>|<span data-ttu-id="ee443-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ee443-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee443-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ee443-121">Accept</span></span>|<span data-ttu-id="ee443-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="ee443-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee443-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee443-123">Request body</span></span>
<span data-ttu-id="ee443-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ee443-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee443-125">応答</span><span class="sxs-lookup"><span data-stu-id="ee443-125">Response</span></span>
<span data-ttu-id="ee443-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ee443-126">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee443-127">例</span><span class="sxs-lookup"><span data-stu-id="ee443-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee443-128">要求</span><span class="sxs-lookup"><span data-stu-id="ee443-128">Request</span></span>
<span data-ttu-id="ee443-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee443-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="ee443-130">応答</span><span class="sxs-lookup"><span data-stu-id="ee443-130">Response</span></span>
<span data-ttu-id="ee443-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee443-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1933

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
      "appDataEncryptionType": "afterDeviceRestart",
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "deployedAppCount": 0,
      "faceIdBlocked": true
    }
  ]
}
```








