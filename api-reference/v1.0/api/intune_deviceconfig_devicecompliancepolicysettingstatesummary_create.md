# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="ea080-101">deviceCompliancePolicySettingStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="ea080-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="ea080-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ea080-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea080-103">新しい [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ea080-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea080-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ea080-104">Prerequisites</span></span>
<span data-ttu-id="ea080-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea080-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ea080-107">Permission type</span></span>|<span data-ttu-id="ea080-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ea080-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea080-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ea080-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ea080-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea080-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea080-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea080-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea080-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea080-112">Not supported.</span></span>|
|<span data-ttu-id="ea080-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ea080-113">Application</span></span>|<span data-ttu-id="ea080-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea080-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea080-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea080-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ea080-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea080-116">Request headers</span></span>
|<span data-ttu-id="ea080-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea080-117">Header</span></span>|<span data-ttu-id="ea080-118">値</span><span class="sxs-lookup"><span data-stu-id="ea080-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea080-119">承認</span><span class="sxs-lookup"><span data-stu-id="ea080-119">Authorization</span></span>|<span data-ttu-id="ea080-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="ea080-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ea080-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ea080-121">Accept</span></span>|<span data-ttu-id="ea080-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ea080-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea080-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ea080-123">Request body</span></span>
<span data-ttu-id="ea080-124">要求本文で、deviceCompliancePolicySettingStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea080-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ea080-125">次の表に、deviceCompliancePolicySettingStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ea080-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ea080-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ea080-126">Property</span></span>|<span data-ttu-id="ea080-127">型</span><span class="sxs-lookup"><span data-stu-id="ea080-127">Type</span></span>|<span data-ttu-id="ea080-128">説明</span><span class="sxs-lookup"><span data-stu-id="ea080-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea080-129">setting</span><span class="sxs-lookup"><span data-stu-id="ea080-129">setting</span></span>|<span data-ttu-id="ea080-130">String</span><span class="sxs-lookup"><span data-stu-id="ea080-130">String</span></span>|<span data-ttu-id="ea080-131">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="ea080-131">The setting class name and property name.</span></span>|
|<span data-ttu-id="ea080-132">settingName</span><span class="sxs-lookup"><span data-stu-id="ea080-132">settingName</span></span>|<span data-ttu-id="ea080-133">String</span><span class="sxs-lookup"><span data-stu-id="ea080-133">String</span></span>|<span data-ttu-id="ea080-134">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="ea080-134">Name of the setting.</span></span>|
|<span data-ttu-id="ea080-135">platformType</span><span class="sxs-lookup"><span data-stu-id="ea080-135">PlatformType</span></span>|<span data-ttu-id="ea080-136">String</span><span class="sxs-lookup"><span data-stu-id="ea080-136">String</span></span>|<span data-ttu-id="ea080-137">設定のプラットフォーム。可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="ea080-137">Setting platform Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="ea080-138">id</span><span class="sxs-lookup"><span data-stu-id="ea080-138">id</span></span>|<span data-ttu-id="ea080-139">String</span><span class="sxs-lookup"><span data-stu-id="ea080-139">String</span></span>|<span data-ttu-id="ea080-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ea080-140">Name of the entity.</span></span>|
|<span data-ttu-id="ea080-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea080-141">unknownDeviceCount</span></span>|<span data-ttu-id="ea080-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ea080-142">Int32</span></span>|<span data-ttu-id="ea080-143">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ea080-143">Number of unknown devices</span></span>|
|<span data-ttu-id="ea080-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea080-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="ea080-145">Int32</span><span class="sxs-lookup"><span data-stu-id="ea080-145">Int32</span></span>|<span data-ttu-id="ea080-146">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ea080-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="ea080-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea080-147">compliantDeviceCount</span></span>|<span data-ttu-id="ea080-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ea080-148">Int32</span></span>|<span data-ttu-id="ea080-149">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ea080-149">Number of compliant devices</span></span>|
|<span data-ttu-id="ea080-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea080-150">remediatedDeviceCount</span></span>|<span data-ttu-id="ea080-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ea080-151">Int32</span></span>|<span data-ttu-id="ea080-152">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ea080-152">Number of remediated devices</span></span>|
|<span data-ttu-id="ea080-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea080-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ea080-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ea080-154">Int32</span></span>|<span data-ttu-id="ea080-155">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ea080-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="ea080-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea080-156">errorDeviceCount</span></span>|<span data-ttu-id="ea080-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ea080-157">Int32</span></span>|<span data-ttu-id="ea080-158">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ea080-158">Number of error devices</span></span>|
|<span data-ttu-id="ea080-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea080-159">conflictDeviceCount</span></span>|<span data-ttu-id="ea080-160">Int32</span><span class="sxs-lookup"><span data-stu-id="ea080-160">Int32</span></span>|<span data-ttu-id="ea080-161">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ea080-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="ea080-162">応答</span><span class="sxs-lookup"><span data-stu-id="ea080-162">Response</span></span>
<span data-ttu-id="ea080-163">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ea080-163">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea080-164">例</span><span class="sxs-lookup"><span data-stu-id="ea080-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea080-165">要求</span><span class="sxs-lookup"><span data-stu-id="ea080-165">Request</span></span>
<span data-ttu-id="ea080-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ea080-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ea080-167">応答</span><span class="sxs-lookup"><span data-stu-id="ea080-167">Response</span></span>
<span data-ttu-id="ea080-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ea080-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



