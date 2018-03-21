# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="7128b-101">managedAndroidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="7128b-101">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="7128b-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7128b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7128b-103">新しい [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7128b-103">Create a new [plannerBucket](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7128b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7128b-104">Prerequisites</span></span>
<span data-ttu-id="7128b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7128b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7128b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7128b-107">Permission type</span></span>|<span data-ttu-id="7128b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7128b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7128b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7128b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7128b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7128b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7128b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7128b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7128b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7128b-112">Not supported.</span></span>|
|<span data-ttu-id="7128b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7128b-113">Application</span></span>|<span data-ttu-id="7128b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7128b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7128b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7128b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7128b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7128b-116">Request headers</span></span>
|<span data-ttu-id="7128b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7128b-117">Header</span></span>|<span data-ttu-id="7128b-118">値</span><span class="sxs-lookup"><span data-stu-id="7128b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7128b-119">承認</span><span class="sxs-lookup"><span data-stu-id="7128b-119">Authorization</span></span>|<span data-ttu-id="7128b-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="7128b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7128b-121">承諾</span><span class="sxs-lookup"><span data-stu-id="7128b-121">Accept</span></span>|<span data-ttu-id="7128b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7128b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7128b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7128b-123">Request body</span></span>
<span data-ttu-id="7128b-124">要求本文で、managedAndroidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7128b-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="7128b-125">次の表に、managedAndroidStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7128b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="7128b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7128b-126">Property</span></span>|<span data-ttu-id="7128b-127">型</span><span class="sxs-lookup"><span data-stu-id="7128b-127">Type</span></span>|<span data-ttu-id="7128b-128">説明</span><span class="sxs-lookup"><span data-stu-id="7128b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7128b-129">id</span><span class="sxs-lookup"><span data-stu-id="7128b-129">id</span></span>|<span data-ttu-id="7128b-130">String</span><span class="sxs-lookup"><span data-stu-id="7128b-130">String</span></span>|<span data-ttu-id="7128b-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7128b-131">Name of the entity.</span></span> <span data-ttu-id="7128b-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7128b-133">displayName</span></span>|<span data-ttu-id="7128b-134">String</span><span class="sxs-lookup"><span data-stu-id="7128b-134">String</span></span>|<span data-ttu-id="7128b-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="7128b-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7128b-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-137">description</span><span class="sxs-lookup"><span data-stu-id="7128b-137">description</span></span>|<span data-ttu-id="7128b-138">String</span><span class="sxs-lookup"><span data-stu-id="7128b-138">String</span></span>|<span data-ttu-id="7128b-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="7128b-139">The description of the app.</span></span> <span data-ttu-id="7128b-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-141">publisher</span><span class="sxs-lookup"><span data-stu-id="7128b-141">Publisher</span></span>|<span data-ttu-id="7128b-142">String</span><span class="sxs-lookup"><span data-stu-id="7128b-142">String</span></span>|<span data-ttu-id="7128b-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="7128b-143">The name of the app.</span></span> <span data-ttu-id="7128b-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7128b-145">largeIcon</span></span>|[<span data-ttu-id="7128b-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7128b-146">MimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="7128b-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="7128b-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7128b-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7128b-149">createdDateTime</span></span>|<span data-ttu-id="7128b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7128b-150">DateTimeOffset</span></span>|<span data-ttu-id="7128b-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7128b-151">The date and time when the page was created.</span></span> <span data-ttu-id="7128b-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7128b-153">lastModifiedDateTime</span></span>|<span data-ttu-id="7128b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7128b-154">DateTimeOffset</span></span>|<span data-ttu-id="7128b-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="7128b-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="7128b-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7128b-157">isFeatured</span></span>|<span data-ttu-id="7128b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="7128b-158">Boolean</span></span>|<span data-ttu-id="7128b-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7128b-160">privacyInformationUrl</span></span>|<span data-ttu-id="7128b-161">String</span><span class="sxs-lookup"><span data-stu-id="7128b-161">String</span></span>|<span data-ttu-id="7128b-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="7128b-162">The privacy statement Url.</span></span> <span data-ttu-id="7128b-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7128b-164">informationUrl</span></span>|<span data-ttu-id="7128b-165">String</span><span class="sxs-lookup"><span data-stu-id="7128b-165">String</span></span>|<span data-ttu-id="7128b-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="7128b-166">The more information Url.</span></span> <span data-ttu-id="7128b-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-168">owner</span><span class="sxs-lookup"><span data-stu-id="7128b-168">owner</span></span>|<span data-ttu-id="7128b-169">String</span><span class="sxs-lookup"><span data-stu-id="7128b-169">String</span></span>|<span data-ttu-id="7128b-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="7128b-170">The owner of the timesheet.</span></span> <span data-ttu-id="7128b-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-172">developer</span><span class="sxs-lookup"><span data-stu-id="7128b-172">developer</span></span>|<span data-ttu-id="7128b-173">String</span><span class="sxs-lookup"><span data-stu-id="7128b-173">String</span></span>|<span data-ttu-id="7128b-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="7128b-174">The name of the app.</span></span> <span data-ttu-id="7128b-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-176">notes</span><span class="sxs-lookup"><span data-stu-id="7128b-176">notes</span></span>|<span data-ttu-id="7128b-177">String</span><span class="sxs-lookup"><span data-stu-id="7128b-177">String</span></span>|<span data-ttu-id="7128b-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="7128b-178">Notes for the app.</span></span> <span data-ttu-id="7128b-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7128b-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="7128b-180">publishingState</span></span>|<span data-ttu-id="7128b-181">String</span><span class="sxs-lookup"><span data-stu-id="7128b-181">String</span></span>|<span data-ttu-id="7128b-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="7128b-182">The publishing state for the app.</span></span> <span data-ttu-id="7128b-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="7128b-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7128b-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="7128b-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7128b-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="7128b-185">appAvailability</span></span>|<span data-ttu-id="7128b-186">String</span><span class="sxs-lookup"><span data-stu-id="7128b-186">String</span></span>|<span data-ttu-id="7128b-187">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="7128b-187">The Application's availability.</span></span> <span data-ttu-id="7128b-188">[managedApp](../resources/intune_apps_managedapp.md) から継承します。可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="7128b-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="7128b-189">version</span><span class="sxs-lookup"><span data-stu-id="7128b-189">version</span></span>|<span data-ttu-id="7128b-190">String</span><span class="sxs-lookup"><span data-stu-id="7128b-190">String</span></span>|<span data-ttu-id="7128b-191">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7128b-191">The Application's version.</span></span> <span data-ttu-id="7128b-192">[managedApp](../resources/intune_apps_managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7128b-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="7128b-193">packageId</span><span class="sxs-lookup"><span data-stu-id="7128b-193">PackageId</span></span>|<span data-ttu-id="7128b-194">String</span><span class="sxs-lookup"><span data-stu-id="7128b-194">String</span></span>|<span data-ttu-id="7128b-195">アプリのパッケージ ID。</span><span class="sxs-lookup"><span data-stu-id="7128b-195">The app's package ID.</span></span>|
|<span data-ttu-id="7128b-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7128b-196">appStoreUrl</span></span>|<span data-ttu-id="7128b-197">String</span><span class="sxs-lookup"><span data-stu-id="7128b-197">String</span></span>|<span data-ttu-id="7128b-198">Android の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="7128b-198">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="7128b-199">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7128b-199">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7128b-200">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7128b-200">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="7128b-201">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="7128b-201">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="7128b-202">応答</span><span class="sxs-lookup"><span data-stu-id="7128b-202">Response</span></span>
<span data-ttu-id="7128b-203">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7128b-203">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7128b-204">例</span><span class="sxs-lookup"><span data-stu-id="7128b-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="7128b-205">要求</span><span class="sxs-lookup"><span data-stu-id="7128b-205">Request</span></span>
<span data-ttu-id="7128b-206">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7128b-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1080

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="7128b-207">応答</span><span class="sxs-lookup"><span data-stu-id="7128b-207">Response</span></span>
<span data-ttu-id="7128b-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7128b-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1188

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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



