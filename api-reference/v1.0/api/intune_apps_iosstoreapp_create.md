# <a name="create-iosstoreapp"></a><span data-ttu-id="5a0cd-101">iosStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="5a0cd-101">Create iosStoreApp</span></span>

> <span data-ttu-id="5a0cd-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a0cd-103">新しい [iosStoreApp](../resources/intune_apps_iosstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-103">Create a new [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a0cd-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5a0cd-104">Prerequisites</span></span>
<span data-ttu-id="5a0cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5a0cd-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a0cd-107">Permission type</span></span>|<span data-ttu-id="5a0cd-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a0cd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a0cd-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a0cd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5a0cd-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a0cd-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5a0cd-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a0cd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a0cd-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-112">Not supported.</span></span>|
|<span data-ttu-id="5a0cd-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a0cd-113">Application</span></span>|<span data-ttu-id="5a0cd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a0cd-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a0cd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5a0cd-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a0cd-116">Request headers</span></span>
|<span data-ttu-id="5a0cd-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a0cd-117">Header</span></span>|<span data-ttu-id="5a0cd-118">値</span><span class="sxs-lookup"><span data-stu-id="5a0cd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a0cd-119">承認</span><span class="sxs-lookup"><span data-stu-id="5a0cd-119">Authorization</span></span>|<span data-ttu-id="5a0cd-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a0cd-121">承諾</span><span class="sxs-lookup"><span data-stu-id="5a0cd-121">Accept</span></span>|<span data-ttu-id="5a0cd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5a0cd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a0cd-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a0cd-123">Request body</span></span>
<span data-ttu-id="5a0cd-124">要求本文で、iosStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-124">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="5a0cd-125">次の表に、iosStoreApp 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-125">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="5a0cd-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a0cd-126">Property</span></span>|<span data-ttu-id="5a0cd-127">型</span><span class="sxs-lookup"><span data-stu-id="5a0cd-127">Type</span></span>|<span data-ttu-id="5a0cd-128">説明</span><span class="sxs-lookup"><span data-stu-id="5a0cd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a0cd-129">id</span><span class="sxs-lookup"><span data-stu-id="5a0cd-129">id</span></span>|<span data-ttu-id="5a0cd-130">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-130">String</span></span>|<span data-ttu-id="5a0cd-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-131">Key of the entity.</span></span> <span data-ttu-id="5a0cd-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5a0cd-133">displayName</span></span>|<span data-ttu-id="5a0cd-134">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-134">String</span></span>|<span data-ttu-id="5a0cd-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5a0cd-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-137">description</span><span class="sxs-lookup"><span data-stu-id="5a0cd-137">description</span></span>|<span data-ttu-id="5a0cd-138">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-138">String</span></span>|<span data-ttu-id="5a0cd-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-139">The description of the app.</span></span> <span data-ttu-id="5a0cd-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-141">publisher</span><span class="sxs-lookup"><span data-stu-id="5a0cd-141">publisher</span></span>|<span data-ttu-id="5a0cd-142">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-142">String</span></span>|<span data-ttu-id="5a0cd-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-143">The publisher of the app.</span></span> <span data-ttu-id="5a0cd-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5a0cd-145">largeIcon</span></span>|[<span data-ttu-id="5a0cd-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5a0cd-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="5a0cd-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5a0cd-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a0cd-149">createdDateTime</span></span>|<span data-ttu-id="5a0cd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a0cd-150">DateTimeOffset</span></span>|<span data-ttu-id="5a0cd-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-151">The date and time the app was created.</span></span> <span data-ttu-id="5a0cd-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a0cd-153">lastModifiedDateTime</span></span>|<span data-ttu-id="5a0cd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a0cd-154">DateTimeOffset</span></span>|<span data-ttu-id="5a0cd-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-155">The date and time the app was last modified.</span></span> <span data-ttu-id="5a0cd-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5a0cd-157">isFeatured</span></span>|<span data-ttu-id="5a0cd-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a0cd-158">Boolean</span></span>|<span data-ttu-id="5a0cd-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5a0cd-160">privacyInformationUrl</span></span>|<span data-ttu-id="5a0cd-161">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-161">String</span></span>|<span data-ttu-id="5a0cd-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-162">The privacy statement Url.</span></span> <span data-ttu-id="5a0cd-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5a0cd-164">informationUrl</span></span>|<span data-ttu-id="5a0cd-165">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-165">String</span></span>|<span data-ttu-id="5a0cd-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-166">The more information Url.</span></span> <span data-ttu-id="5a0cd-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-168">owner</span><span class="sxs-lookup"><span data-stu-id="5a0cd-168">owner</span></span>|<span data-ttu-id="5a0cd-169">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-169">String</span></span>|<span data-ttu-id="5a0cd-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-170">The owner of the app.</span></span> <span data-ttu-id="5a0cd-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-172">developer</span><span class="sxs-lookup"><span data-stu-id="5a0cd-172">developer</span></span>|<span data-ttu-id="5a0cd-173">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-173">String</span></span>|<span data-ttu-id="5a0cd-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-174">The developer of the app.</span></span> <span data-ttu-id="5a0cd-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-176">notes</span><span class="sxs-lookup"><span data-stu-id="5a0cd-176">notes</span></span>|<span data-ttu-id="5a0cd-177">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-177">String</span></span>|<span data-ttu-id="5a0cd-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-178">Notes for the app.</span></span> <span data-ttu-id="5a0cd-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5a0cd-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5a0cd-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="5a0cd-180">publishingState</span></span>|[<span data-ttu-id="5a0cd-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5a0cd-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="5a0cd-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-182">The publishing state for the app.</span></span> <span data-ttu-id="5a0cd-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5a0cd-184">[MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="5a0cd-185">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5a0cd-186">bundleId</span><span class="sxs-lookup"><span data-stu-id="5a0cd-186">bundleId</span></span>|<span data-ttu-id="5a0cd-187">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-187">String</span></span>|<span data-ttu-id="5a0cd-188">ID 名。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-188">The Identity Name.</span></span>|
|<span data-ttu-id="5a0cd-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5a0cd-189">appStoreUrl</span></span>|<span data-ttu-id="5a0cd-190">String</span><span class="sxs-lookup"><span data-stu-id="5a0cd-190">String</span></span>|<span data-ttu-id="5a0cd-191">Apple App Store の URL。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-191">The Apple App Store URL</span></span>|
|<span data-ttu-id="5a0cd-192">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5a0cd-192">applicableDeviceType</span></span>|[<span data-ttu-id="5a0cd-193">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5a0cd-193">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="5a0cd-194">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-194">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="5a0cd-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5a0cd-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5a0cd-196">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5a0cd-196">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="5a0cd-197">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="5a0cd-198">応答</span><span class="sxs-lookup"><span data-stu-id="5a0cd-198">Response</span></span>
<span data-ttu-id="5a0cd-199">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosStoreApp](../resources/intune_apps_iosstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-199">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a0cd-200">例</span><span class="sxs-lookup"><span data-stu-id="5a0cd-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a0cd-201">要求</span><span class="sxs-lookup"><span data-stu-id="5a0cd-201">Request</span></span>
<span data-ttu-id="5a0cd-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1006

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="5a0cd-203">応答</span><span class="sxs-lookup"><span data-stu-id="5a0cd-203">Response</span></span>
<span data-ttu-id="5a0cd-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5a0cd-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1178

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```



