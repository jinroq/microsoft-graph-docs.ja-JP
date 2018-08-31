# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="ed949-101">ManagedDeviceMobileAppConfigurationDeviceStatus を作成する</span><span class="sxs-lookup"><span data-stu-id="ed949-101">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="ed949-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed949-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed949-103">新しい [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ed949-103">Create a new [deviceCompliancePolicyAssignment](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed949-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ed949-104">Prerequisites</span></span>
<span data-ttu-id="ed949-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ed949-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed949-107">Permission type</span></span>|<span data-ttu-id="ed949-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed949-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed949-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed949-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ed949-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed949-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed949-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed949-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed949-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed949-112">Not supported.</span></span>|
|<span data-ttu-id="ed949-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed949-113">Application</span></span>|<span data-ttu-id="ed949-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed949-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed949-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed949-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ed949-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed949-116">Request headers</span></span>
|<span data-ttu-id="ed949-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed949-117">Header</span></span>|<span data-ttu-id="ed949-118">値</span><span class="sxs-lookup"><span data-stu-id="ed949-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed949-119">承認</span><span class="sxs-lookup"><span data-stu-id="ed949-119">Authorization</span></span>|<span data-ttu-id="ed949-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ed949-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed949-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ed949-121">Accept</span></span>|<span data-ttu-id="ed949-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="ed949-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed949-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed949-123">Request body</span></span>
<span data-ttu-id="ed949-124">要求本文で、windows10GeneralConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed949-124">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="ed949-125">次の表に、managedDeviceMobileAppConfigurationDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ed949-125">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="ed949-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed949-126">Property</span></span>|<span data-ttu-id="ed949-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="ed949-127">Type</span></span>|<span data-ttu-id="ed949-128">説明</span><span class="sxs-lookup"><span data-stu-id="ed949-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed949-129">ID</span><span class="sxs-lookup"><span data-stu-id="ed949-129">id</span></span>|<span data-ttu-id="ed949-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ed949-130">String</span></span>|<span data-ttu-id="ed949-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ed949-131">Key of the entity.</span></span>|
|<span data-ttu-id="ed949-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed949-132">deviceDisplayName</span></span>|<span data-ttu-id="ed949-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ed949-133">String</span></span>|<span data-ttu-id="ed949-134">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="ed949-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ed949-135">userName</span><span class="sxs-lookup"><span data-stu-id="ed949-135">userName</span></span>|<span data-ttu-id="ed949-136">文字列</span><span class="sxs-lookup"><span data-stu-id="ed949-136">String</span></span>|<span data-ttu-id="ed949-137">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="ed949-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="ed949-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ed949-138">deviceModel</span></span>|<span data-ttu-id="ed949-139">文字列</span><span class="sxs-lookup"><span data-stu-id="ed949-139">String</span></span>|<span data-ttu-id="ed949-140">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="ed949-140">The device model that is being reported</span></span>|
|<span data-ttu-id="ed949-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ed949-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ed949-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed949-142">DateTimeOffset</span></span>|<span data-ttu-id="ed949-143">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="ed949-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ed949-144">状態</span><span class="sxs-lookup"><span data-stu-id="ed949-144">status</span></span>|[<span data-ttu-id="ed949-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ed949-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="ed949-146">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="ed949-146">Compliance status of the policy report.</span></span> <span data-ttu-id="ed949-147">指定できる値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="ed949-147">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="ed949-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed949-148">lastReportedDateTime</span></span>|<span data-ttu-id="ed949-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed949-149">DateTimeOffset</span></span>|<span data-ttu-id="ed949-150">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="ed949-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ed949-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed949-151">userPrincipalName</span></span>|<span data-ttu-id="ed949-152">文字列</span><span class="sxs-lookup"><span data-stu-id="ed949-152">String</span></span>|<span data-ttu-id="ed949-153">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="ed949-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ed949-154">応答</span><span class="sxs-lookup"><span data-stu-id="ed949-154">Response</span></span>
<span data-ttu-id="ed949-155">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ed949-155">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed949-156">例</span><span class="sxs-lookup"><span data-stu-id="ed949-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed949-157">要求</span><span class="sxs-lookup"><span data-stu-id="ed949-157">Request</span></span>
<span data-ttu-id="ed949-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed949-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="ed949-159">応答</span><span class="sxs-lookup"><span data-stu-id="ed949-159">Response</span></span>
<span data-ttu-id="ed949-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed949-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



