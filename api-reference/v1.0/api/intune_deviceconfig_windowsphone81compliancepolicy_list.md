# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="685ef-101">windowsPhone81CompliancePolicies のリスト</span><span class="sxs-lookup"><span data-stu-id="685ef-101">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="685ef-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="685ef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="685ef-103">[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="685ef-103">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="685ef-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="685ef-104">Prerequisites</span></span>
<span data-ttu-id="685ef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="685ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="685ef-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="685ef-107">Permission type</span></span>|<span data-ttu-id="685ef-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="685ef-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="685ef-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="685ef-109">Delegated (work or school account)</span></span>|<span data-ttu-id="685ef-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="685ef-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="685ef-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="685ef-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="685ef-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="685ef-112">Not supported.</span></span>|
|<span data-ttu-id="685ef-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="685ef-113">Application</span></span>|<span data-ttu-id="685ef-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="685ef-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="685ef-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="685ef-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="685ef-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="685ef-116">Request headers</span></span>
|<span data-ttu-id="685ef-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="685ef-117">Header</span></span>|<span data-ttu-id="685ef-118">値</span><span class="sxs-lookup"><span data-stu-id="685ef-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="685ef-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="685ef-119">Authorization</span></span>|<span data-ttu-id="685ef-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="685ef-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="685ef-121">Accept</span><span class="sxs-lookup"><span data-stu-id="685ef-121">Accept</span></span>|<span data-ttu-id="685ef-122">application/json</span><span class="sxs-lookup"><span data-stu-id="685ef-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="685ef-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="685ef-123">Request body</span></span>
<span data-ttu-id="685ef-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="685ef-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="685ef-125">応答</span><span class="sxs-lookup"><span data-stu-id="685ef-125">Response</span></span>
<span data-ttu-id="685ef-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="685ef-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="685ef-127">例</span><span class="sxs-lookup"><span data-stu-id="685ef-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="685ef-128">要求</span><span class="sxs-lookup"><span data-stu-id="685ef-128">Request</span></span>
<span data-ttu-id="685ef-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="685ef-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="685ef-130">応答</span><span class="sxs-lookup"><span data-stu-id="685ef-130">Response</span></span>
<span data-ttu-id="685ef-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="685ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
      "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```



