# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="b693c-101">mobileThreatDefenseConnector の更新</span><span class="sxs-lookup"><span data-stu-id="b693c-101">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="b693c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b693c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b693c-103">[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b693c-103">Update the properties of a [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b693c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b693c-104">Prerequisites</span></span>
<span data-ttu-id="b693c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b693c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b693c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b693c-107">Permission type</span></span>|<span data-ttu-id="b693c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b693c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b693c-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="b693c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b693c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b693c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b693c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b693c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b693c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b693c-112">Not supported.</span></span>|
|<span data-ttu-id="b693c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b693c-113">Application</span></span>|<span data-ttu-id="b693c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b693c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b693c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b693c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="b693c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b693c-116">Request headers</span></span>
|<span data-ttu-id="b693c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b693c-117">Header</span></span>|<span data-ttu-id="b693c-118">値</span><span class="sxs-lookup"><span data-stu-id="b693c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b693c-119">承認</span><span class="sxs-lookup"><span data-stu-id="b693c-119">Authorization</span></span>|<span data-ttu-id="b693c-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b693c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b693c-121">承諾</span><span class="sxs-lookup"><span data-stu-id="b693c-121">Accept</span></span>|<span data-ttu-id="b693c-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="b693c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b693c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b693c-123">Request body</span></span>
<span data-ttu-id="b693c-124">要求本文で、[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b693c-124">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="b693c-125">次の表に、[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b693c-125">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="b693c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b693c-126">Property</span></span>|<span data-ttu-id="b693c-127">型</span><span class="sxs-lookup"><span data-stu-id="b693c-127">Type</span></span>|<span data-ttu-id="b693c-128">説明</span><span class="sxs-lookup"><span data-stu-id="b693c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b693c-129">ID</span><span class="sxs-lookup"><span data-stu-id="b693c-129">id</span></span>|<span data-ttu-id="b693c-130">文字列</span><span class="sxs-lookup"><span data-stu-id="b693c-130">String</span></span>|<span data-ttu-id="b693c-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b693c-131">Not yet documented</span></span>|
|<span data-ttu-id="b693c-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="b693c-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="b693c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b693c-133">DateTimeOffset</span></span>|<span data-ttu-id="b693c-134">データ同期パートナーから受信した最後のハートビートの日時</span><span class="sxs-lookup"><span data-stu-id="b693c-134">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="b693c-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="b693c-135">partnerState</span></span>|[<span data-ttu-id="b693c-136">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="b693c-136">mobileThreatPartnerTenantState</span></span>](../resources/intune_onboarding_mobilethreatpartnertenantstate.md)|<span data-ttu-id="b693c-137">このアカウントのデータの同期パートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="b693c-137">Data Sync Partner state for this account Possible values are: , , , .</span></span> <span data-ttu-id="b693c-138">指定できる値は、`unavailable`、`available`、`enabled`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="b693c-138">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="b693c-139">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="b693c-139">androidEnabled</span></span>|<span data-ttu-id="b693c-140">ブール型</span><span class="sxs-lookup"><span data-stu-id="b693c-140">Boolean</span></span>|<span data-ttu-id="b693c-141">Android において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="b693c-141">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b693c-142">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="b693c-142">iosEnabled</span></span>|<span data-ttu-id="b693c-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="b693c-143">Boolean</span></span>|<span data-ttu-id="b693c-144">IOS において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="b693c-144">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b693c-145">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b693c-145">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b693c-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="b693c-146">Boolean</span></span>|<span data-ttu-id="b693c-147">Android において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="b693c-147">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b693c-148">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b693c-148">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b693c-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="b693c-149">Boolean</span></span>|<span data-ttu-id="b693c-150">IOS において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="b693c-150">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b693c-151">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="b693c-151">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="b693c-152">ブール型</span><span class="sxs-lookup"><span data-stu-id="b693c-152">Boolean</span></span>|<span data-ttu-id="b693c-153">データ同期パートナーの最小バージョンの要件を満たさない、有効なプラットフォーム上のデバイスをブロックするかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="b693c-153">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="b693c-154">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="b693c-154">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="b693c-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b693c-155">Int32</span></span>|<span data-ttu-id="b693c-156">このパートナー統合に関する、テナントごとの無応答許容範囲を取得または設定します</span><span class="sxs-lookup"><span data-stu-id="b693c-156">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="b693c-157">応答</span><span class="sxs-lookup"><span data-stu-id="b693c-157">Response</span></span>
<span data-ttu-id="b693c-158">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="b693c-158">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b693c-159">例</span><span class="sxs-lookup"><span data-stu-id="b693c-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="b693c-160">要求</span><span class="sxs-lookup"><span data-stu-id="b693c-160">Request</span></span>
<span data-ttu-id="b693c-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b693c-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 347

{
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

### <a name="response"></a><span data-ttu-id="b693c-162">応答</span><span class="sxs-lookup"><span data-stu-id="b693c-162">Response</span></span>
<span data-ttu-id="b693c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b693c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








