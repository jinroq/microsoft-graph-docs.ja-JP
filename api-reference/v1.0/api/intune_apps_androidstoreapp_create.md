# <a name="create-androidstoreapp"></a><span data-ttu-id="eebcb-101">androidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="eebcb-101">Create androidStoreApp</span></span>

> <span data-ttu-id="eebcb-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eebcb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eebcb-103">新しい [androidStoreApp](../resources/intune_apps_androidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="eebcb-103">Create a new [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eebcb-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="eebcb-104">Prerequisites</span></span>
<span data-ttu-id="eebcb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eebcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eebcb-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eebcb-107">Permission type</span></span>|<span data-ttu-id="eebcb-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="eebcb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eebcb-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eebcb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="eebcb-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eebcb-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eebcb-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eebcb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eebcb-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eebcb-112">Not supported.</span></span>|
|<span data-ttu-id="eebcb-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eebcb-113">Application</span></span>|<span data-ttu-id="eebcb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eebcb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eebcb-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eebcb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="eebcb-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eebcb-116">Request headers</span></span>
|<span data-ttu-id="eebcb-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eebcb-117">Header</span></span>|<span data-ttu-id="eebcb-118">値</span><span class="sxs-lookup"><span data-stu-id="eebcb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eebcb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="eebcb-119">Authorization</span></span>|<span data-ttu-id="eebcb-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="eebcb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eebcb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="eebcb-121">Accept</span></span>|<span data-ttu-id="eebcb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="eebcb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eebcb-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="eebcb-123">Request body</span></span>
<span data-ttu-id="eebcb-124">要求本文で、androidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eebcb-124">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="eebcb-125">次の表に、androidStoreApp の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="eebcb-125">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="eebcb-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eebcb-126">Property</span></span>|<span data-ttu-id="eebcb-127">型</span><span class="sxs-lookup"><span data-stu-id="eebcb-127">Type</span></span>|<span data-ttu-id="eebcb-128">説明</span><span class="sxs-lookup"><span data-stu-id="eebcb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eebcb-129">id</span><span class="sxs-lookup"><span data-stu-id="eebcb-129">id</span></span>|<span data-ttu-id="eebcb-130">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-130">String</span></span>|<span data-ttu-id="eebcb-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="eebcb-131">Key of the entity.</span></span> <span data-ttu-id="eebcb-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="eebcb-133">displayName</span></span>|<span data-ttu-id="eebcb-134">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-134">String</span></span>|<span data-ttu-id="eebcb-135">管理者が指定またはインポートした、アプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="eebcb-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eebcb-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-137">description</span><span class="sxs-lookup"><span data-stu-id="eebcb-137">description</span></span>|<span data-ttu-id="eebcb-138">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-138">String</span></span>|<span data-ttu-id="eebcb-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="eebcb-139">The description of the app.</span></span> <span data-ttu-id="eebcb-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-141">publisher</span><span class="sxs-lookup"><span data-stu-id="eebcb-141">publisher</span></span>|<span data-ttu-id="eebcb-142">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-142">String</span></span>|<span data-ttu-id="eebcb-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="eebcb-143">The publisher of the app.</span></span> <span data-ttu-id="eebcb-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eebcb-145">largeIcon</span></span>|[<span data-ttu-id="eebcb-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eebcb-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="eebcb-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="eebcb-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eebcb-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eebcb-149">createdDateTime</span></span>|<span data-ttu-id="eebcb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eebcb-150">DateTimeOffset</span></span>|<span data-ttu-id="eebcb-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="eebcb-151">The date and time the app was created.</span></span> <span data-ttu-id="eebcb-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eebcb-153">lastModifiedDateTime</span></span>|<span data-ttu-id="eebcb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eebcb-154">DateTimeOffset</span></span>|<span data-ttu-id="eebcb-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="eebcb-155">The date and time the app was last modified.</span></span> <span data-ttu-id="eebcb-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eebcb-157">isFeatured</span></span>|<span data-ttu-id="eebcb-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="eebcb-158">Boolean</span></span>|<span data-ttu-id="eebcb-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eebcb-160">privacyInformationUrl</span></span>|<span data-ttu-id="eebcb-161">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-161">String</span></span>|<span data-ttu-id="eebcb-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="eebcb-162">The privacy statement Url.</span></span> <span data-ttu-id="eebcb-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eebcb-164">informationUrl</span></span>|<span data-ttu-id="eebcb-165">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-165">String</span></span>|<span data-ttu-id="eebcb-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="eebcb-166">The more information Url.</span></span> <span data-ttu-id="eebcb-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-168">owner</span><span class="sxs-lookup"><span data-stu-id="eebcb-168">owner</span></span>|<span data-ttu-id="eebcb-169">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-169">String</span></span>|<span data-ttu-id="eebcb-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="eebcb-170">The owner of the app.</span></span> <span data-ttu-id="eebcb-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-172">developer</span><span class="sxs-lookup"><span data-stu-id="eebcb-172">developer</span></span>|<span data-ttu-id="eebcb-173">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-173">String</span></span>|<span data-ttu-id="eebcb-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="eebcb-174">The developer of the app.</span></span> <span data-ttu-id="eebcb-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-176">notes</span><span class="sxs-lookup"><span data-stu-id="eebcb-176">notes</span></span>|<span data-ttu-id="eebcb-177">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-177">String</span></span>|<span data-ttu-id="eebcb-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="eebcb-178">Notes for the app.</span></span> <span data-ttu-id="eebcb-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eebcb-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eebcb-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="eebcb-180">publishingState</span></span>|[<span data-ttu-id="eebcb-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="eebcb-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="eebcb-182">アプリの発行状態。</span><span class="sxs-lookup"><span data-stu-id="eebcb-182">The publishing state for the app.</span></span> <span data-ttu-id="eebcb-183">アプリが発行されていないと、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="eebcb-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eebcb-184">[MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="eebcb-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="eebcb-185">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="eebcb-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eebcb-186">packageId</span><span class="sxs-lookup"><span data-stu-id="eebcb-186">packageId</span></span>|<span data-ttu-id="eebcb-187">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-187">String</span></span>|<span data-ttu-id="eebcb-188">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="eebcb-188">The package identifier.</span></span>|
|<span data-ttu-id="eebcb-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="eebcb-189">appStoreUrl</span></span>|<span data-ttu-id="eebcb-190">String</span><span class="sxs-lookup"><span data-stu-id="eebcb-190">String</span></span>|<span data-ttu-id="eebcb-191">Android アプリ ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="eebcb-191">The Android app store URL.</span></span>|
|<span data-ttu-id="eebcb-192">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eebcb-192">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="eebcb-193">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eebcb-193">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="eebcb-194">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="eebcb-194">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="eebcb-195">応答</span><span class="sxs-lookup"><span data-stu-id="eebcb-195">Response</span></span>
<span data-ttu-id="eebcb-196">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidStoreApp](../resources/intune_apps_androidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eebcb-196">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eebcb-197">例</span><span class="sxs-lookup"><span data-stu-id="eebcb-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="eebcb-198">要求</span><span class="sxs-lookup"><span data-stu-id="eebcb-198">Request</span></span>
<span data-ttu-id="eebcb-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eebcb-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="eebcb-200">応答</span><span class="sxs-lookup"><span data-stu-id="eebcb-200">Response</span></span>
<span data-ttu-id="eebcb-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eebcb-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```



