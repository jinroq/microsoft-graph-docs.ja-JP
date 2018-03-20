# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="5052e-101">applePushNotificationCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="5052e-101">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="5052e-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5052e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5052e-103">[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5052e-103">Update the properties of a [calendar](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5052e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5052e-104">Prerequisites</span></span>
<span data-ttu-id="5052e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5052e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5052e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5052e-107">Permission type</span></span>|<span data-ttu-id="5052e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5052e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5052e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5052e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5052e-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5052e-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5052e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5052e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5052e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5052e-112">Not supported.</span></span>|
|<span data-ttu-id="5052e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5052e-113">Application</span></span>|<span data-ttu-id="5052e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5052e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5052e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5052e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="5052e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5052e-116">Request headers</span></span>
|<span data-ttu-id="5052e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5052e-117">Header</span></span>|<span data-ttu-id="5052e-118">値</span><span class="sxs-lookup"><span data-stu-id="5052e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5052e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5052e-119">Authorization</span></span>|<span data-ttu-id="5052e-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5052e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5052e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5052e-121">Accept</span></span>|<span data-ttu-id="5052e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5052e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5052e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5052e-123">Request body</span></span>
<span data-ttu-id="5052e-124">要求本文で、[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5052e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="5052e-125">次の表に、[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5052e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5052e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5052e-126">Property</span></span>|<span data-ttu-id="5052e-127">型</span><span class="sxs-lookup"><span data-stu-id="5052e-127">Type</span></span>|<span data-ttu-id="5052e-128">説明</span><span class="sxs-lookup"><span data-stu-id="5052e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5052e-129">id</span><span class="sxs-lookup"><span data-stu-id="5052e-129">id</span></span>|<span data-ttu-id="5052e-130">String</span><span class="sxs-lookup"><span data-stu-id="5052e-130">String</span></span>|<span data-ttu-id="5052e-131">証明書の一意識別子</span><span class="sxs-lookup"><span data-stu-id="5052e-131">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="5052e-132">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="5052e-132">appleIdentifier</span></span>|<span data-ttu-id="5052e-133">String</span><span class="sxs-lookup"><span data-stu-id="5052e-133">String</span></span>|<span data-ttu-id="5052e-134">MDM プッシュ証明書の作成に使用するアカウントの Apple ID。</span><span class="sxs-lookup"><span data-stu-id="5052e-134">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="5052e-135">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="5052e-135">topicIdentifier</span></span>|<span data-ttu-id="5052e-136">String</span><span class="sxs-lookup"><span data-stu-id="5052e-136">String</span></span>|<span data-ttu-id="5052e-137">トピック ID。</span><span class="sxs-lookup"><span data-stu-id="5052e-137">Topic Id.</span></span>|
|<span data-ttu-id="5052e-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5052e-138">lastModifiedDateTime</span></span>|<span data-ttu-id="5052e-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5052e-139">DateTimeOffset</span></span>|<span data-ttu-id="5052e-140">Apple プッシュ通知証明書の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="5052e-140">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5052e-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5052e-141">expirationDateTime</span></span>|<span data-ttu-id="5052e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5052e-142">DateTimeOffset</span></span>|<span data-ttu-id="5052e-143">Apple プッシュ通知証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="5052e-143">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5052e-144">証明書</span><span class="sxs-lookup"><span data-stu-id="5052e-144">ACS, certificate</span></span>|<span data-ttu-id="5052e-145">String</span><span class="sxs-lookup"><span data-stu-id="5052e-145">String</span></span>|<span data-ttu-id="5052e-146">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5052e-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5052e-147">応答</span><span class="sxs-lookup"><span data-stu-id="5052e-147">Response</span></span>
<span data-ttu-id="5052e-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5052e-148">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5052e-149">例</span><span class="sxs-lookup"><span data-stu-id="5052e-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="5052e-150">要求</span><span class="sxs-lookup"><span data-stu-id="5052e-150">Request</span></span>
<span data-ttu-id="5052e-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5052e-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5052e-152">応答</span><span class="sxs-lookup"><span data-stu-id="5052e-152">Response</span></span>
<span data-ttu-id="5052e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5052e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



