# <a name="update-reportroot"></a><span data-ttu-id="8657f-101">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="8657f-101">Update reportRoot</span></span>

> <span data-ttu-id="8657f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8657f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8657f-103">[reportRoot](../resources/intune_shared_reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8657f-103">Update the properties of a [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8657f-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="8657f-104">Prerequisites</span></span>
<span data-ttu-id="8657f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8657f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8657f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8657f-107">Permission type</span></span>|<span data-ttu-id="8657f-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8657f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8657f-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="8657f-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8657f-110">&nbsp; &nbsp; デバイス構成</span><span class="sxs-lookup"><span data-stu-id="8657f-110">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="8657f-111">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8657f-111">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8657f-112">&nbsp; &nbsp; トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="8657f-112">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="8657f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8657f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8657f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8657f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8657f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8657f-115">Not supported.</span></span>|
|<span data-ttu-id="8657f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8657f-116">Application</span></span>|<span data-ttu-id="8657f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8657f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8657f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8657f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="8657f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8657f-119">Request headers</span></span>
|<span data-ttu-id="8657f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8657f-120">Header</span></span>|<span data-ttu-id="8657f-121">値</span><span class="sxs-lookup"><span data-stu-id="8657f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8657f-122">承認</span><span class="sxs-lookup"><span data-stu-id="8657f-122">Authorization</span></span>|<span data-ttu-id="8657f-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8657f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8657f-124">承諾する</span><span class="sxs-lookup"><span data-stu-id="8657f-124">Accept</span></span>|<span data-ttu-id="8657f-125">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="8657f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8657f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8657f-126">Request body</span></span>
<span data-ttu-id="8657f-127">要求本文で、[reportRoot](../resources/intune_shared_reportroot.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8657f-127">In the request body, supply a JSON representation for the [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>

<span data-ttu-id="8657f-128">次の表に、[reportRoot](../resources/intune_shared_reportroot.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8657f-128">The following table shows the properties that are required when you create the [reportRoot](../resources/intune_shared_reportroot.md).</span></span>

|<span data-ttu-id="8657f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8657f-129">Property</span></span>|<span data-ttu-id="8657f-130">型</span><span class="sxs-lookup"><span data-stu-id="8657f-130">Type</span></span>|<span data-ttu-id="8657f-131">説明</span><span class="sxs-lookup"><span data-stu-id="8657f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8657f-132">ID</span><span class="sxs-lookup"><span data-stu-id="8657f-132">id</span></span>|<span data-ttu-id="8657f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8657f-133">String</span></span>|<span data-ttu-id="8657f-134">このエンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="8657f-134">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8657f-135">応答</span><span class="sxs-lookup"><span data-stu-id="8657f-135">Response</span></span>
<span data-ttu-id="8657f-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [reportRoot](../resources/intune_shared_reportroot.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8657f-136">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune_shared_reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8657f-137">例</span><span class="sxs-lookup"><span data-stu-id="8657f-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="8657f-138">要求</span><span class="sxs-lookup"><span data-stu-id="8657f-138">Request</span></span>
<span data-ttu-id="8657f-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8657f-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="8657f-140">応答</span><span class="sxs-lookup"><span data-stu-id="8657f-140">Response</span></span>
<span data-ttu-id="8657f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8657f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








