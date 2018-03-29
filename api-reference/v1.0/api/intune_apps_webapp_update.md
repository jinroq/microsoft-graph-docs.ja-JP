# <a name="update-webapp"></a><span data-ttu-id="198ad-101">Update webApp</span><span class="sxs-lookup"><span data-stu-id="198ad-101">Update webApp</span></span>

> <span data-ttu-id="198ad-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="198ad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="198ad-103">[webApp](../resources/intune_apps_webapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="198ad-103">Update the properties of a [calendar](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="198ad-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="198ad-104">Prerequisites</span></span>
<span data-ttu-id="198ad-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="198ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="198ad-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="198ad-107">Permission type</span></span>|<span data-ttu-id="198ad-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="198ad-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="198ad-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="198ad-109">Delegated (work or school account)</span></span>|<span data-ttu-id="198ad-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="198ad-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="198ad-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="198ad-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="198ad-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="198ad-112">Not supported.</span></span>|
|<span data-ttu-id="198ad-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="198ad-113">Application</span></span>|<span data-ttu-id="198ad-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="198ad-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="198ad-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="198ad-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="198ad-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="198ad-116">Request headers</span></span>
|<span data-ttu-id="198ad-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="198ad-117">Header</span></span>|<span data-ttu-id="198ad-118">値</span><span class="sxs-lookup"><span data-stu-id="198ad-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="198ad-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="198ad-119">Authorization</span></span>|<span data-ttu-id="198ad-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="198ad-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="198ad-121">Accept</span><span class="sxs-lookup"><span data-stu-id="198ad-121">Accept</span></span>|<span data-ttu-id="198ad-122">application/json</span><span class="sxs-lookup"><span data-stu-id="198ad-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="198ad-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="198ad-123">Request body</span></span>
<span data-ttu-id="198ad-124">要求本文で、[webApp](../resources/intune_apps_webapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="198ad-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_webapp.md) object.</span></span>

<span data-ttu-id="198ad-125">次の表に、[webApp](../resources/intune_apps_webapp.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="198ad-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="198ad-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="198ad-126">Property</span></span>|<span data-ttu-id="198ad-127">型</span><span class="sxs-lookup"><span data-stu-id="198ad-127">Type</span></span>|<span data-ttu-id="198ad-128">説明</span><span class="sxs-lookup"><span data-stu-id="198ad-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="198ad-129">id</span><span class="sxs-lookup"><span data-stu-id="198ad-129">id</span></span>|<span data-ttu-id="198ad-130">String</span><span class="sxs-lookup"><span data-stu-id="198ad-130">String</span></span>|<span data-ttu-id="198ad-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="198ad-131">Name of the entity.</span></span> <span data-ttu-id="198ad-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-133">displayName</span><span class="sxs-lookup"><span data-stu-id="198ad-133">displayName</span></span>|<span data-ttu-id="198ad-134">String</span><span class="sxs-lookup"><span data-stu-id="198ad-134">String</span></span>|<span data-ttu-id="198ad-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="198ad-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="198ad-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-137">description</span><span class="sxs-lookup"><span data-stu-id="198ad-137">description</span></span>|<span data-ttu-id="198ad-138">String</span><span class="sxs-lookup"><span data-stu-id="198ad-138">String</span></span>|<span data-ttu-id="198ad-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="198ad-139">The description of the app.</span></span> <span data-ttu-id="198ad-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-141">publisher</span><span class="sxs-lookup"><span data-stu-id="198ad-141">Publisher</span></span>|<span data-ttu-id="198ad-142">String</span><span class="sxs-lookup"><span data-stu-id="198ad-142">String</span></span>|<span data-ttu-id="198ad-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="198ad-143">The name of the app.</span></span> <span data-ttu-id="198ad-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="198ad-145">largeIcon</span></span>|[<span data-ttu-id="198ad-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="198ad-146">MimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="198ad-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="198ad-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="198ad-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="198ad-149">createdDateTime</span></span>|<span data-ttu-id="198ad-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="198ad-150">DateTimeOffset</span></span>|<span data-ttu-id="198ad-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="198ad-151">The date and time when the page was created.</span></span> <span data-ttu-id="198ad-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="198ad-153">lastModifiedDateTime</span></span>|<span data-ttu-id="198ad-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="198ad-154">DateTimeOffset</span></span>|<span data-ttu-id="198ad-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="198ad-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="198ad-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="198ad-157">isFeatured</span></span>|<span data-ttu-id="198ad-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="198ad-158">Boolean</span></span>|<span data-ttu-id="198ad-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="198ad-160">privacyInformationUrl</span></span>|<span data-ttu-id="198ad-161">String</span><span class="sxs-lookup"><span data-stu-id="198ad-161">String</span></span>|<span data-ttu-id="198ad-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="198ad-162">The privacy statement Url.</span></span> <span data-ttu-id="198ad-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="198ad-164">informationUrl</span></span>|<span data-ttu-id="198ad-165">String</span><span class="sxs-lookup"><span data-stu-id="198ad-165">String</span></span>|<span data-ttu-id="198ad-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="198ad-166">The more information Url.</span></span> <span data-ttu-id="198ad-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-168">owner</span><span class="sxs-lookup"><span data-stu-id="198ad-168">owner</span></span>|<span data-ttu-id="198ad-169">String</span><span class="sxs-lookup"><span data-stu-id="198ad-169">String</span></span>|<span data-ttu-id="198ad-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="198ad-170">The owner of the timesheet.</span></span> <span data-ttu-id="198ad-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-172">developer</span><span class="sxs-lookup"><span data-stu-id="198ad-172">developer</span></span>|<span data-ttu-id="198ad-173">String</span><span class="sxs-lookup"><span data-stu-id="198ad-173">String</span></span>|<span data-ttu-id="198ad-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="198ad-174">The name of the app.</span></span> <span data-ttu-id="198ad-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-176">notes</span><span class="sxs-lookup"><span data-stu-id="198ad-176">notes</span></span>|<span data-ttu-id="198ad-177">String</span><span class="sxs-lookup"><span data-stu-id="198ad-177">String</span></span>|<span data-ttu-id="198ad-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="198ad-178">Notes for the app.</span></span> <span data-ttu-id="198ad-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="198ad-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="198ad-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="198ad-180">publishingState</span></span>|<span data-ttu-id="198ad-181">String</span><span class="sxs-lookup"><span data-stu-id="198ad-181">String</span></span>|<span data-ttu-id="198ad-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="198ad-182">The publishing state for the app.</span></span> <span data-ttu-id="198ad-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="198ad-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="198ad-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="198ad-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="198ad-185">appUrl</span><span class="sxs-lookup"><span data-stu-id="198ad-185">appUrl</span></span>|<span data-ttu-id="198ad-186">String</span><span class="sxs-lookup"><span data-stu-id="198ad-186">String</span></span>|<span data-ttu-id="198ad-187">Web アプリの URL。</span><span class="sxs-lookup"><span data-stu-id="198ad-187">The web app URL.</span></span>|
|<span data-ttu-id="198ad-188">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="198ad-188">useManagedBrowser</span></span>|<span data-ttu-id="198ad-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="198ad-189">Boolean</span></span>|<span data-ttu-id="198ad-190">管理対象のブラウザーを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="198ad-190">Whether or not to use managed browser.</span></span> <span data-ttu-id="198ad-191">このプロパティは、Android と iOS にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="198ad-191">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="198ad-192">応答</span><span class="sxs-lookup"><span data-stu-id="198ad-192">Response</span></span>
<span data-ttu-id="198ad-193">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [webApp](../resources/intune_apps_webapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="198ad-193">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="198ad-194">例</span><span class="sxs-lookup"><span data-stu-id="198ad-194">Example</span></span>
### <a name="request"></a><span data-ttu-id="198ad-195">要求</span><span class="sxs-lookup"><span data-stu-id="198ad-195">Request</span></span>
<span data-ttu-id="198ad-196">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="198ad-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 664

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
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

### <a name="response"></a><span data-ttu-id="198ad-197">応答</span><span class="sxs-lookup"><span data-stu-id="198ad-197">Response</span></span>
<span data-ttu-id="198ad-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="198ad-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



