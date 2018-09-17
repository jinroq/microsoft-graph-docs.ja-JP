# <a name="create-androidstoreapp"></a><span data-ttu-id="cd721-101">androidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="cd721-101">Create androidStoreApp</span></span>

> <span data-ttu-id="cd721-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd721-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd721-103">新しい [androidStoreApp](../resources/intune_apps_androidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cd721-103">Create a new [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd721-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="cd721-104">Prerequisites</span></span>
<span data-ttu-id="cd721-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd721-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cd721-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd721-107">Permission type</span></span>|<span data-ttu-id="cd721-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd721-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd721-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd721-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cd721-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd721-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cd721-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd721-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd721-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd721-112">Not supported.</span></span>|
|<span data-ttu-id="cd721-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd721-113">Application</span></span>|<span data-ttu-id="cd721-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd721-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd721-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd721-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cd721-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd721-116">Request headers</span></span>
|<span data-ttu-id="cd721-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd721-117">Header</span></span>|<span data-ttu-id="cd721-118">値</span><span class="sxs-lookup"><span data-stu-id="cd721-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd721-119">承認</span><span class="sxs-lookup"><span data-stu-id="cd721-119">Authorization</span></span>|<span data-ttu-id="cd721-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cd721-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd721-121">承諾</span><span class="sxs-lookup"><span data-stu-id="cd721-121">Accept</span></span>|<span data-ttu-id="cd721-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="cd721-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd721-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd721-123">Request body</span></span>
<span data-ttu-id="cd721-124">要求本文で、androidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cd721-124">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="cd721-125">次の表に、androidStoreApp の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cd721-125">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="cd721-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd721-126">Property</span></span>|<span data-ttu-id="cd721-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="cd721-127">Type</span></span>|<span data-ttu-id="cd721-128">説明</span><span class="sxs-lookup"><span data-stu-id="cd721-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd721-129">ID</span><span class="sxs-lookup"><span data-stu-id="cd721-129">id</span></span>|<span data-ttu-id="cd721-130">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-130">String</span></span>|<span data-ttu-id="cd721-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cd721-131">Key of the entity.</span></span> <span data-ttu-id="cd721-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cd721-133">displayName</span></span>|<span data-ttu-id="cd721-134">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-134">String</span></span>|<span data-ttu-id="cd721-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="cd721-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cd721-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-137">説明</span><span class="sxs-lookup"><span data-stu-id="cd721-137">description</span></span>|<span data-ttu-id="cd721-138">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-138">String</span></span>|<span data-ttu-id="cd721-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="cd721-139">The description of the app.</span></span> <span data-ttu-id="cd721-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-141">パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="cd721-141">publisher</span></span>|<span data-ttu-id="cd721-142">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-142">String</span></span>|<span data-ttu-id="cd721-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="cd721-143">The publisher of the app.</span></span> <span data-ttu-id="cd721-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cd721-145">largeIcon</span></span>|[<span data-ttu-id="cd721-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cd721-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="cd721-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="cd721-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cd721-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd721-149">createdDateTime</span></span>|<span data-ttu-id="cd721-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd721-150">DateTimeOffset</span></span>|<span data-ttu-id="cd721-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="cd721-151">The date and time the app was created.</span></span> <span data-ttu-id="cd721-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd721-153">lastModifiedDateTime</span></span>|<span data-ttu-id="cd721-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd721-154">DateTimeOffset</span></span>|<span data-ttu-id="cd721-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="cd721-155">The date and time the app was last modified.</span></span> <span data-ttu-id="cd721-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cd721-157">isFeatured</span></span>|<span data-ttu-id="cd721-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="cd721-158">Boolean</span></span>|<span data-ttu-id="cd721-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cd721-160">privacyInformationUrl</span></span>|<span data-ttu-id="cd721-161">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-161">String</span></span>|<span data-ttu-id="cd721-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="cd721-162">The privacy statement Url.</span></span> <span data-ttu-id="cd721-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cd721-164">informationUrl</span></span>|<span data-ttu-id="cd721-165">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-165">String</span></span>|<span data-ttu-id="cd721-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="cd721-166">The more information Url.</span></span> <span data-ttu-id="cd721-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-168">所有者</span><span class="sxs-lookup"><span data-stu-id="cd721-168">owner</span></span>|<span data-ttu-id="cd721-169">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-169">String</span></span>|<span data-ttu-id="cd721-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="cd721-170">The owner of the app.</span></span> <span data-ttu-id="cd721-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-172">開発者</span><span class="sxs-lookup"><span data-stu-id="cd721-172">developer</span></span>|<span data-ttu-id="cd721-173">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-173">String</span></span>|<span data-ttu-id="cd721-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="cd721-174">The developer of the app.</span></span> <span data-ttu-id="cd721-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-176">メモ</span><span class="sxs-lookup"><span data-stu-id="cd721-176">notes</span></span>|<span data-ttu-id="cd721-177">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-177">String</span></span>|<span data-ttu-id="cd721-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="cd721-178">Notes for the app.</span></span> <span data-ttu-id="cd721-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cd721-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="cd721-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="cd721-180">publishingState</span></span>|[<span data-ttu-id="cd721-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cd721-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="cd721-p114">アプリケーションの発行の状態です。アプリが公開されていない限り、アプリケーションを割り当てることができません。 [MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。使用可能な値は`notPublished`、`processing`、`published`です。</span><span class="sxs-lookup"><span data-stu-id="cd721-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cd721-186">packageId</span><span class="sxs-lookup"><span data-stu-id="cd721-186">packageId</span></span>|<span data-ttu-id="cd721-187">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-187">String</span></span>|<span data-ttu-id="cd721-188">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="cd721-188">The package identifier.</span></span>|
|<span data-ttu-id="cd721-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cd721-189">appStoreUrl</span></span>|<span data-ttu-id="cd721-190">文字列</span><span class="sxs-lookup"><span data-stu-id="cd721-190">String</span></span>|<span data-ttu-id="cd721-191">Android アプリ ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="cd721-191">The Android app store URL.</span></span>|
|<span data-ttu-id="cd721-192">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cd721-192">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cd721-193">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cd721-193">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="cd721-194">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="cd721-194">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="cd721-195">応答</span><span class="sxs-lookup"><span data-stu-id="cd721-195">Response</span></span>
<span data-ttu-id="cd721-196">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidStoreApp](../resources/intune_apps_androidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cd721-196">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd721-197">例</span><span class="sxs-lookup"><span data-stu-id="cd721-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd721-198">要求</span><span class="sxs-lookup"><span data-stu-id="cd721-198">Request</span></span>
<span data-ttu-id="cd721-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cd721-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1002

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

### <a name="response"></a><span data-ttu-id="cd721-200">応答</span><span class="sxs-lookup"><span data-stu-id="cd721-200">Response</span></span>
<span data-ttu-id="cd721-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cd721-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








