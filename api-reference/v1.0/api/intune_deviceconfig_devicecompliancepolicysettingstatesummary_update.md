# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="affc9-101">deviceCompliancePolicySettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="affc9-101">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="affc9-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="affc9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="affc9-103">[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="affc9-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="affc9-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="affc9-104">Prerequisites</span></span>
<span data-ttu-id="affc9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="affc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="affc9-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="affc9-107">Permission type</span></span>|<span data-ttu-id="affc9-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="affc9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="affc9-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="affc9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="affc9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="affc9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="affc9-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="affc9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="affc9-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="affc9-112">Not supported.</span></span>|
|<span data-ttu-id="affc9-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="affc9-113">Application</span></span>|<span data-ttu-id="affc9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="affc9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="affc9-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="affc9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="affc9-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="affc9-116">Request headers</span></span>
|<span data-ttu-id="affc9-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="affc9-117">Header</span></span>|<span data-ttu-id="affc9-118">値</span><span class="sxs-lookup"><span data-stu-id="affc9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="affc9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="affc9-119">Authorization</span></span>|<span data-ttu-id="affc9-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="affc9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="affc9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="affc9-121">Accept</span></span>|<span data-ttu-id="affc9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="affc9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="affc9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="affc9-123">Request body</span></span>
<span data-ttu-id="affc9-124">要求本文で、[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="affc9-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="affc9-125">次の表に、[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="affc9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="affc9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="affc9-126">Property</span></span>|<span data-ttu-id="affc9-127">型</span><span class="sxs-lookup"><span data-stu-id="affc9-127">Type</span></span>|<span data-ttu-id="affc9-128">説明</span><span class="sxs-lookup"><span data-stu-id="affc9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="affc9-129">setting</span><span class="sxs-lookup"><span data-stu-id="affc9-129">setting</span></span>|<span data-ttu-id="affc9-130">String</span><span class="sxs-lookup"><span data-stu-id="affc9-130">String</span></span>|<span data-ttu-id="affc9-131">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="affc9-131">The setting class name and property name.</span></span>|
|<span data-ttu-id="affc9-132">settingName</span><span class="sxs-lookup"><span data-stu-id="affc9-132">settingName</span></span>|<span data-ttu-id="affc9-133">String</span><span class="sxs-lookup"><span data-stu-id="affc9-133">String</span></span>|<span data-ttu-id="affc9-134">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="affc9-134">Name of the setting.</span></span>|
|<span data-ttu-id="affc9-135">platformType</span><span class="sxs-lookup"><span data-stu-id="affc9-135">PlatformType</span></span>|<span data-ttu-id="affc9-136">String</span><span class="sxs-lookup"><span data-stu-id="affc9-136">String</span></span>|<span data-ttu-id="affc9-137">設定のプラットフォーム。可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="affc9-137">Setting platform Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="affc9-138">id</span><span class="sxs-lookup"><span data-stu-id="affc9-138">id</span></span>|<span data-ttu-id="affc9-139">String</span><span class="sxs-lookup"><span data-stu-id="affc9-139">String</span></span>|<span data-ttu-id="affc9-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="affc9-140">Name of the entity.</span></span>|
|<span data-ttu-id="affc9-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="affc9-141">unknownDeviceCount</span></span>|<span data-ttu-id="affc9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="affc9-142">Int32</span></span>|<span data-ttu-id="affc9-143">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="affc9-143">Number of unknown devices</span></span>|
|<span data-ttu-id="affc9-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="affc9-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="affc9-145">Int32</span><span class="sxs-lookup"><span data-stu-id="affc9-145">Int32</span></span>|<span data-ttu-id="affc9-146">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="affc9-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="affc9-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="affc9-147">compliantDeviceCount</span></span>|<span data-ttu-id="affc9-148">Int32</span><span class="sxs-lookup"><span data-stu-id="affc9-148">Int32</span></span>|<span data-ttu-id="affc9-149">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="affc9-149">Number of compliant devices</span></span>|
|<span data-ttu-id="affc9-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="affc9-150">remediatedDeviceCount</span></span>|<span data-ttu-id="affc9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="affc9-151">Int32</span></span>|<span data-ttu-id="affc9-152">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="affc9-152">Number of remediated devices</span></span>|
|<span data-ttu-id="affc9-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="affc9-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="affc9-154">Int32</span><span class="sxs-lookup"><span data-stu-id="affc9-154">Int32</span></span>|<span data-ttu-id="affc9-155">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="affc9-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="affc9-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="affc9-156">errorDeviceCount</span></span>|<span data-ttu-id="affc9-157">Int32</span><span class="sxs-lookup"><span data-stu-id="affc9-157">Int32</span></span>|<span data-ttu-id="affc9-158">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="affc9-158">Number of error devices</span></span>|
|<span data-ttu-id="affc9-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="affc9-159">conflictDeviceCount</span></span>|<span data-ttu-id="affc9-160">Int32</span><span class="sxs-lookup"><span data-stu-id="affc9-160">Int32</span></span>|<span data-ttu-id="affc9-161">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="affc9-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="affc9-162">応答</span><span class="sxs-lookup"><span data-stu-id="affc9-162">Response</span></span>
<span data-ttu-id="affc9-163">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="affc9-163">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="affc9-164">例</span><span class="sxs-lookup"><span data-stu-id="affc9-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="affc9-165">要求</span><span class="sxs-lookup"><span data-stu-id="affc9-165">Request</span></span>
<span data-ttu-id="affc9-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="affc9-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 311

{
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

### <a name="response"></a><span data-ttu-id="affc9-167">応答</span><span class="sxs-lookup"><span data-stu-id="affc9-167">Response</span></span>
<span data-ttu-id="affc9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="affc9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



