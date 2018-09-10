# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="8c1d3-101">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="8c1d3-101">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="8c1d3-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c1d3-103">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-103">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c1d3-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="8c1d3-104">Prerequisites</span></span>
<span data-ttu-id="8c1d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c1d3-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c1d3-107">Permission type</span></span>|<span data-ttu-id="8c1d3-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c1d3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c1d3-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c1d3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8c1d3-110">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c1d3-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8c1d3-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c1d3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c1d3-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-112">Not supported.</span></span>|
|<span data-ttu-id="8c1d3-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c1d3-113">Application</span></span>|<span data-ttu-id="8c1d3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c1d3-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c1d3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c1d3-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c1d3-116">Optional query parameters</span></span>
<span data-ttu-id="8c1d3-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8c1d3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c1d3-118">Request headers</span></span>
|<span data-ttu-id="8c1d3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c1d3-119">Header</span></span>|<span data-ttu-id="8c1d3-120">値</span><span class="sxs-lookup"><span data-stu-id="8c1d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c1d3-121">承認</span><span class="sxs-lookup"><span data-stu-id="8c1d3-121">Authorization</span></span>|<span data-ttu-id="8c1d3-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c1d3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8c1d3-123">Accept</span></span>|<span data-ttu-id="8c1d3-124">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="8c1d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c1d3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c1d3-125">Request body</span></span>
<span data-ttu-id="8c1d3-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c1d3-127">応答</span><span class="sxs-lookup"><span data-stu-id="8c1d3-127">Response</span></span>
<span data-ttu-id="8c1d3-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-128">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c1d3-129">例</span><span class="sxs-lookup"><span data-stu-id="8c1d3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c1d3-130">要求</span><span class="sxs-lookup"><span data-stu-id="8c1d3-130">Request</span></span>
<span data-ttu-id="8c1d3-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="8c1d3-132">応答</span><span class="sxs-lookup"><span data-stu-id="8c1d3-132">Response</span></span>
<span data-ttu-id="8c1d3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c1d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
    "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
    "userDisplayName": "User Display Name value",
    "acceptedVersion": 15,
    "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
  }
}
```








