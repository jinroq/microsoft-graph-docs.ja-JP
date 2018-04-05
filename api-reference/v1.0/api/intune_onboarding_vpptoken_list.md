# <a name="list-vpptokens"></a><span data-ttu-id="15c03-101">List vppTokens</span><span class="sxs-lookup"><span data-stu-id="15c03-101">List vppTokens</span></span>

> <span data-ttu-id="15c03-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15c03-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15c03-103">[vppToken](../resources/intune_onboarding_vpptoken.md) オブジェクトのプロパティとリレーションシップを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="15c03-103">List properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune_onboarding_vpptoken.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15c03-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="15c03-104">Prerequisites</span></span>
<span data-ttu-id="15c03-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15c03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="15c03-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15c03-107">Permission type</span></span>|<span data-ttu-id="15c03-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="15c03-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15c03-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15c03-109">Delegated (work or school account)</span></span>|<span data-ttu-id="15c03-110">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="15c03-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="15c03-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15c03-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15c03-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15c03-112">Not supported.</span></span>|
|<span data-ttu-id="15c03-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15c03-113">Application</span></span>|<span data-ttu-id="15c03-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15c03-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15c03-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15c03-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="15c03-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15c03-116">Request headers</span></span>
|<span data-ttu-id="15c03-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15c03-117">Header</span></span>|<span data-ttu-id="15c03-118">値</span><span class="sxs-lookup"><span data-stu-id="15c03-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15c03-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="15c03-119">Authorization</span></span>|<span data-ttu-id="15c03-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="15c03-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15c03-121">Accept</span><span class="sxs-lookup"><span data-stu-id="15c03-121">Accept</span></span>|<span data-ttu-id="15c03-122">application/json</span><span class="sxs-lookup"><span data-stu-id="15c03-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15c03-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="15c03-123">Request body</span></span>
<span data-ttu-id="15c03-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="15c03-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15c03-125">応答</span><span class="sxs-lookup"><span data-stu-id="15c03-125">Response</span></span>
<span data-ttu-id="15c03-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [vppToken](../resources/intune_onboarding_vpptoken.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="15c03-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/intune_onboarding_vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15c03-127">例</span><span class="sxs-lookup"><span data-stu-id="15c03-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="15c03-128">要求</span><span class="sxs-lookup"><span data-stu-id="15c03-128">Request</span></span>
<span data-ttu-id="15c03-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="15c03-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="15c03-130">応答</span><span class="sxs-lookup"><span data-stu-id="15c03-130">Response</span></span>
<span data-ttu-id="15c03-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="15c03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vppToken",
      "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
      "organizationName": "Organization Name value",
      "vppTokenAccountType": "education",
      "appleId": "Apple Id value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "token": "Token value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "valid",
      "lastSyncStatus": "inProgress",
      "automaticallyUpdateApps": true,
      "countryOrRegion": "Country Or Region value"
    }
  ]
}
```



