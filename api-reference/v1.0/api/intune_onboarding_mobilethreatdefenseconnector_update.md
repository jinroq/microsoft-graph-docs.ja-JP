# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="337b2-101">mobileThreatDefenseConnector の更新</span><span class="sxs-lookup"><span data-stu-id="337b2-101">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="337b2-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="337b2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="337b2-103">[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="337b2-103">Update the properties of a [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="337b2-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="337b2-104">Prerequisites</span></span>
<span data-ttu-id="337b2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="337b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="337b2-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="337b2-107">Permission type</span></span>|<span data-ttu-id="337b2-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="337b2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="337b2-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="337b2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="337b2-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="337b2-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="337b2-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="337b2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="337b2-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="337b2-112">Not supported.</span></span>|
|<span data-ttu-id="337b2-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="337b2-113">Application</span></span>|<span data-ttu-id="337b2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="337b2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="337b2-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="337b2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="337b2-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="337b2-116">Request headers</span></span>
|<span data-ttu-id="337b2-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="337b2-117">Header</span></span>|<span data-ttu-id="337b2-118">値</span><span class="sxs-lookup"><span data-stu-id="337b2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="337b2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="337b2-119">Authorization</span></span>|<span data-ttu-id="337b2-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="337b2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="337b2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="337b2-121">Accept</span></span>|<span data-ttu-id="337b2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="337b2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="337b2-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="337b2-123">Request body</span></span>
<span data-ttu-id="337b2-124">要求本文で、[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="337b2-124">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="337b2-125">次の表に、[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="337b2-125">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="337b2-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="337b2-126">Property</span></span>|<span data-ttu-id="337b2-127">型</span><span class="sxs-lookup"><span data-stu-id="337b2-127">Type</span></span>|<span data-ttu-id="337b2-128">説明</span><span class="sxs-lookup"><span data-stu-id="337b2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="337b2-129">id</span><span class="sxs-lookup"><span data-stu-id="337b2-129">id</span></span>|<span data-ttu-id="337b2-130">String</span><span class="sxs-lookup"><span data-stu-id="337b2-130">String</span></span>|<span data-ttu-id="337b2-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="337b2-131">Not yet documented</span></span>|
|<span data-ttu-id="337b2-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="337b2-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="337b2-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="337b2-133">DateTimeOffset</span></span>|<span data-ttu-id="337b2-134">データ同期パートナーから受信した最後のハートビートの日時</span><span class="sxs-lookup"><span data-stu-id="337b2-134">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="337b2-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="337b2-135">partnerState</span></span>|<span data-ttu-id="337b2-136">String</span><span class="sxs-lookup"><span data-stu-id="337b2-136">String</span></span>|<span data-ttu-id="337b2-137">このアカウントのデータ同期パートナーの状態です。使用可能な値は、`unavailable`、 `available`、 `enabled`、`unresponsive`です。</span><span class="sxs-lookup"><span data-stu-id="337b2-137">Data Sync Partner state for this account Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="337b2-138">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="337b2-138">androidEnabled</span></span>|<span data-ttu-id="337b2-139">ブール型</span><span class="sxs-lookup"><span data-stu-id="337b2-139">Boolean</span></span>|<span data-ttu-id="337b2-140">Android において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="337b2-140">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="337b2-141">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="337b2-141">iosEnabled</span></span>|<span data-ttu-id="337b2-142">ブール型</span><span class="sxs-lookup"><span data-stu-id="337b2-142">Boolean</span></span>|<span data-ttu-id="337b2-143">IOS において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="337b2-143">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="337b2-144">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="337b2-144">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="337b2-145">ブール型</span><span class="sxs-lookup"><span data-stu-id="337b2-145">Boolean</span></span>|<span data-ttu-id="337b2-146">Android において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="337b2-146">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="337b2-147">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="337b2-147">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="337b2-148">ブール型</span><span class="sxs-lookup"><span data-stu-id="337b2-148">Boolean</span></span>|<span data-ttu-id="337b2-149">IOS において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="337b2-149">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="337b2-150">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="337b2-150">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="337b2-151">ブール型</span><span class="sxs-lookup"><span data-stu-id="337b2-151">Boolean</span></span>|<span data-ttu-id="337b2-152">データ同期パートナーの最小バージョンの要件を満たさない、有効なプラットフォーム上のデバイスをブロックするかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="337b2-152">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="337b2-153">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="337b2-153">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="337b2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="337b2-154">Int32</span></span>|<span data-ttu-id="337b2-155">このパートナー統合に関する、テナントごとの無応答許容範囲を取得または設定します</span><span class="sxs-lookup"><span data-stu-id="337b2-155">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="337b2-156">応答</span><span class="sxs-lookup"><span data-stu-id="337b2-156">Response</span></span>
<span data-ttu-id="337b2-157">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="337b2-157">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="337b2-158">例</span><span class="sxs-lookup"><span data-stu-id="337b2-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="337b2-159">要求</span><span class="sxs-lookup"><span data-stu-id="337b2-159">Request</span></span>
<span data-ttu-id="337b2-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="337b2-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="337b2-161">応答</span><span class="sxs-lookup"><span data-stu-id="337b2-161">Response</span></span>
<span data-ttu-id="337b2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="337b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



