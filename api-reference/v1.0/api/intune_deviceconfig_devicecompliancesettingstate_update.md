# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="2eab0-101">deviceComplianceSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="2eab0-101">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="2eab0-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2eab0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2eab0-103">[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2eab0-103">Update the properties of a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2eab0-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2eab0-104">Prerequisites</span></span>
<span data-ttu-id="2eab0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2eab0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2eab0-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2eab0-107">Permission type</span></span>|<span data-ttu-id="2eab0-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2eab0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eab0-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2eab0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2eab0-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eab0-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2eab0-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2eab0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eab0-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2eab0-112">Not supported.</span></span>|
|<span data-ttu-id="2eab0-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2eab0-113">Application</span></span>|<span data-ttu-id="2eab0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2eab0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eab0-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2eab0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="2eab0-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2eab0-116">Request headers</span></span>
|<span data-ttu-id="2eab0-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2eab0-117">Header</span></span>|<span data-ttu-id="2eab0-118">値</span><span class="sxs-lookup"><span data-stu-id="2eab0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eab0-119">承認</span><span class="sxs-lookup"><span data-stu-id="2eab0-119">Authorization</span></span>|<span data-ttu-id="2eab0-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2eab0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eab0-121">承諾</span><span class="sxs-lookup"><span data-stu-id="2eab0-121">Accept</span></span>|<span data-ttu-id="2eab0-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="2eab0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eab0-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2eab0-123">Request body</span></span>
<span data-ttu-id="2eab0-124">要求本文で、[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2eab0-124">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="2eab0-125">次の表に、[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2eab0-125">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="2eab0-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2eab0-126">Property</span></span>|<span data-ttu-id="2eab0-127">型</span><span class="sxs-lookup"><span data-stu-id="2eab0-127">Type</span></span>|<span data-ttu-id="2eab0-128">説明</span><span class="sxs-lookup"><span data-stu-id="2eab0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2eab0-129">ID</span><span class="sxs-lookup"><span data-stu-id="2eab0-129">id</span></span>|<span data-ttu-id="2eab0-130">文字列</span><span class="sxs-lookup"><span data-stu-id="2eab0-130">String</span></span>|<span data-ttu-id="2eab0-131">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="2eab0-131">Key of the entity</span></span>|
|<span data-ttu-id="2eab0-132">setting</span><span class="sxs-lookup"><span data-stu-id="2eab0-132">setting</span></span>|<span data-ttu-id="2eab0-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2eab0-133">String</span></span>|<span data-ttu-id="2eab0-134">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="2eab0-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="2eab0-135">settingName</span><span class="sxs-lookup"><span data-stu-id="2eab0-135">settingName</span></span>|<span data-ttu-id="2eab0-136">文字列</span><span class="sxs-lookup"><span data-stu-id="2eab0-136">String</span></span>|<span data-ttu-id="2eab0-137">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="2eab0-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="2eab0-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="2eab0-138">deviceId</span></span>|<span data-ttu-id="2eab0-139">文字列</span><span class="sxs-lookup"><span data-stu-id="2eab0-139">String</span></span>|<span data-ttu-id="2eab0-140">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="2eab0-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="2eab0-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="2eab0-141">deviceName</span></span>|<span data-ttu-id="2eab0-142">文字列</span><span class="sxs-lookup"><span data-stu-id="2eab0-142">String</span></span>|<span data-ttu-id="2eab0-143">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="2eab0-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="2eab0-144">userId</span><span class="sxs-lookup"><span data-stu-id="2eab0-144">userId</span></span>|<span data-ttu-id="2eab0-145">文字列</span><span class="sxs-lookup"><span data-stu-id="2eab0-145">String</span></span>|<span data-ttu-id="2eab0-146">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="2eab0-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="2eab0-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="2eab0-147">userEmail</span></span>|<span data-ttu-id="2eab0-148">文字列</span><span class="sxs-lookup"><span data-stu-id="2eab0-148">String</span></span>|<span data-ttu-id="2eab0-149">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="2eab0-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="2eab0-150">userName</span><span class="sxs-lookup"><span data-stu-id="2eab0-150">userName</span></span>|<span data-ttu-id="2eab0-151">文字列</span><span class="sxs-lookup"><span data-stu-id="2eab0-151">String</span></span>|<span data-ttu-id="2eab0-152">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="2eab0-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="2eab0-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2eab0-153">userPrincipalName</span></span>|<span data-ttu-id="2eab0-154">文字列</span><span class="sxs-lookup"><span data-stu-id="2eab0-154">String</span></span>|<span data-ttu-id="2eab0-155">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="2eab0-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="2eab0-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2eab0-156">deviceModel</span></span>|<span data-ttu-id="2eab0-157">文字列</span><span class="sxs-lookup"><span data-stu-id="2eab0-157">String</span></span>|<span data-ttu-id="2eab0-158">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="2eab0-158">The device model that is being reported</span></span>|
|<span data-ttu-id="2eab0-159">state</span><span class="sxs-lookup"><span data-stu-id="2eab0-159">state</span></span>|[<span data-ttu-id="2eab0-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2eab0-160">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="2eab0-161">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="2eab0-161">The compliance state of the setting Possible values are: , , , , , , .</span></span> <span data-ttu-id="2eab0-162">使用可能な値は`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="2eab0-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2eab0-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2eab0-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2eab0-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eab0-164">DateTimeOffset</span></span>|<span data-ttu-id="2eab0-165">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="2eab0-165">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="2eab0-166">応答</span><span class="sxs-lookup"><span data-stu-id="2eab0-166">Response</span></span>
<span data-ttu-id="2eab0-167">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="2eab0-167">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eab0-168">例</span><span class="sxs-lookup"><span data-stu-id="2eab0-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="2eab0-169">要求</span><span class="sxs-lookup"><span data-stu-id="2eab0-169">Request</span></span>
<span data-ttu-id="2eab0-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2eab0-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 450

{
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```

### <a name="response"></a><span data-ttu-id="2eab0-171">応答</span><span class="sxs-lookup"><span data-stu-id="2eab0-171">Response</span></span>
<span data-ttu-id="2eab0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2eab0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```








