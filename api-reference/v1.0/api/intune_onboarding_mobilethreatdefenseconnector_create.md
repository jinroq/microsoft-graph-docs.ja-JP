# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="6c20b-101">Create mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="6c20b-101">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="6c20b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c20b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c20b-103">新しい [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6c20b-103">Create a new [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c20b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="6c20b-104">Prerequisites</span></span>
<span data-ttu-id="6c20b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c20b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6c20b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c20b-107">Permission type</span></span>|<span data-ttu-id="6c20b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c20b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c20b-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c20b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6c20b-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c20b-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6c20b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c20b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c20b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c20b-112">Not supported.</span></span>|
|<span data-ttu-id="6c20b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c20b-113">Application</span></span>|<span data-ttu-id="6c20b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c20b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c20b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c20b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="6c20b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c20b-116">Request headers</span></span>
|<span data-ttu-id="6c20b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c20b-117">Header</span></span>|<span data-ttu-id="6c20b-118">値</span><span class="sxs-lookup"><span data-stu-id="6c20b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c20b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c20b-119">Authorization</span></span>|<span data-ttu-id="6c20b-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6c20b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c20b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6c20b-121">Accept</span></span>|<span data-ttu-id="6c20b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6c20b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c20b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c20b-123">Request body</span></span>
<span data-ttu-id="6c20b-124">要求本文で、mobileThreatDefenseConnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c20b-124">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="6c20b-125">次の表に、mobileThreatDefenseConnector 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6c20b-125">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="6c20b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c20b-126">Property</span></span>|<span data-ttu-id="6c20b-127">型</span><span class="sxs-lookup"><span data-stu-id="6c20b-127">Type</span></span>|<span data-ttu-id="6c20b-128">説明</span><span class="sxs-lookup"><span data-stu-id="6c20b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c20b-129">id</span><span class="sxs-lookup"><span data-stu-id="6c20b-129">id</span></span>|<span data-ttu-id="6c20b-130">String</span><span class="sxs-lookup"><span data-stu-id="6c20b-130">String</span></span>|<span data-ttu-id="6c20b-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6c20b-131">Not yet documented</span></span>|
|<span data-ttu-id="6c20b-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="6c20b-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="6c20b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c20b-133">DateTimeOffset</span></span>|<span data-ttu-id="6c20b-134">データ同期パートナーから受信した最後のハートビートの日時</span><span class="sxs-lookup"><span data-stu-id="6c20b-134">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="6c20b-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="6c20b-135">partnerState</span></span>|[<span data-ttu-id="6c20b-136">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="6c20b-136">mobileThreatPartnerTenantState</span></span>](../resources/intune_onboarding_mobilethreatpartnertenantstate.md)|<span data-ttu-id="6c20b-137">このアカウントのデータの同期パートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="6c20b-137">Data Sync Partner state for this account.</span></span> <span data-ttu-id="6c20b-138">可能な値は、`unavailable`、`available`、`enabled`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="6c20b-138">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="6c20b-139">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="6c20b-139">androidEnabled</span></span>|<span data-ttu-id="6c20b-140">ブール型</span><span class="sxs-lookup"><span data-stu-id="6c20b-140">Boolean</span></span>|<span data-ttu-id="6c20b-141">Android において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="6c20b-141">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="6c20b-142">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="6c20b-142">iosEnabled</span></span>|<span data-ttu-id="6c20b-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="6c20b-143">Boolean</span></span>|<span data-ttu-id="6c20b-144">IOS において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="6c20b-144">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="6c20b-145">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="6c20b-145">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="6c20b-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="6c20b-146">Boolean</span></span>|<span data-ttu-id="6c20b-147">Android において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="6c20b-147">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="6c20b-148">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="6c20b-148">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="6c20b-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="6c20b-149">Boolean</span></span>|<span data-ttu-id="6c20b-150">IOS において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="6c20b-150">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="6c20b-151">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="6c20b-151">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="6c20b-152">ブール型</span><span class="sxs-lookup"><span data-stu-id="6c20b-152">Boolean</span></span>|<span data-ttu-id="6c20b-153">データ同期パートナーの最小バージョンの要件を満たさない、有効なプラットフォーム上のデバイスをブロックするかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="6c20b-153">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="6c20b-154">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="6c20b-154">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="6c20b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6c20b-155">Int32</span></span>|<span data-ttu-id="6c20b-156">このパートナー統合に関する、テナントごとの無応答許容範囲を取得または設定します</span><span class="sxs-lookup"><span data-stu-id="6c20b-156">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="6c20b-157">応答</span><span class="sxs-lookup"><span data-stu-id="6c20b-157">Response</span></span>
<span data-ttu-id="6c20b-158">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6c20b-158">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c20b-159">例</span><span class="sxs-lookup"><span data-stu-id="6c20b-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c20b-160">要求</span><span class="sxs-lookup"><span data-stu-id="6c20b-160">Request</span></span>
<span data-ttu-id="6c20b-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c20b-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="6c20b-162">応答</span><span class="sxs-lookup"><span data-stu-id="6c20b-162">Response</span></span>
<span data-ttu-id="6c20b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6c20b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



