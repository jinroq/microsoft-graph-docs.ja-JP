# <a name="get-deviceappmanagement"></a><span data-ttu-id="8ccbe-101">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="8ccbe-101">Get deviceAppManagement</span></span>

> <span data-ttu-id="8ccbe-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ccbe-103">[deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-103">Read properties and relationships of the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ccbe-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="8ccbe-104">Prerequisites</span></span>

<span data-ttu-id="8ccbe-105">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8ccbe-106">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="8ccbe-107">ワークフローに従って、適切なアクセス許可が異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="8ccbe-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ccbe-108">Permission type</span></span>|<span data-ttu-id="8ccbe-109">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ccbe-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ccbe-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ccbe-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8ccbe-111">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ccbe-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="8ccbe-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ccbe-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ccbe-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-113">Not supported.</span></span>|
|<span data-ttu-id="8ccbe-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ccbe-114">Application</span></span>|<span data-ttu-id="8ccbe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ccbe-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ccbe-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ccbe-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ccbe-117">Optional query parameters</span></span>
<span data-ttu-id="8ccbe-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ccbe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ccbe-119">Request headers</span></span>
|<span data-ttu-id="8ccbe-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ccbe-120">Header</span></span>|<span data-ttu-id="8ccbe-121">値</span><span class="sxs-lookup"><span data-stu-id="8ccbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ccbe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ccbe-122">Authorization</span></span>|<span data-ttu-id="8ccbe-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ccbe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8ccbe-124">Accept</span></span>|<span data-ttu-id="8ccbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ccbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ccbe-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ccbe-126">Request body</span></span>
<span data-ttu-id="8ccbe-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ccbe-128">応答</span><span class="sxs-lookup"><span data-stu-id="8ccbe-128">Response</span></span>
<span data-ttu-id="8ccbe-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-129">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="8ccbe-130">要求の例</span><span class="sxs-lookup"><span data-stu-id="8ccbe-130">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="8ccbe-131">応答の例</span><span class="sxs-lookup"><span data-stu-id="8ccbe-131">Example response</span></span>
<span data-ttu-id="8ccbe-132">ここに示す応答オブジェクトは、簡潔にするために切り詰められます。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8ccbe-133">すべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8ccbe-133">All properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



