# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="f342c-101">deviceConfigurationDeviceActivity 関数</span><span class="sxs-lookup"><span data-stu-id="f342c-101">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="f342c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f342c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f342c-103">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="f342c-103">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f342c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="f342c-104">Prerequisites</span></span>
<span data-ttu-id="f342c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f342c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f342c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f342c-107">Permission type</span></span>|<span data-ttu-id="f342c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f342c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f342c-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f342c-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f342c-110">&nbsp; &nbsp; デバイス構成</span><span class="sxs-lookup"><span data-stu-id="f342c-110">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="f342c-111">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f342c-111">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f342c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f342c-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f342c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f342c-113">Not supported.</span></span>|
|<span data-ttu-id="f342c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f342c-114">Application</span></span>|<span data-ttu-id="f342c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f342c-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f342c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f342c-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="f342c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f342c-117">Request headers</span></span>
|<span data-ttu-id="f342c-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f342c-118">Header</span></span>|<span data-ttu-id="f342c-119">値</span><span class="sxs-lookup"><span data-stu-id="f342c-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f342c-120">承認</span><span class="sxs-lookup"><span data-stu-id="f342c-120">Authorization</span></span>|<span data-ttu-id="f342c-121">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f342c-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f342c-122">承諾する</span><span class="sxs-lookup"><span data-stu-id="f342c-122">Accept</span></span>|<span data-ttu-id="f342c-123">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="f342c-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f342c-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="f342c-124">Request body</span></span>
<span data-ttu-id="f342c-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f342c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f342c-126">応答</span><span class="sxs-lookup"><span data-stu-id="f342c-126">Response</span></span>
<span data-ttu-id="f342c-127">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune_shared_report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="f342c-127">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f342c-128">例</span><span class="sxs-lookup"><span data-stu-id="f342c-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="f342c-129">要求</span><span class="sxs-lookup"><span data-stu-id="f342c-129">Request</span></span>
<span data-ttu-id="f342c-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f342c-130">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="f342c-131">応答</span><span class="sxs-lookup"><span data-stu-id="f342c-131">Response</span></span>
<span data-ttu-id="f342c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f342c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








