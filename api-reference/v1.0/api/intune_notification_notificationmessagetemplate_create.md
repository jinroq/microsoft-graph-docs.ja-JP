# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="74e57-101">notificationMessageTemplate の作成</span><span class="sxs-lookup"><span data-stu-id="74e57-101">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="74e57-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="74e57-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74e57-103">新しい [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="74e57-103">Create a new [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74e57-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="74e57-104">Prerequisites</span></span>
<span data-ttu-id="74e57-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74e57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="74e57-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74e57-107">Permission type</span></span>|<span data-ttu-id="74e57-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="74e57-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74e57-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="74e57-109">Delegated (work or school account)</span></span>|<span data-ttu-id="74e57-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e57-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="74e57-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74e57-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74e57-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74e57-112">Not supported.</span></span>|
|<span data-ttu-id="74e57-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74e57-113">Application</span></span>|<span data-ttu-id="74e57-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74e57-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74e57-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74e57-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="74e57-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74e57-116">Request headers</span></span>
|<span data-ttu-id="74e57-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74e57-117">Header</span></span>|<span data-ttu-id="74e57-118">値</span><span class="sxs-lookup"><span data-stu-id="74e57-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74e57-119">承認</span><span class="sxs-lookup"><span data-stu-id="74e57-119">Authorization</span></span>|<span data-ttu-id="74e57-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="74e57-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74e57-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="74e57-121">Accept</span></span>|<span data-ttu-id="74e57-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="74e57-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74e57-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="74e57-123">Request body</span></span>
<span data-ttu-id="74e57-124">要求の本文で、notificationMessageTemplate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="74e57-124">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="74e57-125">次の表に、notificationMessageTemplate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="74e57-125">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="74e57-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74e57-126">Property</span></span>|<span data-ttu-id="74e57-127">型</span><span class="sxs-lookup"><span data-stu-id="74e57-127">Type</span></span>|<span data-ttu-id="74e57-128">説明</span><span class="sxs-lookup"><span data-stu-id="74e57-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74e57-129">ID</span><span class="sxs-lookup"><span data-stu-id="74e57-129">id</span></span>|<span data-ttu-id="74e57-130">文字列</span><span class="sxs-lookup"><span data-stu-id="74e57-130">String</span></span>|<span data-ttu-id="74e57-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="74e57-131">Key of the entity.</span></span>|
|<span data-ttu-id="74e57-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74e57-132">lastModifiedDateTime</span></span>|<span data-ttu-id="74e57-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74e57-133">DateTimeOffset</span></span>|<span data-ttu-id="74e57-134">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="74e57-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="74e57-135">displayName</span><span class="sxs-lookup"><span data-stu-id="74e57-135">displayName</span></span>|<span data-ttu-id="74e57-136">文字列</span><span class="sxs-lookup"><span data-stu-id="74e57-136">String</span></span>|<span data-ttu-id="74e57-137">通知メッセージ テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="74e57-137">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="74e57-138">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="74e57-138">defaultLocale</span></span>|<span data-ttu-id="74e57-139">文字列</span><span class="sxs-lookup"><span data-stu-id="74e57-139">String</span></span>|<span data-ttu-id="74e57-140">要求されたロケールが使用できないときにフォールバックする既定のロケール。</span><span class="sxs-lookup"><span data-stu-id="74e57-140">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="74e57-141">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="74e57-141">brandingOptions</span></span>|[<span data-ttu-id="74e57-142">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="74e57-142">notificationTemplateBrandingOptions</span></span>](../resources/intune_notification_notificationtemplatebrandingoptions.md)|<span data-ttu-id="74e57-143">メッセージ テンプレートのブランド化オプション。</span><span class="sxs-lookup"><span data-stu-id="74e57-143">The Message Template Branding Options.</span></span> <span data-ttu-id="74e57-144">ブランド化は、Intune 管理コンソールで定義されます。</span><span class="sxs-lookup"><span data-stu-id="74e57-144">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="74e57-145">可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。</span><span class="sxs-lookup"><span data-stu-id="74e57-145">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="74e57-146">応答</span><span class="sxs-lookup"><span data-stu-id="74e57-146">Response</span></span>
<span data-ttu-id="74e57-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="74e57-147">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74e57-148">例</span><span class="sxs-lookup"><span data-stu-id="74e57-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="74e57-149">要求</span><span class="sxs-lookup"><span data-stu-id="74e57-149">Request</span></span>
<span data-ttu-id="74e57-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74e57-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="74e57-151">応答</span><span class="sxs-lookup"><span data-stu-id="74e57-151">Response</span></span>
<span data-ttu-id="74e57-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74e57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```








