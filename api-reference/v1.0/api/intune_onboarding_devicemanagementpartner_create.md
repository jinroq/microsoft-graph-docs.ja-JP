# <a name="create-devicemanagementpartner"></a><span data-ttu-id="3c26d-101">deviceManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="3c26d-101">Create deviceManagementPartner</span></span>

> <span data-ttu-id="3c26d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c26d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c26d-103">新しい [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3c26d-103">Create a new [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c26d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="3c26d-104">Prerequisites</span></span>
<span data-ttu-id="3c26d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c26d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3c26d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c26d-107">Permission type</span></span>|<span data-ttu-id="3c26d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c26d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c26d-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c26d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3c26d-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c26d-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3c26d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c26d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c26d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c26d-112">Not supported.</span></span>|
|<span data-ttu-id="3c26d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c26d-113">Application</span></span>|<span data-ttu-id="3c26d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c26d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c26d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c26d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="3c26d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c26d-116">Request headers</span></span>
|<span data-ttu-id="3c26d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c26d-117">Header</span></span>|<span data-ttu-id="3c26d-118">値</span><span class="sxs-lookup"><span data-stu-id="3c26d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c26d-119">承認</span><span class="sxs-lookup"><span data-stu-id="3c26d-119">Authorization</span></span>|<span data-ttu-id="3c26d-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3c26d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c26d-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="3c26d-121">Accept</span></span>|<span data-ttu-id="3c26d-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="3c26d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c26d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c26d-123">Request body</span></span>
<span data-ttu-id="3c26d-124">要求本文で、deviceManagementPartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c26d-124">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="3c26d-125">次の表に、deviceManagementPartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3c26d-125">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="3c26d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c26d-126">Property</span></span>|<span data-ttu-id="3c26d-127">型</span><span class="sxs-lookup"><span data-stu-id="3c26d-127">Type</span></span>|<span data-ttu-id="3c26d-128">説明</span><span class="sxs-lookup"><span data-stu-id="3c26d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c26d-129">ID</span><span class="sxs-lookup"><span data-stu-id="3c26d-129">id</span></span>|<span data-ttu-id="3c26d-130">文字列</span><span class="sxs-lookup"><span data-stu-id="3c26d-130">String</span></span>|<span data-ttu-id="3c26d-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c26d-131">Not yet documented</span></span>|
|<span data-ttu-id="3c26d-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="3c26d-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="3c26d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c26d-133">DateTimeOffset</span></span>|<span data-ttu-id="3c26d-134">管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="3c26d-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="3c26d-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="3c26d-135">partnerState</span></span>|[<span data-ttu-id="3c26d-136">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="3c26d-136">deviceManagementPartnerTenantState</span></span>](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|<span data-ttu-id="3c26d-137">このテナントのパートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="3c26d-137">Partner state of this tenant Possible values are: , , , .</span></span> <span data-ttu-id="3c26d-138">使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="3c26d-138">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="3c26d-139">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="3c26d-139">partnerAppType</span></span>|[<span data-ttu-id="3c26d-140">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="3c26d-140">deviceManagementPartnerAppType</span></span>](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|<span data-ttu-id="3c26d-141">パートナー アプリの種類。</span><span class="sxs-lookup"><span data-stu-id="3c26d-141">Partner App Type.</span></span> <span data-ttu-id="3c26d-142">可能な値は、`unknown`、`singleTenantApp`、`multiTenantApp` です。</span><span class="sxs-lookup"><span data-stu-id="3c26d-142">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="3c26d-143">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="3c26d-143">singleTenantAppId</span></span>|<span data-ttu-id="3c26d-144">文字列</span><span class="sxs-lookup"><span data-stu-id="3c26d-144">String</span></span>|<span data-ttu-id="3c26d-145">パートナーのシングル テナントのアプリ ID</span><span class="sxs-lookup"><span data-stu-id="3c26d-145">Partner Single tenant App id</span></span>|
|<span data-ttu-id="3c26d-146">displayName</span><span class="sxs-lookup"><span data-stu-id="3c26d-146">displayName</span></span>|<span data-ttu-id="3c26d-147">文字列</span><span class="sxs-lookup"><span data-stu-id="3c26d-147">String</span></span>|<span data-ttu-id="3c26d-148">パートナー表示名</span><span class="sxs-lookup"><span data-stu-id="3c26d-148">Partner display name</span></span>|
|<span data-ttu-id="3c26d-149">isConfigured</span><span class="sxs-lookup"><span data-stu-id="3c26d-149">isConfigured</span></span>|<span data-ttu-id="3c26d-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="3c26d-150">Boolean</span></span>|<span data-ttu-id="3c26d-151">デバイス管理パートナーが構成されているかどうかを指定します</span><span class="sxs-lookup"><span data-stu-id="3c26d-151">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="3c26d-152">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c26d-152">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="3c26d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c26d-153">DateTimeOffset</span></span>|<span data-ttu-id="3c26d-154">パートナー デバイスが削除されるときの日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="3c26d-154">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="3c26d-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="3c26d-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="3c26d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c26d-156">DateTimeOffset</span></span>|<span data-ttu-id="3c26d-157">パートナー デバイスが準拠していないとマークされる日時 (UTC)</span><span class="sxs-lookup"><span data-stu-id="3c26d-157">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="3c26d-158">応答</span><span class="sxs-lookup"><span data-stu-id="3c26d-158">Response</span></span>
<span data-ttu-id="3c26d-159">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3c26d-159">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c26d-160">例</span><span class="sxs-lookup"><span data-stu-id="3c26d-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c26d-161">要求</span><span class="sxs-lookup"><span data-stu-id="3c26d-161">Request</span></span>
<span data-ttu-id="3c26d-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c26d-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
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

### <a name="response"></a><span data-ttu-id="3c26d-163">応答</span><span class="sxs-lookup"><span data-stu-id="3c26d-163">Response</span></span>
<span data-ttu-id="3c26d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3c26d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








