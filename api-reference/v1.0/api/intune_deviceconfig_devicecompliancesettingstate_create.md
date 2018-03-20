# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="1c573-101">deviceComplianceSettingState の作成</span><span class="sxs-lookup"><span data-stu-id="1c573-101">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="1c573-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c573-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c573-103">新しい [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1c573-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c573-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="1c573-104">Prerequisites</span></span>
<span data-ttu-id="1c573-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c573-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c573-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c573-107">Permission type</span></span>|<span data-ttu-id="1c573-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c573-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c573-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c573-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1c573-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c573-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c573-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c573-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c573-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c573-112">Not supported.</span></span>|
|<span data-ttu-id="1c573-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c573-113">Application</span></span>|<span data-ttu-id="1c573-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c573-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c573-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c573-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="1c573-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c573-116">Request headers</span></span>
|<span data-ttu-id="1c573-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c573-117">Header</span></span>|<span data-ttu-id="1c573-118">値</span><span class="sxs-lookup"><span data-stu-id="1c573-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c573-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c573-119">Authorization</span></span>|<span data-ttu-id="1c573-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1c573-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1c573-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1c573-121">Accept</span></span>|<span data-ttu-id="1c573-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1c573-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c573-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c573-123">Request body</span></span>
<span data-ttu-id="1c573-124">要求本文で、deviceComplianceSettingState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1c573-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="1c573-125">次の表に、deviceComplianceSettingState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1c573-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="1c573-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c573-126">Property</span></span>|<span data-ttu-id="1c573-127">型</span><span class="sxs-lookup"><span data-stu-id="1c573-127">Type</span></span>|<span data-ttu-id="1c573-128">説明</span><span class="sxs-lookup"><span data-stu-id="1c573-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c573-129">id</span><span class="sxs-lookup"><span data-stu-id="1c573-129">id</span></span>|<span data-ttu-id="1c573-130">String</span><span class="sxs-lookup"><span data-stu-id="1c573-130">String</span></span>|<span data-ttu-id="1c573-131">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="1c573-131">Name of the entity.</span></span>|
|<span data-ttu-id="1c573-132">setting</span><span class="sxs-lookup"><span data-stu-id="1c573-132">setting</span></span>|<span data-ttu-id="1c573-133">String</span><span class="sxs-lookup"><span data-stu-id="1c573-133">String</span></span>|<span data-ttu-id="1c573-134">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="1c573-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="1c573-135">settingName</span><span class="sxs-lookup"><span data-stu-id="1c573-135">settingName</span></span>|<span data-ttu-id="1c573-136">String</span><span class="sxs-lookup"><span data-stu-id="1c573-136">String</span></span>|<span data-ttu-id="1c573-137">レポートされている設定名</span><span class="sxs-lookup"><span data-stu-id="1c573-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="1c573-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="1c573-138">deviceId</span></span>|<span data-ttu-id="1c573-139">String</span><span class="sxs-lookup"><span data-stu-id="1c573-139">String</span></span>|<span data-ttu-id="1c573-140">レポートされているデバイス ID</span><span class="sxs-lookup"><span data-stu-id="1c573-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="1c573-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="1c573-141">DeviceName</span></span>|<span data-ttu-id="1c573-142">String</span><span class="sxs-lookup"><span data-stu-id="1c573-142">String</span></span>|<span data-ttu-id="1c573-143">レポートされているデバイス名</span><span class="sxs-lookup"><span data-stu-id="1c573-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="1c573-144">userId</span><span class="sxs-lookup"><span data-stu-id="1c573-144">userId</span></span>|<span data-ttu-id="1c573-145">String</span><span class="sxs-lookup"><span data-stu-id="1c573-145">String</span></span>|<span data-ttu-id="1c573-146">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="1c573-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="1c573-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="1c573-147">?user_email=...</span></span>|<span data-ttu-id="1c573-148">String</span><span class="sxs-lookup"><span data-stu-id="1c573-148">String</span></span>|<span data-ttu-id="1c573-149">レポートされているユーザーのメール アドレス</span><span class="sxs-lookup"><span data-stu-id="1c573-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="1c573-150">userName</span><span class="sxs-lookup"><span data-stu-id="1c573-150">Username</span></span>|<span data-ttu-id="1c573-151">String</span><span class="sxs-lookup"><span data-stu-id="1c573-151">String</span></span>|<span data-ttu-id="1c573-152">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="1c573-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="1c573-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1c573-153">userPrincipalName</span></span>|<span data-ttu-id="1c573-154">String</span><span class="sxs-lookup"><span data-stu-id="1c573-154">String</span></span>|<span data-ttu-id="1c573-155">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="1c573-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="1c573-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1c573-156">deviceModel</span></span>|<span data-ttu-id="1c573-157">String</span><span class="sxs-lookup"><span data-stu-id="1c573-157">String</span></span>|<span data-ttu-id="1c573-158">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="1c573-158">The device model that is being reported</span></span>|
|<span data-ttu-id="1c573-159">state</span><span class="sxs-lookup"><span data-stu-id="1c573-159">state</span></span>|<span data-ttu-id="1c573-160">String</span><span class="sxs-lookup"><span data-stu-id="1c573-160">String</span></span>|<span data-ttu-id="1c573-161">設定のコンプライアンス対応状態。可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="1c573-161">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="1c573-162">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1c573-162">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1c573-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c573-163">DateTimeOffset</span></span>|<span data-ttu-id="1c573-164">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="1c573-164">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="1c573-165">応答</span><span class="sxs-lookup"><span data-stu-id="1c573-165">Response</span></span>
<span data-ttu-id="1c573-166">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1c573-166">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c573-167">例</span><span class="sxs-lookup"><span data-stu-id="1c573-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c573-168">要求</span><span class="sxs-lookup"><span data-stu-id="1c573-168">Request</span></span>
<span data-ttu-id="1c573-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1c573-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
Content-type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="1c573-170">応答</span><span class="sxs-lookup"><span data-stu-id="1c573-170">Response</span></span>
<span data-ttu-id="1c573-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1c573-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



