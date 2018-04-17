# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="e1552-101">iosMobileAppConfiguration のリスト</span><span class="sxs-lookup"><span data-stu-id="e1552-101">List iosMobileAppConfigurations</span></span>

> <span data-ttu-id="e1552-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1552-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1552-103">[iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) オブジェクトのプロパティとリレーションシップのリストを作成します。</span><span class="sxs-lookup"><span data-stu-id="e1552-103">List properties and relationships of the [managedMobileApp](../resources/intune_apps_iosmobileappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1552-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e1552-104">Prerequisites</span></span>
<span data-ttu-id="e1552-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1552-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1552-107">Permission type</span></span>|<span data-ttu-id="e1552-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1552-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1552-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1552-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e1552-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1552-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e1552-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1552-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1552-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1552-112">Not supported.</span></span>|
|<span data-ttu-id="e1552-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1552-113">Application</span></span>|<span data-ttu-id="e1552-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1552-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1552-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1552-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e1552-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1552-116">Request headers</span></span>
|<span data-ttu-id="e1552-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1552-117">Header</span></span>|<span data-ttu-id="e1552-118">値</span><span class="sxs-lookup"><span data-stu-id="e1552-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1552-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1552-119">Authorization</span></span>|<span data-ttu-id="e1552-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e1552-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1552-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e1552-121">Accept</span></span>|<span data-ttu-id="e1552-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e1552-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1552-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1552-123">Request body</span></span>
<span data-ttu-id="e1552-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e1552-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1552-125">応答</span><span class="sxs-lookup"><span data-stu-id="e1552-125">Response</span></span>
<span data-ttu-id="e1552-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e1552-126">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_apps_iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1552-127">例</span><span class="sxs-lookup"><span data-stu-id="e1552-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1552-128">要求</span><span class="sxs-lookup"><span data-stu-id="e1552-128">Request</span></span>
<span data-ttu-id="e1552-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1552-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="e1552-130">応答</span><span class="sxs-lookup"><span data-stu-id="e1552-130">Response</span></span>
<span data-ttu-id="e1552-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1552-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 815

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
      "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
      "settings": [
        {
          "@odata.type": "microsoft.graph.appConfigurationSettingItem",
          "appConfigKey": "App Config Key value",
          "appConfigKeyType": "integerType",
          "appConfigKeyValue": "App Config Key Value value"
        }
      ]
    }
  ]
}
```



