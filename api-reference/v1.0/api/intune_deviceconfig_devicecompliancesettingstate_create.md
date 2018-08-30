# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="3cf26-101">deviceComplianceSettingState の作成</span><span class="sxs-lookup"><span data-stu-id="3cf26-101">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="3cf26-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3cf26-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cf26-103">新しい [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3cf26-103">Create a new [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3cf26-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="3cf26-104">Prerequisites</span></span>
<span data-ttu-id="3cf26-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cf26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3cf26-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3cf26-107">Permission type</span></span>|<span data-ttu-id="3cf26-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3cf26-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cf26-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3cf26-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3cf26-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cf26-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3cf26-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3cf26-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cf26-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cf26-112">Not supported.</span></span>|
|<span data-ttu-id="3cf26-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3cf26-113">Application</span></span>|<span data-ttu-id="3cf26-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cf26-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cf26-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3cf26-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="3cf26-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cf26-116">Request headers</span></span>
|<span data-ttu-id="3cf26-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cf26-117">Header</span></span>|<span data-ttu-id="3cf26-118">値</span><span class="sxs-lookup"><span data-stu-id="3cf26-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cf26-119">承認</span><span class="sxs-lookup"><span data-stu-id="3cf26-119">Authorization</span></span>|<span data-ttu-id="3cf26-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3cf26-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cf26-121">承諾</span><span class="sxs-lookup"><span data-stu-id="3cf26-121">Accept</span></span>|<span data-ttu-id="3cf26-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3cf26-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cf26-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="3cf26-123">Request body</span></span>
<span data-ttu-id="3cf26-124">要求本文で、deviceComplianceSettingState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3cf26-124">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="3cf26-125">次の表に、deviceComplianceSettingState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3cf26-125">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="3cf26-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cf26-126">Property</span></span>|<span data-ttu-id="3cf26-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="3cf26-127">Type</span></span>|<span data-ttu-id="3cf26-128">説明</span><span class="sxs-lookup"><span data-stu-id="3cf26-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cf26-129">ID</span><span class="sxs-lookup"><span data-stu-id="3cf26-129">id</span></span>|<span data-ttu-id="3cf26-130">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf26-130">String</span></span>|<span data-ttu-id="3cf26-131">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="3cf26-131">Key of the entity</span></span>|
|<span data-ttu-id="3cf26-132">setting</span><span class="sxs-lookup"><span data-stu-id="3cf26-132">setting</span></span>|<span data-ttu-id="3cf26-133">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf26-133">String</span></span>|<span data-ttu-id="3cf26-134">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="3cf26-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="3cf26-135">settingName</span><span class="sxs-lookup"><span data-stu-id="3cf26-135">settingName</span></span>|<span data-ttu-id="3cf26-136">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf26-136">String</span></span>|<span data-ttu-id="3cf26-137">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="3cf26-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="3cf26-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="3cf26-138">deviceId</span></span>|<span data-ttu-id="3cf26-139">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf26-139">String</span></span>|<span data-ttu-id="3cf26-140">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="3cf26-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="3cf26-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="3cf26-141">deviceName</span></span>|<span data-ttu-id="3cf26-142">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf26-142">String</span></span>|<span data-ttu-id="3cf26-143">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="3cf26-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="3cf26-144">userId</span><span class="sxs-lookup"><span data-stu-id="3cf26-144">userId</span></span>|<span data-ttu-id="3cf26-145">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf26-145">String</span></span>|<span data-ttu-id="3cf26-146">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="3cf26-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="3cf26-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="3cf26-147">userEmail</span></span>|<span data-ttu-id="3cf26-148">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf26-148">String</span></span>|<span data-ttu-id="3cf26-149">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="3cf26-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="3cf26-150">userName</span><span class="sxs-lookup"><span data-stu-id="3cf26-150">userName</span></span>|<span data-ttu-id="3cf26-151">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf26-151">String</span></span>|<span data-ttu-id="3cf26-152">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="3cf26-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="3cf26-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3cf26-153">userPrincipalName</span></span>|<span data-ttu-id="3cf26-154">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf26-154">String</span></span>|<span data-ttu-id="3cf26-155">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="3cf26-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="3cf26-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="3cf26-156">deviceModel</span></span>|<span data-ttu-id="3cf26-157">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf26-157">String</span></span>|<span data-ttu-id="3cf26-158">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="3cf26-158">The device model that is being reported</span></span>|
|<span data-ttu-id="3cf26-159">状態</span><span class="sxs-lookup"><span data-stu-id="3cf26-159">state</span></span>|[<span data-ttu-id="3cf26-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3cf26-160">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="3cf26-161">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="3cf26-161">The compliance state of the setting Possible values are: , , , , , , .</span></span> <span data-ttu-id="3cf26-162">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="3cf26-162">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="3cf26-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3cf26-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3cf26-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cf26-164">DateTimeOffset</span></span>|<span data-ttu-id="3cf26-165">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="3cf26-165">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="3cf26-166">応答</span><span class="sxs-lookup"><span data-stu-id="3cf26-166">Response</span></span>
<span data-ttu-id="3cf26-167">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3cf26-167">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cf26-168">例</span><span class="sxs-lookup"><span data-stu-id="3cf26-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cf26-169">要求</span><span class="sxs-lookup"><span data-stu-id="3cf26-169">Request</span></span>
<span data-ttu-id="3cf26-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3cf26-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3cf26-171">応答</span><span class="sxs-lookup"><span data-stu-id="3cf26-171">Response</span></span>
<span data-ttu-id="3cf26-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3cf26-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



