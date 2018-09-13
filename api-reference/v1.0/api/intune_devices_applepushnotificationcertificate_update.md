# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="b28ce-101">applePushNotificationCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="b28ce-101">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="b28ce-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b28ce-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b28ce-103">[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b28ce-103">Update the properties of a [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b28ce-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b28ce-104">Prerequisites</span></span>
<span data-ttu-id="b28ce-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b28ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b28ce-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b28ce-107">Permission type</span></span>|<span data-ttu-id="b28ce-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b28ce-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b28ce-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b28ce-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b28ce-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b28ce-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b28ce-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b28ce-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b28ce-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b28ce-112">Not supported.</span></span>|
|<span data-ttu-id="b28ce-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b28ce-113">Application</span></span>|<span data-ttu-id="b28ce-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b28ce-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b28ce-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b28ce-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="b28ce-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b28ce-116">Request headers</span></span>
|<span data-ttu-id="b28ce-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b28ce-117">Header</span></span>|<span data-ttu-id="b28ce-118">値</span><span class="sxs-lookup"><span data-stu-id="b28ce-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b28ce-119">承認</span><span class="sxs-lookup"><span data-stu-id="b28ce-119">Authorization</span></span>|<span data-ttu-id="b28ce-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b28ce-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b28ce-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="b28ce-121">Accept</span></span>|<span data-ttu-id="b28ce-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="b28ce-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b28ce-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b28ce-123">Request body</span></span>
<span data-ttu-id="b28ce-124">要求本文で、[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b28ce-124">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="b28ce-125">次の表に、[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b28ce-125">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="b28ce-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b28ce-126">Property</span></span>|<span data-ttu-id="b28ce-127">型</span><span class="sxs-lookup"><span data-stu-id="b28ce-127">Type</span></span>|<span data-ttu-id="b28ce-128">説明</span><span class="sxs-lookup"><span data-stu-id="b28ce-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b28ce-129">ID</span><span class="sxs-lookup"><span data-stu-id="b28ce-129">id</span></span>|<span data-ttu-id="b28ce-130">文字列</span><span class="sxs-lookup"><span data-stu-id="b28ce-130">String</span></span>|<span data-ttu-id="b28ce-131">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="b28ce-131">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="b28ce-132">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="b28ce-132">appleIdentifier</span></span>|<span data-ttu-id="b28ce-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b28ce-133">String</span></span>|<span data-ttu-id="b28ce-134">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="b28ce-134">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="b28ce-135">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="b28ce-135">topicIdentifier</span></span>|<span data-ttu-id="b28ce-136">文字列</span><span class="sxs-lookup"><span data-stu-id="b28ce-136">String</span></span>|<span data-ttu-id="b28ce-137">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="b28ce-137">Topic Id.</span></span>|
|<span data-ttu-id="b28ce-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b28ce-138">lastModifiedDateTime</span></span>|<span data-ttu-id="b28ce-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28ce-139">DateTimeOffset</span></span>|<span data-ttu-id="b28ce-140">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="b28ce-140">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b28ce-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b28ce-141">expirationDateTime</span></span>|<span data-ttu-id="b28ce-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28ce-142">DateTimeOffset</span></span>|<span data-ttu-id="b28ce-143">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="b28ce-143">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="b28ce-144">証明書</span><span class="sxs-lookup"><span data-stu-id="b28ce-144">certificate</span></span>|<span data-ttu-id="b28ce-145">文字列</span><span class="sxs-lookup"><span data-stu-id="b28ce-145">String</span></span>|<span data-ttu-id="b28ce-146">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b28ce-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b28ce-147">応答</span><span class="sxs-lookup"><span data-stu-id="b28ce-147">Response</span></span>
<span data-ttu-id="b28ce-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b28ce-148">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b28ce-149">例</span><span class="sxs-lookup"><span data-stu-id="b28ce-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="b28ce-150">要求</span><span class="sxs-lookup"><span data-stu-id="b28ce-150">Request</span></span>
<span data-ttu-id="b28ce-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b28ce-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 264

{
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="b28ce-152">応答</span><span class="sxs-lookup"><span data-stu-id="b28ce-152">Response</span></span>
<span data-ttu-id="b28ce-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b28ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```








