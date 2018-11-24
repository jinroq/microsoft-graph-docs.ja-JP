# <a name="update-devicemanagementpartner"></a><span data-ttu-id="fb0e9-101">deviceManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="fb0e9-101">Update deviceManagementPartner</span></span>

> <span data-ttu-id="fb0e9-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb0e9-103">[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-103">Update the properties of a [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb0e9-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="fb0e9-104">Prerequisites</span></span>
<span data-ttu-id="fb0e9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb0e9-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb0e9-107">Permission type</span></span>|<span data-ttu-id="fb0e9-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb0e9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb0e9-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb0e9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fb0e9-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb0e9-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fb0e9-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb0e9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb0e9-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-112">Not supported.</span></span>|
|<span data-ttu-id="fb0e9-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb0e9-113">Application</span></span>|<span data-ttu-id="fb0e9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb0e9-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb0e9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="fb0e9-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb0e9-116">Request headers</span></span>
|<span data-ttu-id="fb0e9-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb0e9-117">Header</span></span>|<span data-ttu-id="fb0e9-118">値</span><span class="sxs-lookup"><span data-stu-id="fb0e9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb0e9-119">承認</span><span class="sxs-lookup"><span data-stu-id="fb0e9-119">Authorization</span></span>|<span data-ttu-id="fb0e9-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb0e9-121">承諾</span><span class="sxs-lookup"><span data-stu-id="fb0e9-121">Accept</span></span>|<span data-ttu-id="fb0e9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fb0e9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb0e9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb0e9-123">Request body</span></span>
<span data-ttu-id="fb0e9-124">要求本文で、[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-124">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="fb0e9-125">次の表に、[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-125">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span></span>

|<span data-ttu-id="fb0e9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb0e9-126">Property</span></span>|<span data-ttu-id="fb0e9-127">型</span><span class="sxs-lookup"><span data-stu-id="fb0e9-127">Type</span></span>|<span data-ttu-id="fb0e9-128">説明</span><span class="sxs-lookup"><span data-stu-id="fb0e9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb0e9-129">id</span><span class="sxs-lookup"><span data-stu-id="fb0e9-129">id</span></span>|<span data-ttu-id="fb0e9-130">String</span><span class="sxs-lookup"><span data-stu-id="fb0e9-130">String</span></span>|<span data-ttu-id="fb0e9-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fb0e9-131">Not yet documented</span></span>|
|<span data-ttu-id="fb0e9-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="fb0e9-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="fb0e9-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb0e9-133">DateTimeOffset</span></span>|<span data-ttu-id="fb0e9-134">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="fb0e9-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="fb0e9-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="fb0e9-135">partnerState</span></span>|[<span data-ttu-id="fb0e9-136">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="fb0e9-136">deviceManagementPartnerTenantState</span></span>](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|<span data-ttu-id="fb0e9-137">このテナントのパートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-137">Partner state of this tenant.</span></span> <span data-ttu-id="fb0e9-138">使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-138">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="fb0e9-139">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="fb0e9-139">partnerAppType</span></span>|[<span data-ttu-id="fb0e9-140">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="fb0e9-140">deviceManagementPartnerAppType</span></span>](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|<span data-ttu-id="fb0e9-141">パートナー ・ アプリケーションの種類です。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-141">Partner App type.</span></span> <span data-ttu-id="fb0e9-142">可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-142">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="fb0e9-143">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="fb0e9-143">singleTenantAppId</span></span>|<span data-ttu-id="fb0e9-144">String</span><span class="sxs-lookup"><span data-stu-id="fb0e9-144">String</span></span>|<span data-ttu-id="fb0e9-145">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="fb0e9-145">Partner Single tenant App id</span></span>|
|<span data-ttu-id="fb0e9-146">displayName</span><span class="sxs-lookup"><span data-stu-id="fb0e9-146">displayName</span></span>|<span data-ttu-id="fb0e9-147">String</span><span class="sxs-lookup"><span data-stu-id="fb0e9-147">String</span></span>|<span data-ttu-id="fb0e9-148">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="fb0e9-148">Partner display name</span></span>|
|<span data-ttu-id="fb0e9-149">isConfigured</span><span class="sxs-lookup"><span data-stu-id="fb0e9-149">isConfigured</span></span>|<span data-ttu-id="fb0e9-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb0e9-150">Boolean</span></span>|<span data-ttu-id="fb0e9-151">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="fb0e9-151">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="fb0e9-152">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb0e9-152">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="fb0e9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb0e9-153">DateTimeOffset</span></span>|<span data-ttu-id="fb0e9-154">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="fb0e9-154">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="fb0e9-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="fb0e9-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="fb0e9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb0e9-156">DateTimeOffset</span></span>|<span data-ttu-id="fb0e9-157">パートナー デバイスが準拠していないとマークされる日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="fb0e9-157">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="fb0e9-158">応答</span><span class="sxs-lookup"><span data-stu-id="fb0e9-158">Response</span></span>
<span data-ttu-id="fb0e9-159">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-159">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb0e9-160">例</span><span class="sxs-lookup"><span data-stu-id="fb0e9-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb0e9-161">要求</span><span class="sxs-lookup"><span data-stu-id="fb0e9-161">Request</span></span>
<span data-ttu-id="fb0e9-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
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

### <a name="response"></a><span data-ttu-id="fb0e9-163">応答</span><span class="sxs-lookup"><span data-stu-id="fb0e9-163">Response</span></span>
<span data-ttu-id="fb0e9-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fb0e9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



