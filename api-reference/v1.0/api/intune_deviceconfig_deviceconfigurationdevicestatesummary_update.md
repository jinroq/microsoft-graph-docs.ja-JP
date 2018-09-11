# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="2a6d5-101">deviceConfigurationDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="2a6d5-101">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="2a6d5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a6d5-103">[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-103">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a6d5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2a6d5-104">Prerequisites</span></span>
<span data-ttu-id="2a6d5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a6d5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a6d5-107">Permission type</span></span>|<span data-ttu-id="2a6d5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a6d5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a6d5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a6d5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2a6d5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6d5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a6d5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a6d5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a6d5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-112">Not supported.</span></span>|
|<span data-ttu-id="2a6d5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a6d5-113">Application</span></span>|<span data-ttu-id="2a6d5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a6d5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a6d5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="2a6d5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a6d5-116">Request headers</span></span>
|<span data-ttu-id="2a6d5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a6d5-117">Header</span></span>|<span data-ttu-id="2a6d5-118">値</span><span class="sxs-lookup"><span data-stu-id="2a6d5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a6d5-119">承認</span><span class="sxs-lookup"><span data-stu-id="2a6d5-119">Authorization</span></span>|<span data-ttu-id="2a6d5-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a6d5-121">承諾</span><span class="sxs-lookup"><span data-stu-id="2a6d5-121">Accept</span></span>|<span data-ttu-id="2a6d5-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="2a6d5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a6d5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a6d5-123">Request body</span></span>
<span data-ttu-id="2a6d5-124">要求本文で、[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="2a6d5-125">次の表に、[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-125">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="2a6d5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a6d5-126">Property</span></span>|<span data-ttu-id="2a6d5-127">型</span><span class="sxs-lookup"><span data-stu-id="2a6d5-127">Type</span></span>|<span data-ttu-id="2a6d5-128">説明</span><span class="sxs-lookup"><span data-stu-id="2a6d5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a6d5-129">ID</span><span class="sxs-lookup"><span data-stu-id="2a6d5-129">id</span></span>|<span data-ttu-id="2a6d5-130">文字列</span><span class="sxs-lookup"><span data-stu-id="2a6d5-130">String</span></span>|<span data-ttu-id="2a6d5-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-131">Key of the entity.</span></span>|
|<span data-ttu-id="2a6d5-132">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a6d5-132">unknownDeviceCount</span></span>|<span data-ttu-id="2a6d5-133">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6d5-133">Int32</span></span>|<span data-ttu-id="2a6d5-134">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2a6d5-134">Number of unknown devices</span></span>|
|<span data-ttu-id="2a6d5-135">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a6d5-135">notApplicableDeviceCount</span></span>|<span data-ttu-id="2a6d5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6d5-136">Int32</span></span>|<span data-ttu-id="2a6d5-137">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2a6d5-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="2a6d5-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a6d5-138">compliantDeviceCount</span></span>|<span data-ttu-id="2a6d5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6d5-139">Int32</span></span>|<span data-ttu-id="2a6d5-140">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="2a6d5-140">Number of compliant devices</span></span>|
|<span data-ttu-id="2a6d5-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a6d5-141">remediatedDeviceCount</span></span>|<span data-ttu-id="2a6d5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6d5-142">Int32</span></span>|<span data-ttu-id="2a6d5-143">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2a6d5-143">Number of remediated devices</span></span>|
|<span data-ttu-id="2a6d5-144">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a6d5-144">nonCompliantDeviceCount</span></span>|<span data-ttu-id="2a6d5-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6d5-145">Int32</span></span>|<span data-ttu-id="2a6d5-146">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2a6d5-146">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="2a6d5-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a6d5-147">errorDeviceCount</span></span>|<span data-ttu-id="2a6d5-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6d5-148">Int32</span></span>|<span data-ttu-id="2a6d5-149">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="2a6d5-149">Number of error devices</span></span>|
|<span data-ttu-id="2a6d5-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a6d5-150">conflictDeviceCount</span></span>|<span data-ttu-id="2a6d5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6d5-151">Int32</span></span>|<span data-ttu-id="2a6d5-152">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="2a6d5-152">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="2a6d5-153">応答</span><span class="sxs-lookup"><span data-stu-id="2a6d5-153">Response</span></span>
<span data-ttu-id="2a6d5-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-154">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a6d5-155">例</span><span class="sxs-lookup"><span data-stu-id="2a6d5-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a6d5-156">要求</span><span class="sxs-lookup"><span data-stu-id="2a6d5-156">Request</span></span>
<span data-ttu-id="2a6d5-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="2a6d5-158">応答</span><span class="sxs-lookup"><span data-stu-id="2a6d5-158">Response</span></span>
<span data-ttu-id="2a6d5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2a6d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```








