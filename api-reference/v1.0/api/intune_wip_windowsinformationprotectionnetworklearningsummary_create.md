# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="b9b3a-101">windowsInformationProtectionNetworkLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="b9b3a-101">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="b9b3a-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9b3a-103">新しい [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-103">Create a new [plannerBucket](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9b3a-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b9b3a-104">Prerequisites</span></span>
<span data-ttu-id="b9b3a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9b3a-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9b3a-107">Permission type</span></span>|<span data-ttu-id="b9b3a-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9b3a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9b3a-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9b3a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b9b3a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9b3a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b9b3a-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9b3a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9b3a-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-112">Not supported.</span></span>|
|<span data-ttu-id="b9b3a-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9b3a-113">Application</span></span>|<span data-ttu-id="b9b3a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9b3a-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9b3a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="b9b3a-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9b3a-116">Request headers</span></span>
|<span data-ttu-id="b9b3a-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9b3a-117">Header</span></span>|<span data-ttu-id="b9b3a-118">値</span><span class="sxs-lookup"><span data-stu-id="b9b3a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9b3a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9b3a-119">Authorization</span></span>|<span data-ttu-id="b9b3a-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b9b3a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b9b3a-121">Accept</span></span>|<span data-ttu-id="b9b3a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b9b3a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9b3a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9b3a-123">Request body</span></span>
<span data-ttu-id="b9b3a-124">要求本文で、windowsInformationProtectionNetworkLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="b9b3a-125">次の表に、windowsInformationProtectionNetworkLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="b9b3a-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9b3a-126">Property</span></span>|<span data-ttu-id="b9b3a-127">型</span><span class="sxs-lookup"><span data-stu-id="b9b3a-127">Type</span></span>|<span data-ttu-id="b9b3a-128">説明</span><span class="sxs-lookup"><span data-stu-id="b9b3a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9b3a-129">id</span><span class="sxs-lookup"><span data-stu-id="b9b3a-129">id</span></span>|<span data-ttu-id="b9b3a-130">String</span><span class="sxs-lookup"><span data-stu-id="b9b3a-130">String</span></span>|<span data-ttu-id="b9b3a-131">WindowsInformationProtectionNetworkLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-131">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="b9b3a-132">url</span><span class="sxs-lookup"><span data-stu-id="b9b3a-132">url</span></span>|<span data-ttu-id="b9b3a-133">String</span><span class="sxs-lookup"><span data-stu-id="b9b3a-133">String</span></span>|<span data-ttu-id="b9b3a-134">Web サイト URL</span><span class="sxs-lookup"><span data-stu-id="b9b3a-134">Website url</span></span>|
|<span data-ttu-id="b9b3a-135">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b9b3a-135">deviceCount</span></span>|<span data-ttu-id="b9b3a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b9b3a-136">Int32</span></span>|<span data-ttu-id="b9b3a-137">デバイス数</span><span class="sxs-lookup"><span data-stu-id="b9b3a-137">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="b9b3a-138">応答</span><span class="sxs-lookup"><span data-stu-id="b9b3a-138">Response</span></span>
<span data-ttu-id="b9b3a-139">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-139">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9b3a-140">例</span><span class="sxs-lookup"><span data-stu-id="b9b3a-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9b3a-141">要求</span><span class="sxs-lookup"><span data-stu-id="b9b3a-141">Request</span></span>
<span data-ttu-id="b9b3a-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="b9b3a-143">応答</span><span class="sxs-lookup"><span data-stu-id="b9b3a-143">Response</span></span>
<span data-ttu-id="b9b3a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b9b3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```



