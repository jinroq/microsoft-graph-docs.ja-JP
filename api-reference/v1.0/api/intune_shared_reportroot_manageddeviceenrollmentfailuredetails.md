# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="659f6-101">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="659f6-101">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="659f6-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="659f6-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="659f6-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="659f6-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="659f6-104">Prerequisites</span></span>
<span data-ttu-id="659f6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="659f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="659f6-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="659f6-107">Permission type</span></span>|<span data-ttu-id="659f6-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="659f6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="659f6-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="659f6-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="659f6-110">&nbsp; &nbsp; トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="659f6-110">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="659f6-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="659f6-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="659f6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="659f6-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="659f6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="659f6-113">Not supported.</span></span>|
|<span data-ttu-id="659f6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="659f6-114">Application</span></span>|<span data-ttu-id="659f6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="659f6-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="659f6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="659f6-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="659f6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="659f6-117">Request headers</span></span>
|<span data-ttu-id="659f6-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="659f6-118">Header</span></span>|<span data-ttu-id="659f6-119">値</span><span class="sxs-lookup"><span data-stu-id="659f6-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="659f6-120">承認</span><span class="sxs-lookup"><span data-stu-id="659f6-120">Authorization</span></span>|<span data-ttu-id="659f6-121">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="659f6-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="659f6-122">承諾する</span><span class="sxs-lookup"><span data-stu-id="659f6-122">Accept</span></span>|<span data-ttu-id="659f6-123">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="659f6-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="659f6-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="659f6-124">Request body</span></span>
<span data-ttu-id="659f6-125">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="659f6-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="659f6-126">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="659f6-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="659f6-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="659f6-127">Property</span></span>|<span data-ttu-id="659f6-128">型</span><span class="sxs-lookup"><span data-stu-id="659f6-128">Type</span></span>|<span data-ttu-id="659f6-129">説明</span><span class="sxs-lookup"><span data-stu-id="659f6-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="659f6-130">スキップ</span><span class="sxs-lookup"><span data-stu-id="659f6-130">skip</span></span>|<span data-ttu-id="659f6-131">Int32</span><span class="sxs-lookup"><span data-stu-id="659f6-131">Int32</span></span>|<span data-ttu-id="659f6-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="659f6-132">Not yet documented</span></span>|
|<span data-ttu-id="659f6-133">top</span><span class="sxs-lookup"><span data-stu-id="659f6-133">top</span></span>|<span data-ttu-id="659f6-134">Int32</span><span class="sxs-lookup"><span data-stu-id="659f6-134">Int32</span></span>|<span data-ttu-id="659f6-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="659f6-135">Not yet documented</span></span>|
|<span data-ttu-id="659f6-136">filter</span><span class="sxs-lookup"><span data-stu-id="659f6-136">filter</span></span>|<span data-ttu-id="659f6-137">文字列</span><span class="sxs-lookup"><span data-stu-id="659f6-137">String</span></span>|<span data-ttu-id="659f6-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="659f6-138">Not yet documented</span></span>|
|<span data-ttu-id="659f6-139">skipToken</span><span class="sxs-lookup"><span data-stu-id="659f6-139">skipToken</span></span>|<span data-ttu-id="659f6-140">文字列</span><span class="sxs-lookup"><span data-stu-id="659f6-140">String</span></span>|<span data-ttu-id="659f6-141">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="659f6-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="659f6-142">応答</span><span class="sxs-lookup"><span data-stu-id="659f6-142">Response</span></span>
<span data-ttu-id="659f6-143">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune_shared_report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="659f6-143">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="659f6-144">例</span><span class="sxs-lookup"><span data-stu-id="659f6-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="659f6-145">要求</span><span class="sxs-lookup"><span data-stu-id="659f6-145">Request</span></span>
<span data-ttu-id="659f6-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="659f6-146">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="659f6-147">応答</span><span class="sxs-lookup"><span data-stu-id="659f6-147">Response</span></span>
<span data-ttu-id="659f6-148">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="659f6-148">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="659f6-149">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="659f6-149">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```




