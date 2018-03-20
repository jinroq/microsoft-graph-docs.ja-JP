# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="119e6-101">deviceConfigurationDeviceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="119e6-101">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="119e6-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="119e6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="119e6-103">[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="119e6-103">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="119e6-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="119e6-104">Prerequisites</span></span>
<span data-ttu-id="119e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="119e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="119e6-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="119e6-107">Permission type</span></span>|<span data-ttu-id="119e6-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="119e6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="119e6-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="119e6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="119e6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="119e6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="119e6-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="119e6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="119e6-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="119e6-112">Not supported.</span></span>|
|<span data-ttu-id="119e6-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="119e6-113">Application</span></span>|<span data-ttu-id="119e6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="119e6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="119e6-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="119e6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="119e6-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="119e6-116">Request headers</span></span>
|<span data-ttu-id="119e6-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="119e6-117">Header</span></span>|<span data-ttu-id="119e6-118">値</span><span class="sxs-lookup"><span data-stu-id="119e6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="119e6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="119e6-119">Authorization</span></span>|<span data-ttu-id="119e6-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="119e6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="119e6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="119e6-121">Accept</span></span>|<span data-ttu-id="119e6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="119e6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="119e6-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="119e6-123">Request body</span></span>
<span data-ttu-id="119e6-124">要求本文で、[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="119e6-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="119e6-125">次の表に、[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="119e6-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="119e6-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="119e6-126">Property</span></span>|<span data-ttu-id="119e6-127">型</span><span class="sxs-lookup"><span data-stu-id="119e6-127">Type</span></span>|<span data-ttu-id="119e6-128">説明</span><span class="sxs-lookup"><span data-stu-id="119e6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="119e6-129">id</span><span class="sxs-lookup"><span data-stu-id="119e6-129">id</span></span>|<span data-ttu-id="119e6-130">String</span><span class="sxs-lookup"><span data-stu-id="119e6-130">String</span></span>|<span data-ttu-id="119e6-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="119e6-131">Name of the entity.</span></span>|
|<span data-ttu-id="119e6-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="119e6-132">deviceDisplayName</span></span>|<span data-ttu-id="119e6-133">String</span><span class="sxs-lookup"><span data-stu-id="119e6-133">String</span></span>|<span data-ttu-id="119e6-134">DevicePolicyStatus のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="119e6-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="119e6-135">userName</span><span class="sxs-lookup"><span data-stu-id="119e6-135">Username</span></span>|<span data-ttu-id="119e6-136">String</span><span class="sxs-lookup"><span data-stu-id="119e6-136">String</span></span>|<span data-ttu-id="119e6-137">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="119e6-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="119e6-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="119e6-138">deviceModel</span></span>|<span data-ttu-id="119e6-139">String</span><span class="sxs-lookup"><span data-stu-id="119e6-139">String</span></span>|<span data-ttu-id="119e6-140">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="119e6-140">The device model that is being reported</span></span>|
|<span data-ttu-id="119e6-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="119e6-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="119e6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="119e6-142">DateTimeOffset</span></span>|<span data-ttu-id="119e6-143">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="119e6-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="119e6-144">status</span><span class="sxs-lookup"><span data-stu-id="119e6-144">status</span></span>|<span data-ttu-id="119e6-145">String</span><span class="sxs-lookup"><span data-stu-id="119e6-145">String</span></span>|<span data-ttu-id="119e6-146">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="119e6-146">Compliance status of the policy report.</span></span> <span data-ttu-id="119e6-147">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="119e6-147">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="119e6-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="119e6-148">lastReportedDateTime</span></span>|<span data-ttu-id="119e6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="119e6-149">DateTimeOffset</span></span>|<span data-ttu-id="119e6-150">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="119e6-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="119e6-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="119e6-151">userPrincipalName</span></span>|<span data-ttu-id="119e6-152">String</span><span class="sxs-lookup"><span data-stu-id="119e6-152">String</span></span>|<span data-ttu-id="119e6-153">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="119e6-153">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="119e6-154">応答</span><span class="sxs-lookup"><span data-stu-id="119e6-154">Response</span></span>
<span data-ttu-id="119e6-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="119e6-155">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="119e6-156">例</span><span class="sxs-lookup"><span data-stu-id="119e6-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="119e6-157">要求</span><span class="sxs-lookup"><span data-stu-id="119e6-157">Request</span></span>
<span data-ttu-id="119e6-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="119e6-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 359

{
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="119e6-159">応答</span><span class="sxs-lookup"><span data-stu-id="119e6-159">Response</span></span>
<span data-ttu-id="119e6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="119e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



