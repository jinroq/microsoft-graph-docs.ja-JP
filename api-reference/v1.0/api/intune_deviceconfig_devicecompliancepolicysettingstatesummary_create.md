# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="fdd00-101">deviceCompliancePolicySettingStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="fdd00-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="fdd00-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fdd00-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdd00-103">新しい [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fdd00-103">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fdd00-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="fdd00-104">Prerequisites</span></span>
<span data-ttu-id="fdd00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fdd00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fdd00-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fdd00-107">Permission type</span></span>|<span data-ttu-id="fdd00-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fdd00-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdd00-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fdd00-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fdd00-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd00-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fdd00-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fdd00-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdd00-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fdd00-112">Not supported.</span></span>|
|<span data-ttu-id="fdd00-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fdd00-113">Application</span></span>|<span data-ttu-id="fdd00-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fdd00-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdd00-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fdd00-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="fdd00-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fdd00-116">Request headers</span></span>
|<span data-ttu-id="fdd00-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fdd00-117">Header</span></span>|<span data-ttu-id="fdd00-118">値</span><span class="sxs-lookup"><span data-stu-id="fdd00-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdd00-119">承認</span><span class="sxs-lookup"><span data-stu-id="fdd00-119">Authorization</span></span>|<span data-ttu-id="fdd00-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="fdd00-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdd00-121">承諾</span><span class="sxs-lookup"><span data-stu-id="fdd00-121">Accept</span></span>|<span data-ttu-id="fdd00-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fdd00-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdd00-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="fdd00-123">Request body</span></span>
<span data-ttu-id="fdd00-124">要求本文で、deviceCompliancePolicySettingStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fdd00-124">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="fdd00-125">次の表に、deviceCompliancePolicySettingStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fdd00-125">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="fdd00-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fdd00-126">Property</span></span>|<span data-ttu-id="fdd00-127">型</span><span class="sxs-lookup"><span data-stu-id="fdd00-127">Type</span></span>|<span data-ttu-id="fdd00-128">説明</span><span class="sxs-lookup"><span data-stu-id="fdd00-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdd00-129">id</span><span class="sxs-lookup"><span data-stu-id="fdd00-129">id</span></span>|<span data-ttu-id="fdd00-130">String</span><span class="sxs-lookup"><span data-stu-id="fdd00-130">String</span></span>|<span data-ttu-id="fdd00-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fdd00-131">Key of the entity.</span></span>|
|<span data-ttu-id="fdd00-132">setting</span><span class="sxs-lookup"><span data-stu-id="fdd00-132">setting</span></span>|<span data-ttu-id="fdd00-133">String</span><span class="sxs-lookup"><span data-stu-id="fdd00-133">String</span></span>|<span data-ttu-id="fdd00-134">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="fdd00-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="fdd00-135">settingName</span><span class="sxs-lookup"><span data-stu-id="fdd00-135">settingName</span></span>|<span data-ttu-id="fdd00-136">String</span><span class="sxs-lookup"><span data-stu-id="fdd00-136">String</span></span>|<span data-ttu-id="fdd00-137">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="fdd00-137">Name of the setting.</span></span>|
|<span data-ttu-id="fdd00-138">platformType</span><span class="sxs-lookup"><span data-stu-id="fdd00-138">platformType</span></span>|[<span data-ttu-id="fdd00-139">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="fdd00-139">policyPlatformType</span></span>](../resources/intune_deviceconfig_policyplatformtype.md)|<span data-ttu-id="fdd00-140">設定のプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="fdd00-140">Setting platform.</span></span> <span data-ttu-id="fdd00-141">可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="fdd00-141">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="fdd00-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fdd00-142">unknownDeviceCount</span></span>|<span data-ttu-id="fdd00-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fdd00-143">Int32</span></span>|<span data-ttu-id="fdd00-144">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="fdd00-144">Number of unknown devices</span></span>|
|<span data-ttu-id="fdd00-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fdd00-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="fdd00-146">Int32</span><span class="sxs-lookup"><span data-stu-id="fdd00-146">Int32</span></span>|<span data-ttu-id="fdd00-147">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="fdd00-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="fdd00-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fdd00-148">compliantDeviceCount</span></span>|<span data-ttu-id="fdd00-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fdd00-149">Int32</span></span>|<span data-ttu-id="fdd00-150">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="fdd00-150">Number of compliant devices</span></span>|
|<span data-ttu-id="fdd00-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fdd00-151">remediatedDeviceCount</span></span>|<span data-ttu-id="fdd00-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fdd00-152">Int32</span></span>|<span data-ttu-id="fdd00-153">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="fdd00-153">Number of remediated devices</span></span>|
|<span data-ttu-id="fdd00-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fdd00-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="fdd00-155">Int32</span><span class="sxs-lookup"><span data-stu-id="fdd00-155">Int32</span></span>|<span data-ttu-id="fdd00-156">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="fdd00-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="fdd00-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fdd00-157">errorDeviceCount</span></span>|<span data-ttu-id="fdd00-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fdd00-158">Int32</span></span>|<span data-ttu-id="fdd00-159">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="fdd00-159">Number of error devices</span></span>|
|<span data-ttu-id="fdd00-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fdd00-160">conflictDeviceCount</span></span>|<span data-ttu-id="fdd00-161">Int32</span><span class="sxs-lookup"><span data-stu-id="fdd00-161">Int32</span></span>|<span data-ttu-id="fdd00-162">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="fdd00-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="fdd00-163">応答</span><span class="sxs-lookup"><span data-stu-id="fdd00-163">Response</span></span>
<span data-ttu-id="fdd00-164">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fdd00-164">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdd00-165">例</span><span class="sxs-lookup"><span data-stu-id="fdd00-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="fdd00-166">要求</span><span class="sxs-lookup"><span data-stu-id="fdd00-166">Request</span></span>
<span data-ttu-id="fdd00-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fdd00-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="fdd00-168">応答</span><span class="sxs-lookup"><span data-stu-id="fdd00-168">Response</span></span>
<span data-ttu-id="fdd00-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fdd00-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



