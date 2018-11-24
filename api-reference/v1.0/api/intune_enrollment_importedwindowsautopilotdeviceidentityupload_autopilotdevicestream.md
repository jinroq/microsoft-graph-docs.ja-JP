# <a name="autopilotdevicestream-function"></a><span data-ttu-id="e7ff9-101">autopilotDeviceStream 関数</span><span class="sxs-lookup"><span data-stu-id="e7ff9-101">autopilotDeviceStream function</span></span>

> <span data-ttu-id="e7ff9-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7ff9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7ff9-103">自動操縦デバイスのストリーム内でのアップロード要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="e7ff9-103">Create a upload request with autopilot device stream in it.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7ff9-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e7ff9-104">Prerequisites</span></span>
<span data-ttu-id="e7ff9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7ff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7ff9-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7ff9-107">Permission type</span></span>|<span data-ttu-id="e7ff9-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7ff9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7ff9-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7ff9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e7ff9-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7ff9-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e7ff9-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7ff9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7ff9-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7ff9-112">Not supported.</span></span>|
|<span data-ttu-id="e7ff9-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7ff9-113">Application</span></span>|<span data-ttu-id="e7ff9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7ff9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7ff9-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7ff9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="e7ff9-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7ff9-116">Request headers</span></span>
|<span data-ttu-id="e7ff9-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7ff9-117">Header</span></span>|<span data-ttu-id="e7ff9-118">値</span><span class="sxs-lookup"><span data-stu-id="e7ff9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7ff9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7ff9-119">Authorization</span></span>|<span data-ttu-id="e7ff9-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e7ff9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7ff9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e7ff9-121">Accept</span></span>|<span data-ttu-id="e7ff9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e7ff9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7ff9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7ff9-123">Request body</span></span>
<span data-ttu-id="e7ff9-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7ff9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7ff9-125">応答</span><span class="sxs-lookup"><span data-stu-id="e7ff9-125">Response</span></span>
<span data-ttu-id="e7ff9-126">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String を返します。</span><span class="sxs-lookup"><span data-stu-id="e7ff9-126">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7ff9-127">例</span><span class="sxs-lookup"><span data-stu-id="e7ff9-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7ff9-128">要求</span><span class="sxs-lookup"><span data-stu-id="e7ff9-128">Request</span></span>
<span data-ttu-id="e7ff9-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e7ff9-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="e7ff9-130">応答</span><span class="sxs-lookup"><span data-stu-id="e7ff9-130">Response</span></span>
<span data-ttu-id="e7ff9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7ff9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```



