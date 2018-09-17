# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="b345d-101">windowsInformationProtectionAppLearningSummary の更新</span><span class="sxs-lookup"><span data-stu-id="b345d-101">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="b345d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b345d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b345d-103">[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b345d-103">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b345d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b345d-104">Prerequisites</span></span>
<span data-ttu-id="b345d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b345d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b345d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b345d-107">Permission type</span></span>|<span data-ttu-id="b345d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b345d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b345d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b345d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b345d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b345d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b345d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b345d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b345d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b345d-112">Not supported.</span></span>|
|<span data-ttu-id="b345d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b345d-113">Application</span></span>|<span data-ttu-id="b345d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b345d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b345d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b345d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b345d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b345d-116">Request headers</span></span>
|<span data-ttu-id="b345d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b345d-117">Header</span></span>|<span data-ttu-id="b345d-118">値</span><span class="sxs-lookup"><span data-stu-id="b345d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b345d-119">承認</span><span class="sxs-lookup"><span data-stu-id="b345d-119">Authorization</span></span>|<span data-ttu-id="b345d-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b345d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b345d-121">承諾</span><span class="sxs-lookup"><span data-stu-id="b345d-121">Accept</span></span>|<span data-ttu-id="b345d-122">アプリケーション/json</span><span class="sxs-lookup"><span data-stu-id="b345d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b345d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b345d-123">Request body</span></span>
<span data-ttu-id="b345d-124">要求本文で、[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b345d-124">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="b345d-125">次の表に、[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b345d-125">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="b345d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b345d-126">Property</span></span>|<span data-ttu-id="b345d-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="b345d-127">Type</span></span>|<span data-ttu-id="b345d-128">説明</span><span class="sxs-lookup"><span data-stu-id="b345d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b345d-129">ID</span><span class="sxs-lookup"><span data-stu-id="b345d-129">id</span></span>|<span data-ttu-id="b345d-130">文字列</span><span class="sxs-lookup"><span data-stu-id="b345d-130">String</span></span>|<span data-ttu-id="b345d-131">WindowsInformationProtectionAppLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b345d-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="b345d-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="b345d-132">applicationName</span></span>|<span data-ttu-id="b345d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b345d-133">String</span></span>|<span data-ttu-id="b345d-134">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="b345d-134">Application Name</span></span>|
|<span data-ttu-id="b345d-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="b345d-135">applicationType</span></span>|[<span data-ttu-id="b345d-136">applicationType</span><span class="sxs-lookup"><span data-stu-id="b345d-136">applicationType</span></span>](../resources/intune_wip_applicationtype.md)|<span data-ttu-id="b345d-p102">アプリケーションの種類。可能な値は、`universal`、`desktop` です。</span><span class="sxs-lookup"><span data-stu-id="b345d-p102">Application Type Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="b345d-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b345d-139">deviceCount</span></span>|<span data-ttu-id="b345d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b345d-140">Int32</span></span>|<span data-ttu-id="b345d-141">デバイス数</span><span class="sxs-lookup"><span data-stu-id="b345d-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="b345d-142">応答</span><span class="sxs-lookup"><span data-stu-id="b345d-142">Response</span></span>
<span data-ttu-id="b345d-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b345d-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b345d-144">例</span><span class="sxs-lookup"><span data-stu-id="b345d-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="b345d-145">要求</span><span class="sxs-lookup"><span data-stu-id="b345d-145">Request</span></span>
<span data-ttu-id="b345d-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b345d-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 106

{
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="b345d-147">応答</span><span class="sxs-lookup"><span data-stu-id="b345d-147">Response</span></span>
<span data-ttu-id="b345d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b345d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








