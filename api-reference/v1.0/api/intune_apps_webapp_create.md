# <a name="create-webapp"></a><span data-ttu-id="df284-101">webApp の作成</span><span class="sxs-lookup"><span data-stu-id="df284-101">Create webApp</span></span>

> <span data-ttu-id="df284-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="df284-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df284-103">新しい [webApp](../resources/intune_apps_webapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="df284-103">Create a new [webApp](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df284-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="df284-104">Prerequisites</span></span>
<span data-ttu-id="df284-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="df284-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df284-107">Permission type</span></span>|<span data-ttu-id="df284-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="df284-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df284-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df284-109">Delegated (work or school account)</span></span>|<span data-ttu-id="df284-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df284-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="df284-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="df284-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df284-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df284-112">Not supported.</span></span>|
|<span data-ttu-id="df284-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df284-113">Application</span></span>|<span data-ttu-id="df284-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df284-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df284-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df284-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="df284-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df284-116">Request headers</span></span>
|<span data-ttu-id="df284-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df284-117">Header</span></span>|<span data-ttu-id="df284-118">値</span><span class="sxs-lookup"><span data-stu-id="df284-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df284-119">承認</span><span class="sxs-lookup"><span data-stu-id="df284-119">Authorization</span></span>|<span data-ttu-id="df284-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="df284-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df284-121">承諾</span><span class="sxs-lookup"><span data-stu-id="df284-121">Accept</span></span>|<span data-ttu-id="df284-122">application/json</span><span class="sxs-lookup"><span data-stu-id="df284-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df284-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="df284-123">Request body</span></span>
<span data-ttu-id="df284-124">要求本文で、webApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="df284-124">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="df284-125">次の表に、webApp 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="df284-125">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="df284-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df284-126">Property</span></span>|<span data-ttu-id="df284-127">型</span><span class="sxs-lookup"><span data-stu-id="df284-127">Type</span></span>|<span data-ttu-id="df284-128">説明</span><span class="sxs-lookup"><span data-stu-id="df284-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df284-129">id</span><span class="sxs-lookup"><span data-stu-id="df284-129">id</span></span>|<span data-ttu-id="df284-130">String</span><span class="sxs-lookup"><span data-stu-id="df284-130">String</span></span>|<span data-ttu-id="df284-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="df284-131">Key of the entity.</span></span> <span data-ttu-id="df284-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-133">displayName</span><span class="sxs-lookup"><span data-stu-id="df284-133">displayName</span></span>|<span data-ttu-id="df284-134">String</span><span class="sxs-lookup"><span data-stu-id="df284-134">String</span></span>|<span data-ttu-id="df284-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="df284-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="df284-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-137">description</span><span class="sxs-lookup"><span data-stu-id="df284-137">description</span></span>|<span data-ttu-id="df284-138">String</span><span class="sxs-lookup"><span data-stu-id="df284-138">String</span></span>|<span data-ttu-id="df284-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="df284-139">The description of the app.</span></span> <span data-ttu-id="df284-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-141">publisher</span><span class="sxs-lookup"><span data-stu-id="df284-141">publisher</span></span>|<span data-ttu-id="df284-142">String</span><span class="sxs-lookup"><span data-stu-id="df284-142">String</span></span>|<span data-ttu-id="df284-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="df284-143">The publisher of the app.</span></span> <span data-ttu-id="df284-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="df284-145">largeIcon</span></span>|[<span data-ttu-id="df284-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df284-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="df284-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="df284-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="df284-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df284-149">createdDateTime</span></span>|<span data-ttu-id="df284-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df284-150">DateTimeOffset</span></span>|<span data-ttu-id="df284-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="df284-151">The date and time the app was created.</span></span> <span data-ttu-id="df284-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df284-153">lastModifiedDateTime</span></span>|<span data-ttu-id="df284-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df284-154">DateTimeOffset</span></span>|<span data-ttu-id="df284-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="df284-155">The date and time the app was last modified.</span></span> <span data-ttu-id="df284-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="df284-157">isFeatured</span></span>|<span data-ttu-id="df284-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="df284-158">Boolean</span></span>|<span data-ttu-id="df284-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="df284-160">privacyInformationUrl</span></span>|<span data-ttu-id="df284-161">String</span><span class="sxs-lookup"><span data-stu-id="df284-161">String</span></span>|<span data-ttu-id="df284-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="df284-162">The privacy statement Url.</span></span> <span data-ttu-id="df284-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="df284-164">informationUrl</span></span>|<span data-ttu-id="df284-165">String</span><span class="sxs-lookup"><span data-stu-id="df284-165">String</span></span>|<span data-ttu-id="df284-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="df284-166">The more information Url.</span></span> <span data-ttu-id="df284-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-168">owner</span><span class="sxs-lookup"><span data-stu-id="df284-168">owner</span></span>|<span data-ttu-id="df284-169">String</span><span class="sxs-lookup"><span data-stu-id="df284-169">String</span></span>|<span data-ttu-id="df284-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="df284-170">The owner of the app.</span></span> <span data-ttu-id="df284-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-172">developer</span><span class="sxs-lookup"><span data-stu-id="df284-172">developer</span></span>|<span data-ttu-id="df284-173">String</span><span class="sxs-lookup"><span data-stu-id="df284-173">String</span></span>|<span data-ttu-id="df284-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="df284-174">The developer of the app.</span></span> <span data-ttu-id="df284-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-176">notes</span><span class="sxs-lookup"><span data-stu-id="df284-176">notes</span></span>|<span data-ttu-id="df284-177">String</span><span class="sxs-lookup"><span data-stu-id="df284-177">String</span></span>|<span data-ttu-id="df284-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="df284-178">Notes for the app.</span></span> <span data-ttu-id="df284-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df284-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df284-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="df284-180">publishingState</span></span>|[<span data-ttu-id="df284-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="df284-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="df284-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="df284-182">The publishing state for the app.</span></span> <span data-ttu-id="df284-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="df284-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="df284-184">[MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="df284-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="df284-185">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="df284-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="df284-186">appUrl</span><span class="sxs-lookup"><span data-stu-id="df284-186">appUrl</span></span>|<span data-ttu-id="df284-187">String</span><span class="sxs-lookup"><span data-stu-id="df284-187">String</span></span>|<span data-ttu-id="df284-188">Web アプリの URL。</span><span class="sxs-lookup"><span data-stu-id="df284-188">The web app URL.</span></span>|
|<span data-ttu-id="df284-189">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="df284-189">useManagedBrowser</span></span>|<span data-ttu-id="df284-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="df284-190">Boolean</span></span>|<span data-ttu-id="df284-191">管理対象のブラウザーを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="df284-191">Whether or not to use managed browser.</span></span> <span data-ttu-id="df284-192">このプロパティは、Android と iOS にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="df284-192">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="df284-193">応答</span><span class="sxs-lookup"><span data-stu-id="df284-193">Response</span></span>
<span data-ttu-id="df284-194">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [webApp](../resources/intune_apps_webapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="df284-194">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df284-195">例</span><span class="sxs-lookup"><span data-stu-id="df284-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="df284-196">要求</span><span class="sxs-lookup"><span data-stu-id="df284-196">Request</span></span>
<span data-ttu-id="df284-197">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="df284-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.webApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="df284-198">応答</span><span class="sxs-lookup"><span data-stu-id="df284-198">Response</span></span>
<span data-ttu-id="df284-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="df284-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 817

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```



