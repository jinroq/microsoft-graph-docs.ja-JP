# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="d0d15-101">Create mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="d0d15-101">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="d0d15-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d0d15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0d15-103">新しい [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d0d15-103">Create a new [plannerBucket](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0d15-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="d0d15-104">Prerequisites</span></span>
<span data-ttu-id="d0d15-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0d15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0d15-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0d15-107">Permission type</span></span>|<span data-ttu-id="d0d15-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0d15-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0d15-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0d15-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d0d15-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0d15-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d0d15-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0d15-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0d15-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0d15-112">Not supported.</span></span>|
|<span data-ttu-id="d0d15-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0d15-113">Application</span></span>|<span data-ttu-id="d0d15-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0d15-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0d15-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0d15-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="d0d15-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0d15-116">Request headers</span></span>
|<span data-ttu-id="d0d15-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0d15-117">Header</span></span>|<span data-ttu-id="d0d15-118">値</span><span class="sxs-lookup"><span data-stu-id="d0d15-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0d15-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0d15-119">Authorization</span></span>|<span data-ttu-id="d0d15-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d0d15-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d0d15-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d0d15-121">Accept</span></span>|<span data-ttu-id="d0d15-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d0d15-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0d15-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0d15-123">Request body</span></span>
<span data-ttu-id="d0d15-124">要求本文で、mobileThreatDefenseConnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0d15-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="d0d15-125">次の表に、mobileThreatDefenseConnector 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d0d15-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d0d15-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0d15-126">Property</span></span>|<span data-ttu-id="d0d15-127">型</span><span class="sxs-lookup"><span data-stu-id="d0d15-127">Type</span></span>|<span data-ttu-id="d0d15-128">説明</span><span class="sxs-lookup"><span data-stu-id="d0d15-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0d15-129">id</span><span class="sxs-lookup"><span data-stu-id="d0d15-129">id</span></span>|<span data-ttu-id="d0d15-130">String</span><span class="sxs-lookup"><span data-stu-id="d0d15-130">String</span></span>|<span data-ttu-id="d0d15-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d0d15-131">Not yet documented</span></span>|
|<span data-ttu-id="d0d15-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="d0d15-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="d0d15-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0d15-133">DateTimeOffset</span></span>|<span data-ttu-id="d0d15-134">管理者が MTP へのオプション接続を有効にした後の、最後のハートビートのタイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="d0d15-134">Timestamp of last heartbeat after admin enabled option Connect to MTP</span></span>|
|<span data-ttu-id="d0d15-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="d0d15-135">partnerState</span></span>|<span data-ttu-id="d0d15-136">String</span><span class="sxs-lookup"><span data-stu-id="d0d15-136">String</span></span>|<span data-ttu-id="d0d15-137">このテナントのパートナーの状態です。可能な値は、`unavailable`、`available`、`enabled`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="d0d15-137">Partner state of this tenant Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="d0d15-138">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="d0d15-138">androidEnabled</span></span>|<span data-ttu-id="d0d15-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0d15-139">Boolean</span></span>|<span data-ttu-id="d0d15-140">Android 切り替えのオンまたはオフ</span><span class="sxs-lookup"><span data-stu-id="d0d15-140">Android Toggle On or Off</span></span>|
|<span data-ttu-id="d0d15-141">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="d0d15-141">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="d0d15-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0d15-142">Boolean</span></span>|<span data-ttu-id="d0d15-143">Android において、管理者がデータ同期パートナーの準拠を判断する前に、データ同期パートナーからの受信必須データを設定できるようにします</span><span class="sxs-lookup"><span data-stu-id="d0d15-143">For Android, Allows admin to config must receive data from the data sync partner prior to being considered compliant</span></span>|
|<span data-ttu-id="d0d15-144">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="d0d15-144">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="d0d15-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0d15-145">Boolean</span></span>|<span data-ttu-id="d0d15-146">iOS の場合、管理者がデータ同期パートナーの準拠を判断する前に、データ同期パートナーからの受信必須データを設定できるようにします</span><span class="sxs-lookup"><span data-stu-id="d0d15-146">For IOS, Allows admin to config must receive data from the data sync partner prior to being considered compliant</span></span>|
|<span data-ttu-id="d0d15-147">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="d0d15-147">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="d0d15-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0d15-148">Boolean</span></span>|<span data-ttu-id="d0d15-149">有効にされたプラットフォーム上にあっても最低バージョン要件を満たさないデバイスを管理者がブロックできるようにします</span><span class="sxs-lookup"><span data-stu-id="d0d15-149">Allows admin to block devices on the enabled platforms that do not meet minimum version requirements</span></span>|
|<span data-ttu-id="d0d15-150">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="d0d15-150">iosEnabled</span></span>|<span data-ttu-id="d0d15-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0d15-151">Boolean</span></span>|<span data-ttu-id="d0d15-152">iOS 切り替えのオンまたはオフ</span><span class="sxs-lookup"><span data-stu-id="d0d15-152">IOS Toggle On or Off</span></span>|
|<span data-ttu-id="d0d15-153">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="d0d15-153">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="d0d15-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d0d15-154">Int32</span></span>|<span data-ttu-id="d0d15-155">このパートナー統合に関する、テナントごとの無応答許容範囲を取得または設定します</span><span class="sxs-lookup"><span data-stu-id="d0d15-155">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="d0d15-156">応答</span><span class="sxs-lookup"><span data-stu-id="d0d15-156">Response</span></span>
<span data-ttu-id="d0d15-157">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d0d15-157">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0d15-158">例</span><span class="sxs-lookup"><span data-stu-id="d0d15-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0d15-159">要求</span><span class="sxs-lookup"><span data-stu-id="d0d15-159">Request</span></span>
<span data-ttu-id="d0d15-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d0d15-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="d0d15-161">応答</span><span class="sxs-lookup"><span data-stu-id="d0d15-161">Response</span></span>
<span data-ttu-id="d0d15-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d0d15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



