# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="5eccb-101">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="5eccb-101">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="5eccb-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5eccb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5eccb-103">[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5eccb-103">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5eccb-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5eccb-104">Prerequisites</span></span>
<span data-ttu-id="5eccb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5eccb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5eccb-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5eccb-107">Permission type</span></span>|<span data-ttu-id="5eccb-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5eccb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5eccb-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5eccb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5eccb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eccb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5eccb-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5eccb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5eccb-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5eccb-112">Not supported.</span></span>|
|<span data-ttu-id="5eccb-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5eccb-113">Application</span></span>|<span data-ttu-id="5eccb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5eccb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5eccb-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5eccb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="5eccb-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5eccb-116">Request headers</span></span>
|<span data-ttu-id="5eccb-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5eccb-117">Header</span></span>|<span data-ttu-id="5eccb-118">値</span><span class="sxs-lookup"><span data-stu-id="5eccb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5eccb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eccb-119">Authorization</span></span>|<span data-ttu-id="5eccb-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5eccb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5eccb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5eccb-121">Accept</span></span>|<span data-ttu-id="5eccb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5eccb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eccb-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5eccb-123">Request body</span></span>
<span data-ttu-id="5eccb-124">要求本文で、[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5eccb-124">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="5eccb-125">次の表に、[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5eccb-125">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="5eccb-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5eccb-126">Property</span></span>|<span data-ttu-id="5eccb-127">型</span><span class="sxs-lookup"><span data-stu-id="5eccb-127">Type</span></span>|<span data-ttu-id="5eccb-128">説明</span><span class="sxs-lookup"><span data-stu-id="5eccb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eccb-129">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="5eccb-129">inGracePeriodCount</span></span>|<span data-ttu-id="5eccb-130">Int32</span><span class="sxs-lookup"><span data-stu-id="5eccb-130">Int32</span></span>|<span data-ttu-id="5eccb-131">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5eccb-131">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="5eccb-132">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="5eccb-132">configManagerCount</span></span>|<span data-ttu-id="5eccb-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5eccb-133">Int32</span></span>|<span data-ttu-id="5eccb-134">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5eccb-134">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="5eccb-135">id</span><span class="sxs-lookup"><span data-stu-id="5eccb-135">id</span></span>|<span data-ttu-id="5eccb-136">String</span><span class="sxs-lookup"><span data-stu-id="5eccb-136">String</span></span>|<span data-ttu-id="5eccb-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5eccb-137">Key of the entity.</span></span>|
|<span data-ttu-id="5eccb-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eccb-138">unknownDeviceCount</span></span>|<span data-ttu-id="5eccb-139">Int32</span><span class="sxs-lookup"><span data-stu-id="5eccb-139">Int32</span></span>|<span data-ttu-id="5eccb-140">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5eccb-140">Number of unknown devices</span></span>|
|<span data-ttu-id="5eccb-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eccb-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="5eccb-142">Int32</span><span class="sxs-lookup"><span data-stu-id="5eccb-142">Int32</span></span>|<span data-ttu-id="5eccb-143">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5eccb-143">Number of not applicable devices</span></span>|
|<span data-ttu-id="5eccb-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eccb-144">compliantDeviceCount</span></span>|<span data-ttu-id="5eccb-145">Int32</span><span class="sxs-lookup"><span data-stu-id="5eccb-145">Int32</span></span>|<span data-ttu-id="5eccb-146">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="5eccb-146">Number of compliant devices</span></span>|
|<span data-ttu-id="5eccb-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eccb-147">remediatedDeviceCount</span></span>|<span data-ttu-id="5eccb-148">Int32</span><span class="sxs-lookup"><span data-stu-id="5eccb-148">Int32</span></span>|<span data-ttu-id="5eccb-149">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5eccb-149">Number of remediated devices</span></span>|
|<span data-ttu-id="5eccb-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eccb-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="5eccb-151">Int32</span><span class="sxs-lookup"><span data-stu-id="5eccb-151">Int32</span></span>|<span data-ttu-id="5eccb-152">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5eccb-152">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="5eccb-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eccb-153">errorDeviceCount</span></span>|<span data-ttu-id="5eccb-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5eccb-154">Int32</span></span>|<span data-ttu-id="5eccb-155">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="5eccb-155">Number of error devices</span></span>|
|<span data-ttu-id="5eccb-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5eccb-156">conflictDeviceCount</span></span>|<span data-ttu-id="5eccb-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5eccb-157">Int32</span></span>|<span data-ttu-id="5eccb-158">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="5eccb-158">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="5eccb-159">応答</span><span class="sxs-lookup"><span data-stu-id="5eccb-159">Response</span></span>
<span data-ttu-id="5eccb-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5eccb-160">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eccb-161">例</span><span class="sxs-lookup"><span data-stu-id="5eccb-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="5eccb-162">要求</span><span class="sxs-lookup"><span data-stu-id="5eccb-162">Request</span></span>
<span data-ttu-id="5eccb-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5eccb-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 349

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
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

### <a name="response"></a><span data-ttu-id="5eccb-164">応答</span><span class="sxs-lookup"><span data-stu-id="5eccb-164">Response</span></span>
<span data-ttu-id="5eccb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5eccb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



