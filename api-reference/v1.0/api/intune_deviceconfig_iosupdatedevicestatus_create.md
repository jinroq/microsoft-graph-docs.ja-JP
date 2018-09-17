# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="9e855-101">iosUpdateDeviceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="9e855-101">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="9e855-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e855-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e855-103">新しい [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9e855-103">Create a new [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e855-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e855-104">Prerequisites</span></span>
<span data-ttu-id="9e855-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9e855-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e855-107">Permission type</span></span>|<span data-ttu-id="9e855-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e855-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e855-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e855-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9e855-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e855-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e855-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e855-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e855-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e855-112">Not supported.</span></span>|
|<span data-ttu-id="9e855-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e855-113">Application</span></span>|<span data-ttu-id="9e855-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e855-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e855-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e855-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9e855-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e855-116">Request headers</span></span>
|<span data-ttu-id="9e855-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e855-117">Header</span></span>|<span data-ttu-id="9e855-118">値</span><span class="sxs-lookup"><span data-stu-id="9e855-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e855-119">承認</span><span class="sxs-lookup"><span data-stu-id="9e855-119">Authorization</span></span>|<span data-ttu-id="9e855-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9e855-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e855-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="9e855-121">Accept</span></span>|<span data-ttu-id="9e855-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="9e855-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e855-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e855-123">Request body</span></span>
<span data-ttu-id="9e855-124">要求本文で、iosUpdateDeviceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e855-124">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="9e855-125">次の表に、iosUpdateDeviceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9e855-125">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="9e855-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e855-126">Property</span></span>|<span data-ttu-id="9e855-127">型</span><span class="sxs-lookup"><span data-stu-id="9e855-127">Type</span></span>|<span data-ttu-id="9e855-128">説明</span><span class="sxs-lookup"><span data-stu-id="9e855-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e855-129">ID</span><span class="sxs-lookup"><span data-stu-id="9e855-129">id</span></span>|<span data-ttu-id="9e855-130">文字列</span><span class="sxs-lookup"><span data-stu-id="9e855-130">String</span></span>|<span data-ttu-id="9e855-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9e855-131">Key of the entity.</span></span>|
|<span data-ttu-id="9e855-132">installStatus</span><span class="sxs-lookup"><span data-stu-id="9e855-132">installStatus</span></span>|[<span data-ttu-id="9e855-133">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9e855-133">iosUpdatesInstallStatus</span></span>](../resources/intune_deviceconfig_iosupdatesinstallstatus.md)|<span data-ttu-id="9e855-134">ポリシー レポートのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="9e855-134">The installation status of the policy report.</span></span> <span data-ttu-id="9e855-135">使用可能な値は `success`、 `available`、 `idle`、 `unknown`、 `downloading`、 `downloadFailed`、 `downloadRequiresComputer`、 `downloadInsufficientSpace`、 `downloadInsufficientPower`、 `downloadInsufficientNetwork`、 `installing`、 `installInsufficientSpace`、 `installInsufficientPower`、 `installPhoneCallInProgress`、 `installFailed`、 `notSupportedOperation`、 `sharedDeviceUserLoggedInError`です。</span><span class="sxs-lookup"><span data-stu-id="9e855-135">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`.</span></span>|
|<span data-ttu-id="9e855-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="9e855-136">osVersion</span></span>|<span data-ttu-id="9e855-137">文字列</span><span class="sxs-lookup"><span data-stu-id="9e855-137">String</span></span>|<span data-ttu-id="9e855-138">レポートされているデバイス バージョン。</span><span class="sxs-lookup"><span data-stu-id="9e855-138">The device version that is being reported.</span></span>|
|<span data-ttu-id="9e855-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="9e855-139">deviceId</span></span>|<span data-ttu-id="9e855-140">文字列</span><span class="sxs-lookup"><span data-stu-id="9e855-140">String</span></span>|<span data-ttu-id="9e855-141">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="9e855-141">The device id that is being reported.</span></span>|
|<span data-ttu-id="9e855-142">userId</span><span class="sxs-lookup"><span data-stu-id="9e855-142">userId</span></span>|<span data-ttu-id="9e855-143">文字列</span><span class="sxs-lookup"><span data-stu-id="9e855-143">String</span></span>|<span data-ttu-id="9e855-144">レポートされているユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="9e855-144">The User id that is being reported.</span></span>|
|<span data-ttu-id="9e855-145">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9e855-145">deviceDisplayName</span></span>|<span data-ttu-id="9e855-146">文字列</span><span class="sxs-lookup"><span data-stu-id="9e855-146">String</span></span>|<span data-ttu-id="9e855-147">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="9e855-147">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="9e855-148">userName</span><span class="sxs-lookup"><span data-stu-id="9e855-148">userName</span></span>|<span data-ttu-id="9e855-149">文字列</span><span class="sxs-lookup"><span data-stu-id="9e855-149">String</span></span>|<span data-ttu-id="9e855-150">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="9e855-150">The User Name that is being reported</span></span>|
|<span data-ttu-id="9e855-151">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9e855-151">deviceModel</span></span>|<span data-ttu-id="9e855-152">文字列</span><span class="sxs-lookup"><span data-stu-id="9e855-152">String</span></span>|<span data-ttu-id="9e855-153">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="9e855-153">The device model that is being reported</span></span>|
|<span data-ttu-id="9e855-154">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9e855-154">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9e855-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e855-155">DateTimeOffset</span></span>|<span data-ttu-id="9e855-156">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="9e855-156">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="9e855-157">状態</span><span class="sxs-lookup"><span data-stu-id="9e855-157">status</span></span>|[<span data-ttu-id="9e855-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9e855-158">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="9e855-159">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="9e855-159">Compliance status of the policy report.</span></span> <span data-ttu-id="9e855-160">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="9e855-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9e855-161">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e855-161">lastReportedDateTime</span></span>|<span data-ttu-id="9e855-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e855-162">DateTimeOffset</span></span>|<span data-ttu-id="9e855-163">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="9e855-163">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="9e855-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9e855-164">userPrincipalName</span></span>|<span data-ttu-id="9e855-165">文字列</span><span class="sxs-lookup"><span data-stu-id="9e855-165">String</span></span>|<span data-ttu-id="9e855-166">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="9e855-166">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="9e855-167">応答</span><span class="sxs-lookup"><span data-stu-id="9e855-167">Response</span></span>
<span data-ttu-id="9e855-168">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9e855-168">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e855-169">例</span><span class="sxs-lookup"><span data-stu-id="9e855-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e855-170">要求</span><span class="sxs-lookup"><span data-stu-id="9e855-170">Request</span></span>
<span data-ttu-id="9e855-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e855-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 552

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="9e855-172">応答</span><span class="sxs-lookup"><span data-stu-id="9e855-172">Response</span></span>
<span data-ttu-id="9e855-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e855-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 601

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```








