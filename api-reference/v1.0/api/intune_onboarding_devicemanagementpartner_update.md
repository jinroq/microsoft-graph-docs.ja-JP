# <a name="update-devicemanagementpartner"></a><span data-ttu-id="47076-101">deviceManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="47076-101">Update deviceManagementPartner</span></span>

> <span data-ttu-id="47076-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="47076-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47076-103">[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="47076-103">Update the properties of a [calendar](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47076-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="47076-104">Prerequisites</span></span>
<span data-ttu-id="47076-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47076-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="47076-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="47076-107">Permission type</span></span>|<span data-ttu-id="47076-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="47076-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47076-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="47076-109">Delegated (work or school account)</span></span>|<span data-ttu-id="47076-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47076-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="47076-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="47076-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47076-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47076-112">Not supported.</span></span>|
|<span data-ttu-id="47076-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="47076-113">Application</span></span>|<span data-ttu-id="47076-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47076-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47076-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="47076-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="47076-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47076-116">Request headers</span></span>
|<span data-ttu-id="47076-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47076-117">Header</span></span>|<span data-ttu-id="47076-118">値</span><span class="sxs-lookup"><span data-stu-id="47076-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47076-119">承認</span><span class="sxs-lookup"><span data-stu-id="47076-119">Authorization</span></span>|<span data-ttu-id="47076-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="47076-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="47076-121">承諾</span><span class="sxs-lookup"><span data-stu-id="47076-121">Accept</span></span>|<span data-ttu-id="47076-122">application/json</span><span class="sxs-lookup"><span data-stu-id="47076-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47076-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="47076-123">Request body</span></span>
<span data-ttu-id="47076-124">要求本文で、[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="47076-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="47076-125">次の表に、[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="47076-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="47076-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47076-126">Property</span></span>|<span data-ttu-id="47076-127">型</span><span class="sxs-lookup"><span data-stu-id="47076-127">Type</span></span>|<span data-ttu-id="47076-128">説明</span><span class="sxs-lookup"><span data-stu-id="47076-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47076-129">id</span><span class="sxs-lookup"><span data-stu-id="47076-129">id</span></span>|<span data-ttu-id="47076-130">String</span><span class="sxs-lookup"><span data-stu-id="47076-130">String</span></span>|<span data-ttu-id="47076-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="47076-131">Not yet documented</span></span>|
|<span data-ttu-id="47076-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="47076-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="47076-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47076-133">DateTimeOffset</span></span>|<span data-ttu-id="47076-134">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="47076-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="47076-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="47076-135">partnerState</span></span>|<span data-ttu-id="47076-136">String</span><span class="sxs-lookup"><span data-stu-id="47076-136">String</span></span>|<span data-ttu-id="47076-137">このテナントのパートナーの状態。可能な値は、`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="47076-137">Partner state of this tenant Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="47076-138">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="47076-138">partnerAppType</span></span>|<span data-ttu-id="47076-139">String</span><span class="sxs-lookup"><span data-stu-id="47076-139">String</span></span>|<span data-ttu-id="47076-140">パートナー アプリの種類。可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="47076-140">Partner App type Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="47076-141">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="47076-141">singleTenantAppId</span></span>|<span data-ttu-id="47076-142">String</span><span class="sxs-lookup"><span data-stu-id="47076-142">String</span></span>|<span data-ttu-id="47076-143">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="47076-143">Partner Single tenant App id</span></span>|
|<span data-ttu-id="47076-144">displayName</span><span class="sxs-lookup"><span data-stu-id="47076-144">displayName</span></span>|<span data-ttu-id="47076-145">String</span><span class="sxs-lookup"><span data-stu-id="47076-145">String</span></span>|<span data-ttu-id="47076-146">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="47076-146">Partner display name</span></span>|
|<span data-ttu-id="47076-147">isConfigured</span><span class="sxs-lookup"><span data-stu-id="47076-147">isConfigured</span></span>|<span data-ttu-id="47076-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="47076-148">Boolean</span></span>|<span data-ttu-id="47076-149">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="47076-149">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="47076-150">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="47076-150">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="47076-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47076-151">DateTimeOffset</span></span>|<span data-ttu-id="47076-152">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="47076-152">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="47076-153">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="47076-153">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="47076-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47076-154">DateTimeOffset</span></span>|<span data-ttu-id="47076-155">パートナー デバイスが準拠していないとマークされる日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="47076-155">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="47076-156">応答</span><span class="sxs-lookup"><span data-stu-id="47076-156">Response</span></span>
<span data-ttu-id="47076-157">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="47076-157">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47076-158">例</span><span class="sxs-lookup"><span data-stu-id="47076-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="47076-159">要求</span><span class="sxs-lookup"><span data-stu-id="47076-159">Request</span></span>
<span data-ttu-id="47076-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="47076-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 440

{
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="47076-161">応答</span><span class="sxs-lookup"><span data-stu-id="47076-161">Response</span></span>
<span data-ttu-id="47076-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="47076-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```



