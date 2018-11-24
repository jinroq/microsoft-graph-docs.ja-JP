# <a name="create-localizednotificationmessage"></a><span data-ttu-id="5fb61-101">localizedNotificationMessage の作成</span><span class="sxs-lookup"><span data-stu-id="5fb61-101">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="5fb61-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5fb61-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fb61-103">新しい [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5fb61-103">Create a new [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5fb61-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5fb61-104">Prerequisites</span></span>
<span data-ttu-id="5fb61-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5fb61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5fb61-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5fb61-107">Permission type</span></span>|<span data-ttu-id="5fb61-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5fb61-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fb61-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5fb61-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5fb61-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fb61-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5fb61-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5fb61-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fb61-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5fb61-112">Not supported.</span></span>|
|<span data-ttu-id="5fb61-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5fb61-113">Application</span></span>|<span data-ttu-id="5fb61-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5fb61-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fb61-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5fb61-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="5fb61-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5fb61-116">Request headers</span></span>
|<span data-ttu-id="5fb61-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5fb61-117">Header</span></span>|<span data-ttu-id="5fb61-118">値</span><span class="sxs-lookup"><span data-stu-id="5fb61-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fb61-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fb61-119">Authorization</span></span>|<span data-ttu-id="5fb61-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5fb61-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fb61-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5fb61-121">Accept</span></span>|<span data-ttu-id="5fb61-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5fb61-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fb61-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5fb61-123">Request body</span></span>
<span data-ttu-id="5fb61-124">要求本文で、localizedNotificationMessage オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5fb61-124">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="5fb61-125">次の表に、localizedNotificationMessage の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5fb61-125">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="5fb61-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5fb61-126">Property</span></span>|<span data-ttu-id="5fb61-127">型</span><span class="sxs-lookup"><span data-stu-id="5fb61-127">Type</span></span>|<span data-ttu-id="5fb61-128">説明</span><span class="sxs-lookup"><span data-stu-id="5fb61-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fb61-129">id</span><span class="sxs-lookup"><span data-stu-id="5fb61-129">id</span></span>|<span data-ttu-id="5fb61-130">String</span><span class="sxs-lookup"><span data-stu-id="5fb61-130">String</span></span>|<span data-ttu-id="5fb61-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5fb61-131">Key of the entity.</span></span>|
|<span data-ttu-id="5fb61-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fb61-132">lastModifiedDateTime</span></span>|<span data-ttu-id="5fb61-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fb61-133">DateTimeOffset</span></span>|<span data-ttu-id="5fb61-134">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="5fb61-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5fb61-135">locale</span><span class="sxs-lookup"><span data-stu-id="5fb61-135">locale</span></span>|<span data-ttu-id="5fb61-136">String</span><span class="sxs-lookup"><span data-stu-id="5fb61-136">String</span></span>|<span data-ttu-id="5fb61-137">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="5fb61-137">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="5fb61-138">subject</span><span class="sxs-lookup"><span data-stu-id="5fb61-138">subject</span></span>|<span data-ttu-id="5fb61-139">String</span><span class="sxs-lookup"><span data-stu-id="5fb61-139">String</span></span>|<span data-ttu-id="5fb61-140">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="5fb61-140">The Message Template Subject.</span></span>|
|<span data-ttu-id="5fb61-141">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="5fb61-141">messageTemplate</span></span>|<span data-ttu-id="5fb61-142">String</span><span class="sxs-lookup"><span data-stu-id="5fb61-142">String</span></span>|<span data-ttu-id="5fb61-143">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="5fb61-143">The Message Template content.</span></span>|
|<span data-ttu-id="5fb61-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="5fb61-144">isDefault</span></span>|<span data-ttu-id="5fb61-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb61-145">Boolean</span></span>|<span data-ttu-id="5fb61-146">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="5fb61-146">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="5fb61-147">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5fb61-147">This flag can only be set.</span></span> <span data-ttu-id="5fb61-148">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="5fb61-148">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="5fb61-149">応答</span><span class="sxs-lookup"><span data-stu-id="5fb61-149">Response</span></span>
<span data-ttu-id="5fb61-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5fb61-150">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fb61-151">例</span><span class="sxs-lookup"><span data-stu-id="5fb61-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="5fb61-152">要求</span><span class="sxs-lookup"><span data-stu-id="5fb61-152">Request</span></span>
<span data-ttu-id="5fb61-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5fb61-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="5fb61-154">応答</span><span class="sxs-lookup"><span data-stu-id="5fb61-154">Response</span></span>
<span data-ttu-id="5fb61-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5fb61-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



