# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="62f25-101">windowsInformationProtectionAppLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="62f25-101">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="62f25-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="62f25-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62f25-103">新しい [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="62f25-103">Create a new [plannerBucket](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62f25-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="62f25-104">Prerequisites</span></span>
<span data-ttu-id="62f25-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62f25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="62f25-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62f25-107">Permission type</span></span>|<span data-ttu-id="62f25-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="62f25-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62f25-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62f25-109">Delegated (work or school account)</span></span>|<span data-ttu-id="62f25-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62f25-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62f25-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62f25-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62f25-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62f25-112">Not supported.</span></span>|
|<span data-ttu-id="62f25-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62f25-113">Application</span></span>|<span data-ttu-id="62f25-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62f25-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62f25-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62f25-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="62f25-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62f25-116">Request headers</span></span>
|<span data-ttu-id="62f25-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62f25-117">Header</span></span>|<span data-ttu-id="62f25-118">値</span><span class="sxs-lookup"><span data-stu-id="62f25-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62f25-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="62f25-119">Authorization</span></span>|<span data-ttu-id="62f25-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="62f25-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="62f25-121">Accept</span><span class="sxs-lookup"><span data-stu-id="62f25-121">Accept</span></span>|<span data-ttu-id="62f25-122">application/json</span><span class="sxs-lookup"><span data-stu-id="62f25-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62f25-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="62f25-123">Request body</span></span>
<span data-ttu-id="62f25-124">要求本文で、windowsInformationProtectionAppLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="62f25-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="62f25-125">次の表に、windowsInformationProtectionAppLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="62f25-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="62f25-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62f25-126">Property</span></span>|<span data-ttu-id="62f25-127">型</span><span class="sxs-lookup"><span data-stu-id="62f25-127">Type</span></span>|<span data-ttu-id="62f25-128">説明</span><span class="sxs-lookup"><span data-stu-id="62f25-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f25-129">id</span><span class="sxs-lookup"><span data-stu-id="62f25-129">id</span></span>|<span data-ttu-id="62f25-130">String</span><span class="sxs-lookup"><span data-stu-id="62f25-130">String</span></span>|<span data-ttu-id="62f25-131">WindowsInformationProtectionAppLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="62f25-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="62f25-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="62f25-132">applicationName</span></span>|<span data-ttu-id="62f25-133">String</span><span class="sxs-lookup"><span data-stu-id="62f25-133">String</span></span>|<span data-ttu-id="62f25-134">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="62f25-134">Application Name</span></span>|
|<span data-ttu-id="62f25-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="62f25-135">applicationType</span></span>|<span data-ttu-id="62f25-136">String</span><span class="sxs-lookup"><span data-stu-id="62f25-136">String</span></span>|<span data-ttu-id="62f25-137">アプリケーションの種類。可能な値は、`universal`、`desktop` です。</span><span class="sxs-lookup"><span data-stu-id="62f25-137">Application Type Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="62f25-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="62f25-138">deviceCount</span></span>|<span data-ttu-id="62f25-139">Int32</span><span class="sxs-lookup"><span data-stu-id="62f25-139">Int32</span></span>|<span data-ttu-id="62f25-140">デバイス数</span><span class="sxs-lookup"><span data-stu-id="62f25-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="62f25-141">応答</span><span class="sxs-lookup"><span data-stu-id="62f25-141">Response</span></span>
<span data-ttu-id="62f25-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="62f25-142">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62f25-143">例</span><span class="sxs-lookup"><span data-stu-id="62f25-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="62f25-144">要求</span><span class="sxs-lookup"><span data-stu-id="62f25-144">Request</span></span>
<span data-ttu-id="62f25-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="62f25-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="62f25-146">応答</span><span class="sxs-lookup"><span data-stu-id="62f25-146">Response</span></span>
<span data-ttu-id="62f25-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="62f25-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```



