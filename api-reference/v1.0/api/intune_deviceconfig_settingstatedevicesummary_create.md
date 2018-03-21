# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="d73f0-101">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="d73f0-101">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="d73f0-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d73f0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d73f0-103">新しい [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d73f0-103">Create a new [plannerBucket](../resources/intune_deviceconfig_settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d73f0-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="d73f0-104">Prerequisites</span></span>
<span data-ttu-id="d73f0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d73f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d73f0-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d73f0-107">Permission type</span></span>|<span data-ttu-id="d73f0-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d73f0-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d73f0-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d73f0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d73f0-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d73f0-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d73f0-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d73f0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d73f0-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d73f0-112">Not supported.</span></span>|
|<span data-ttu-id="d73f0-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d73f0-113">Application</span></span>|<span data-ttu-id="d73f0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d73f0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d73f0-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d73f0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d73f0-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d73f0-116">Request headers</span></span>
|<span data-ttu-id="d73f0-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d73f0-117">Header</span></span>|<span data-ttu-id="d73f0-118">値</span><span class="sxs-lookup"><span data-stu-id="d73f0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d73f0-119">承認</span><span class="sxs-lookup"><span data-stu-id="d73f0-119">Authorization</span></span>|<span data-ttu-id="d73f0-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="d73f0-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d73f0-121">承諾</span><span class="sxs-lookup"><span data-stu-id="d73f0-121">Accept</span></span>|<span data-ttu-id="d73f0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d73f0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d73f0-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d73f0-123">Request body</span></span>
<span data-ttu-id="d73f0-124">要求本文で、settingStateDeviceSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d73f0-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="d73f0-125">次の表に、settingStateDeviceSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d73f0-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d73f0-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d73f0-126">Property</span></span>|<span data-ttu-id="d73f0-127">型</span><span class="sxs-lookup"><span data-stu-id="d73f0-127">Type</span></span>|<span data-ttu-id="d73f0-128">説明</span><span class="sxs-lookup"><span data-stu-id="d73f0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d73f0-129">id</span><span class="sxs-lookup"><span data-stu-id="d73f0-129">id</span></span>|<span data-ttu-id="d73f0-130">String</span><span class="sxs-lookup"><span data-stu-id="d73f0-130">String</span></span>|<span data-ttu-id="d73f0-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d73f0-131">Name of the entity.</span></span>|
|<span data-ttu-id="d73f0-132">settingName</span><span class="sxs-lookup"><span data-stu-id="d73f0-132">settingName</span></span>|<span data-ttu-id="d73f0-133">String</span><span class="sxs-lookup"><span data-stu-id="d73f0-133">String</span></span>|<span data-ttu-id="d73f0-134">設定の名前</span><span class="sxs-lookup"><span data-stu-id="d73f0-134">Name of the setting.</span></span>|
|<span data-ttu-id="d73f0-135">instancePath</span><span class="sxs-lookup"><span data-stu-id="d73f0-135">instancePath</span></span>|<span data-ttu-id="d73f0-136">String</span><span class="sxs-lookup"><span data-stu-id="d73f0-136">String</span></span>|<span data-ttu-id="d73f0-137">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="d73f0-137">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="d73f0-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d73f0-138">unknownDeviceCount</span></span>|<span data-ttu-id="d73f0-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d73f0-139">Int32</span></span>|<span data-ttu-id="d73f0-140">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d73f0-140">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="d73f0-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d73f0-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="d73f0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d73f0-142">Int32</span></span>|<span data-ttu-id="d73f0-143">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d73f0-143">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="d73f0-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d73f0-144">compliantDeviceCount</span></span>|<span data-ttu-id="d73f0-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d73f0-145">Int32</span></span>|<span data-ttu-id="d73f0-146">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d73f0-146">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="d73f0-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d73f0-147">remediatedDeviceCount</span></span>|<span data-ttu-id="d73f0-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d73f0-148">Int32</span></span>|<span data-ttu-id="d73f0-149">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d73f0-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="d73f0-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d73f0-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d73f0-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d73f0-151">Int32</span></span>|<span data-ttu-id="d73f0-152">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d73f0-152">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="d73f0-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d73f0-153">errorDeviceCount</span></span>|<span data-ttu-id="d73f0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d73f0-154">Int32</span></span>|<span data-ttu-id="d73f0-155">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="d73f0-155">Device error count for the setting</span></span>|
|<span data-ttu-id="d73f0-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d73f0-156">conflictDeviceCount</span></span>|<span data-ttu-id="d73f0-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d73f0-157">Int32</span></span>|<span data-ttu-id="d73f0-158">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="d73f0-158">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="d73f0-159">応答</span><span class="sxs-lookup"><span data-stu-id="d73f0-159">Response</span></span>
<span data-ttu-id="d73f0-160">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d73f0-160">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d73f0-161">例</span><span class="sxs-lookup"><span data-stu-id="d73f0-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="d73f0-162">要求</span><span class="sxs-lookup"><span data-stu-id="d73f0-162">Request</span></span>
<span data-ttu-id="d73f0-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d73f0-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="d73f0-164">応答</span><span class="sxs-lookup"><span data-stu-id="d73f0-164">Response</span></span>
<span data-ttu-id="d73f0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d73f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



