# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="838a7-101">deviceCompliancePolicySettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="838a7-101">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="838a7-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="838a7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="838a7-103">[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="838a7-103">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="838a7-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="838a7-104">Prerequisites</span></span>
<span data-ttu-id="838a7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="838a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="838a7-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="838a7-107">Permission type</span></span>|<span data-ttu-id="838a7-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="838a7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="838a7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="838a7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="838a7-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="838a7-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="838a7-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="838a7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="838a7-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="838a7-112">Not supported.</span></span>|
|<span data-ttu-id="838a7-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="838a7-113">Application</span></span>|<span data-ttu-id="838a7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="838a7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="838a7-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="838a7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="838a7-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="838a7-116">Request headers</span></span>
|<span data-ttu-id="838a7-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="838a7-117">Header</span></span>|<span data-ttu-id="838a7-118">値</span><span class="sxs-lookup"><span data-stu-id="838a7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="838a7-119">承認</span><span class="sxs-lookup"><span data-stu-id="838a7-119">Authorization</span></span>|<span data-ttu-id="838a7-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="838a7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="838a7-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="838a7-121">Accept</span></span>|<span data-ttu-id="838a7-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="838a7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="838a7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="838a7-123">Request body</span></span>
<span data-ttu-id="838a7-124">要求本文で、[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="838a7-124">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="838a7-125">次の表に、[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="838a7-125">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="838a7-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="838a7-126">Property</span></span>|<span data-ttu-id="838a7-127">型</span><span class="sxs-lookup"><span data-stu-id="838a7-127">Type</span></span>|<span data-ttu-id="838a7-128">説明</span><span class="sxs-lookup"><span data-stu-id="838a7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="838a7-129">ID</span><span class="sxs-lookup"><span data-stu-id="838a7-129">id</span></span>|<span data-ttu-id="838a7-130">文字列</span><span class="sxs-lookup"><span data-stu-id="838a7-130">String</span></span>|<span data-ttu-id="838a7-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="838a7-131">Key of the entity.</span></span>|
|<span data-ttu-id="838a7-132">設定</span><span class="sxs-lookup"><span data-stu-id="838a7-132">setting</span></span>|<span data-ttu-id="838a7-133">文字列</span><span class="sxs-lookup"><span data-stu-id="838a7-133">String</span></span>|<span data-ttu-id="838a7-134">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="838a7-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="838a7-135">settingName</span><span class="sxs-lookup"><span data-stu-id="838a7-135">settingName</span></span>|<span data-ttu-id="838a7-136">文字列</span><span class="sxs-lookup"><span data-stu-id="838a7-136">String</span></span>|<span data-ttu-id="838a7-137">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="838a7-137">Name of the setting.</span></span>|
|<span data-ttu-id="838a7-138">platformType</span><span class="sxs-lookup"><span data-stu-id="838a7-138">platformType</span></span>|[<span data-ttu-id="838a7-139">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="838a7-139">policyPlatformType</span></span>](../resources/intune_deviceconfig_policyplatformtype.md)|<span data-ttu-id="838a7-140">設定のプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="838a7-140">Setting platform.</span></span> <span data-ttu-id="838a7-141">可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="838a7-141">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="838a7-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="838a7-142">unknownDeviceCount</span></span>|<span data-ttu-id="838a7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="838a7-143">Int32</span></span>|<span data-ttu-id="838a7-144">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="838a7-144">Number of unknown devices</span></span>|
|<span data-ttu-id="838a7-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="838a7-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="838a7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="838a7-146">Int32</span></span>|<span data-ttu-id="838a7-147">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="838a7-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="838a7-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="838a7-148">compliantDeviceCount</span></span>|<span data-ttu-id="838a7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="838a7-149">Int32</span></span>|<span data-ttu-id="838a7-150">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="838a7-150">Number of compliant devices</span></span>|
|<span data-ttu-id="838a7-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="838a7-151">remediatedDeviceCount</span></span>|<span data-ttu-id="838a7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="838a7-152">Int32</span></span>|<span data-ttu-id="838a7-153">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="838a7-153">Number of remediated devices</span></span>|
|<span data-ttu-id="838a7-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="838a7-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="838a7-155">Int32</span><span class="sxs-lookup"><span data-stu-id="838a7-155">Int32</span></span>|<span data-ttu-id="838a7-156">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="838a7-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="838a7-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="838a7-157">errorDeviceCount</span></span>|<span data-ttu-id="838a7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="838a7-158">Int32</span></span>|<span data-ttu-id="838a7-159">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="838a7-159">Number of error devices</span></span>|
|<span data-ttu-id="838a7-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="838a7-160">conflictDeviceCount</span></span>|<span data-ttu-id="838a7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="838a7-161">Int32</span></span>|<span data-ttu-id="838a7-162">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="838a7-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="838a7-163">応答</span><span class="sxs-lookup"><span data-stu-id="838a7-163">Response</span></span>
<span data-ttu-id="838a7-164">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="838a7-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="838a7-165">例</span><span class="sxs-lookup"><span data-stu-id="838a7-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="838a7-166">要求</span><span class="sxs-lookup"><span data-stu-id="838a7-166">Request</span></span>
<span data-ttu-id="838a7-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="838a7-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="838a7-168">応答</span><span class="sxs-lookup"><span data-stu-id="838a7-168">Response</span></span>
<span data-ttu-id="838a7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="838a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








