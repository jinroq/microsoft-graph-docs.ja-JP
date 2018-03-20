# <a name="create-androidstoreapp"></a><span data-ttu-id="fd7df-101">androidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="fd7df-101">Create androidStoreApp</span></span>

> <span data-ttu-id="fd7df-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd7df-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd7df-103">新しい [androidStoreApp](../resources/intune_apps_androidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fd7df-103">Create a new [plannerBucket](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd7df-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="fd7df-104">Prerequisites</span></span>
<span data-ttu-id="fd7df-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd7df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd7df-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd7df-107">Permission type</span></span>|<span data-ttu-id="fd7df-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd7df-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd7df-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd7df-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fd7df-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd7df-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fd7df-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd7df-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd7df-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd7df-112">Not supported.</span></span>|
|<span data-ttu-id="fd7df-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd7df-113">Application</span></span>|<span data-ttu-id="fd7df-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd7df-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd7df-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd7df-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fd7df-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd7df-116">Request headers</span></span>
|<span data-ttu-id="fd7df-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd7df-117">Header</span></span>|<span data-ttu-id="fd7df-118">値</span><span class="sxs-lookup"><span data-stu-id="fd7df-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd7df-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd7df-119">Authorization</span></span>|<span data-ttu-id="fd7df-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fd7df-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fd7df-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fd7df-121">Accept</span></span>|<span data-ttu-id="fd7df-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fd7df-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd7df-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd7df-123">Request body</span></span>
<span data-ttu-id="fd7df-124">要求本文で、androidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd7df-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="fd7df-125">次の表に、androidStoreApp の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fd7df-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="fd7df-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd7df-126">Property</span></span>|<span data-ttu-id="fd7df-127">型</span><span class="sxs-lookup"><span data-stu-id="fd7df-127">Type</span></span>|<span data-ttu-id="fd7df-128">説明</span><span class="sxs-lookup"><span data-stu-id="fd7df-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd7df-129">id</span><span class="sxs-lookup"><span data-stu-id="fd7df-129">id</span></span>|<span data-ttu-id="fd7df-130">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-130">String</span></span>|<span data-ttu-id="fd7df-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fd7df-131">Name of the entity.</span></span> <span data-ttu-id="fd7df-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fd7df-133">displayName</span></span>|<span data-ttu-id="fd7df-134">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-134">String</span></span>|<span data-ttu-id="fd7df-135">管理者が指定またはインポートした、アプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="fd7df-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fd7df-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-137">description</span><span class="sxs-lookup"><span data-stu-id="fd7df-137">description</span></span>|<span data-ttu-id="fd7df-138">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-138">String</span></span>|<span data-ttu-id="fd7df-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="fd7df-139">The description of the app.</span></span> <span data-ttu-id="fd7df-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-141">publisher</span><span class="sxs-lookup"><span data-stu-id="fd7df-141">Publisher</span></span>|<span data-ttu-id="fd7df-142">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-142">String</span></span>|<span data-ttu-id="fd7df-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="fd7df-143">The name of the app.</span></span> <span data-ttu-id="fd7df-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fd7df-145">largeIcon</span></span>|[<span data-ttu-id="fd7df-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fd7df-146">MimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="fd7df-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="fd7df-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fd7df-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd7df-149">createdDateTime</span></span>|<span data-ttu-id="fd7df-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd7df-150">DateTimeOffset</span></span>|<span data-ttu-id="fd7df-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="fd7df-151">The date and time when the page was created.</span></span> <span data-ttu-id="fd7df-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd7df-153">lastModifiedDateTime</span></span>|<span data-ttu-id="fd7df-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd7df-154">DateTimeOffset</span></span>|<span data-ttu-id="fd7df-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="fd7df-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="fd7df-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fd7df-157">isFeatured</span></span>|<span data-ttu-id="fd7df-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd7df-158">Boolean</span></span>|<span data-ttu-id="fd7df-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fd7df-160">privacyInformationUrl</span></span>|<span data-ttu-id="fd7df-161">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-161">String</span></span>|<span data-ttu-id="fd7df-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="fd7df-162">The privacy statement Url.</span></span> <span data-ttu-id="fd7df-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fd7df-164">informationUrl</span></span>|<span data-ttu-id="fd7df-165">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-165">String</span></span>|<span data-ttu-id="fd7df-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="fd7df-166">The more information Url.</span></span> <span data-ttu-id="fd7df-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-168">owner</span><span class="sxs-lookup"><span data-stu-id="fd7df-168">owner</span></span>|<span data-ttu-id="fd7df-169">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-169">String</span></span>|<span data-ttu-id="fd7df-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="fd7df-170">The owner of the timesheet.</span></span> <span data-ttu-id="fd7df-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-172">developer</span><span class="sxs-lookup"><span data-stu-id="fd7df-172">developer</span></span>|<span data-ttu-id="fd7df-173">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-173">String</span></span>|<span data-ttu-id="fd7df-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="fd7df-174">The name of the app.</span></span> <span data-ttu-id="fd7df-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-176">notes</span><span class="sxs-lookup"><span data-stu-id="fd7df-176">notes</span></span>|<span data-ttu-id="fd7df-177">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-177">String</span></span>|<span data-ttu-id="fd7df-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="fd7df-178">Notes for the app.</span></span> <span data-ttu-id="fd7df-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd7df-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fd7df-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="fd7df-180">publishingState</span></span>|<span data-ttu-id="fd7df-181">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-181">String</span></span>|<span data-ttu-id="fd7df-182">アプリの発行状態。</span><span class="sxs-lookup"><span data-stu-id="fd7df-182">The publishing state for the app.</span></span> <span data-ttu-id="fd7df-183">アプリが発行されていないと、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="fd7df-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fd7df-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="fd7df-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fd7df-185">packageId</span><span class="sxs-lookup"><span data-stu-id="fd7df-185">PackageId</span></span>|<span data-ttu-id="fd7df-186">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-186">String</span></span>|<span data-ttu-id="fd7df-187">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="fd7df-187">The package identifier.</span></span>|
|<span data-ttu-id="fd7df-188">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="fd7df-188">appStoreUrl</span></span>|<span data-ttu-id="fd7df-189">String</span><span class="sxs-lookup"><span data-stu-id="fd7df-189">String</span></span>|<span data-ttu-id="fd7df-190">Android アプリ ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="fd7df-190">The Android app store URL.</span></span>|
|<span data-ttu-id="fd7df-191">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fd7df-191">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fd7df-192">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fd7df-192">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="fd7df-193">適用可能なオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="fd7df-193">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="fd7df-194">応答</span><span class="sxs-lookup"><span data-stu-id="fd7df-194">Response</span></span>
<span data-ttu-id="fd7df-195">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidStoreApp](../resources/intune_apps_androidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fd7df-195">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd7df-196">例</span><span class="sxs-lookup"><span data-stu-id="fd7df-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd7df-197">要求</span><span class="sxs-lookup"><span data-stu-id="fd7df-197">Request</span></span>
<span data-ttu-id="fd7df-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fd7df-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fd7df-199">応答</span><span class="sxs-lookup"><span data-stu-id="fd7df-199">Response</span></span>
<span data-ttu-id="fd7df-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fd7df-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



