# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="12ef5-101">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="12ef5-101">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="12ef5-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="12ef5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12ef5-103">[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="12ef5-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12ef5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="12ef5-104">Prerequisites</span></span>
<span data-ttu-id="12ef5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12ef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12ef5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12ef5-107">Permission type</span></span>|<span data-ttu-id="12ef5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="12ef5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12ef5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12ef5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="12ef5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12ef5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12ef5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12ef5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12ef5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12ef5-112">Not supported.</span></span>|
|<span data-ttu-id="12ef5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12ef5-113">Application</span></span>|<span data-ttu-id="12ef5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12ef5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12ef5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12ef5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="12ef5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12ef5-116">Request headers</span></span>
|<span data-ttu-id="12ef5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12ef5-117">Header</span></span>|<span data-ttu-id="12ef5-118">値</span><span class="sxs-lookup"><span data-stu-id="12ef5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12ef5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="12ef5-119">Authorization</span></span>|<span data-ttu-id="12ef5-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="12ef5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="12ef5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="12ef5-121">Accept</span></span>|<span data-ttu-id="12ef5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="12ef5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12ef5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="12ef5-123">Request body</span></span>
<span data-ttu-id="12ef5-124">要求本文で、[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="12ef5-124">In the request body, supply a JSON representation of [ContactFolder](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="12ef5-125">次の表に、[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="12ef5-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="12ef5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12ef5-126">Property</span></span>|<span data-ttu-id="12ef5-127">型</span><span class="sxs-lookup"><span data-stu-id="12ef5-127">Type</span></span>|<span data-ttu-id="12ef5-128">説明</span><span class="sxs-lookup"><span data-stu-id="12ef5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12ef5-129">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="12ef5-129">inGracePeriodCount</span></span>|<span data-ttu-id="12ef5-130">Int32</span><span class="sxs-lookup"><span data-stu-id="12ef5-130">Int32</span></span>|<span data-ttu-id="12ef5-131">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="12ef5-131">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="12ef5-132">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="12ef5-132">configManagerCount</span></span>|<span data-ttu-id="12ef5-133">Int32</span><span class="sxs-lookup"><span data-stu-id="12ef5-133">Int32</span></span>|<span data-ttu-id="12ef5-134">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="12ef5-134">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="12ef5-135">id</span><span class="sxs-lookup"><span data-stu-id="12ef5-135">id</span></span>|<span data-ttu-id="12ef5-136">String</span><span class="sxs-lookup"><span data-stu-id="12ef5-136">String</span></span>|<span data-ttu-id="12ef5-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="12ef5-137">Name of the entity.</span></span>|
|<span data-ttu-id="12ef5-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12ef5-138">unknownDeviceCount</span></span>|<span data-ttu-id="12ef5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="12ef5-139">Int32</span></span>|<span data-ttu-id="12ef5-140">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="12ef5-140">Number of unknown devices</span></span>|
|<span data-ttu-id="12ef5-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12ef5-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="12ef5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="12ef5-142">Int32</span></span>|<span data-ttu-id="12ef5-143">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="12ef5-143">Number of not applicable devices</span></span>|
|<span data-ttu-id="12ef5-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12ef5-144">compliantDeviceCount</span></span>|<span data-ttu-id="12ef5-145">Int32</span><span class="sxs-lookup"><span data-stu-id="12ef5-145">Int32</span></span>|<span data-ttu-id="12ef5-146">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="12ef5-146">Number of compliant devices</span></span>|
|<span data-ttu-id="12ef5-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12ef5-147">remediatedDeviceCount</span></span>|<span data-ttu-id="12ef5-148">Int32</span><span class="sxs-lookup"><span data-stu-id="12ef5-148">Int32</span></span>|<span data-ttu-id="12ef5-149">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="12ef5-149">Number of remediated devices</span></span>|
|<span data-ttu-id="12ef5-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12ef5-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="12ef5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="12ef5-151">Int32</span></span>|<span data-ttu-id="12ef5-152">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="12ef5-152">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="12ef5-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12ef5-153">errorDeviceCount</span></span>|<span data-ttu-id="12ef5-154">Int32</span><span class="sxs-lookup"><span data-stu-id="12ef5-154">Int32</span></span>|<span data-ttu-id="12ef5-155">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="12ef5-155">Number of error devices</span></span>|
|<span data-ttu-id="12ef5-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12ef5-156">conflictDeviceCount</span></span>|<span data-ttu-id="12ef5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="12ef5-157">Int32</span></span>|<span data-ttu-id="12ef5-158">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="12ef5-158">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="12ef5-159">応答</span><span class="sxs-lookup"><span data-stu-id="12ef5-159">Response</span></span>
<span data-ttu-id="12ef5-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="12ef5-160">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12ef5-161">例</span><span class="sxs-lookup"><span data-stu-id="12ef5-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="12ef5-162">要求</span><span class="sxs-lookup"><span data-stu-id="12ef5-162">Request</span></span>
<span data-ttu-id="12ef5-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12ef5-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 270

{
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="12ef5-164">応答</span><span class="sxs-lookup"><span data-stu-id="12ef5-164">Response</span></span>
<span data-ttu-id="12ef5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12ef5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



