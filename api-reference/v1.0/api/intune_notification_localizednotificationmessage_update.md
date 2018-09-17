# <a name="update-localizednotificationmessage"></a><span data-ttu-id="dddf0-101">localizedNotificationMessage の更新</span><span class="sxs-lookup"><span data-stu-id="dddf0-101">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="dddf0-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dddf0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dddf0-103">[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dddf0-103">Update the properties of a [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dddf0-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="dddf0-104">Prerequisites</span></span>
<span data-ttu-id="dddf0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dddf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dddf0-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dddf0-107">Permission type</span></span>|<span data-ttu-id="dddf0-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dddf0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dddf0-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="dddf0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dddf0-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dddf0-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dddf0-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dddf0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dddf0-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dddf0-112">Not supported.</span></span>|
|<span data-ttu-id="dddf0-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dddf0-113">Application</span></span>|<span data-ttu-id="dddf0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dddf0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dddf0-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dddf0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="dddf0-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dddf0-116">Request headers</span></span>
|<span data-ttu-id="dddf0-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dddf0-117">Header</span></span>|<span data-ttu-id="dddf0-118">値</span><span class="sxs-lookup"><span data-stu-id="dddf0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dddf0-119">承認</span><span class="sxs-lookup"><span data-stu-id="dddf0-119">Authorization</span></span>|<span data-ttu-id="dddf0-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dddf0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dddf0-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="dddf0-121">Accept</span></span>|<span data-ttu-id="dddf0-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="dddf0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dddf0-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="dddf0-123">Request body</span></span>
<span data-ttu-id="dddf0-124">要求本文で、[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dddf0-124">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="dddf0-125">次の表に、[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dddf0-125">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).</span></span>

|<span data-ttu-id="dddf0-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dddf0-126">Property</span></span>|<span data-ttu-id="dddf0-127">型</span><span class="sxs-lookup"><span data-stu-id="dddf0-127">Type</span></span>|<span data-ttu-id="dddf0-128">説明</span><span class="sxs-lookup"><span data-stu-id="dddf0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dddf0-129">ID</span><span class="sxs-lookup"><span data-stu-id="dddf0-129">id</span></span>|<span data-ttu-id="dddf0-130">文字列</span><span class="sxs-lookup"><span data-stu-id="dddf0-130">String</span></span>|<span data-ttu-id="dddf0-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dddf0-131">Key of the entity.</span></span>|
|<span data-ttu-id="dddf0-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dddf0-132">lastModifiedDateTime</span></span>|<span data-ttu-id="dddf0-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dddf0-133">DateTimeOffset</span></span>|<span data-ttu-id="dddf0-134">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="dddf0-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="dddf0-135">ロケール</span><span class="sxs-lookup"><span data-stu-id="dddf0-135">locale</span></span>|<span data-ttu-id="dddf0-136">文字列</span><span class="sxs-lookup"><span data-stu-id="dddf0-136">String</span></span>|<span data-ttu-id="dddf0-137">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="dddf0-137">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="dddf0-138">件名</span><span class="sxs-lookup"><span data-stu-id="dddf0-138">subject</span></span>|<span data-ttu-id="dddf0-139">文字列</span><span class="sxs-lookup"><span data-stu-id="dddf0-139">String</span></span>|<span data-ttu-id="dddf0-140">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="dddf0-140">The Message Template Subject.</span></span>|
|<span data-ttu-id="dddf0-141">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="dddf0-141">messageTemplate</span></span>|<span data-ttu-id="dddf0-142">文字列</span><span class="sxs-lookup"><span data-stu-id="dddf0-142">String</span></span>|<span data-ttu-id="dddf0-143">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="dddf0-143">The Message Template content.</span></span>|
|<span data-ttu-id="dddf0-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="dddf0-144">isDefault</span></span>|<span data-ttu-id="dddf0-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="dddf0-145">Boolean</span></span>|<span data-ttu-id="dddf0-146">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="dddf0-146">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="dddf0-147">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="dddf0-147">This flag can only be set.</span></span> <span data-ttu-id="dddf0-148">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="dddf0-148">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="dddf0-149">応答</span><span class="sxs-lookup"><span data-stu-id="dddf0-149">Response</span></span>
<span data-ttu-id="dddf0-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dddf0-150">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dddf0-151">例</span><span class="sxs-lookup"><span data-stu-id="dddf0-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="dddf0-152">要求</span><span class="sxs-lookup"><span data-stu-id="dddf0-152">Request</span></span>
<span data-ttu-id="dddf0-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dddf0-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 197

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="dddf0-154">応答</span><span class="sxs-lookup"><span data-stu-id="dddf0-154">Response</span></span>
<span data-ttu-id="dddf0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dddf0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "7a777708-7708-7a77-0877-777a0877777a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```








