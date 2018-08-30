# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="0bbcf-101">managedAndroidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="0bbcf-101">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="0bbcf-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bbcf-103">新しい [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-103">Create a new [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bbcf-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="0bbcf-104">Prerequisites</span></span>
<span data-ttu-id="0bbcf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0bbcf-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0bbcf-107">Permission type</span></span>|<span data-ttu-id="0bbcf-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0bbcf-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bbcf-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0bbcf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0bbcf-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bbcf-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0bbcf-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0bbcf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bbcf-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-112">Not supported.</span></span>|
|<span data-ttu-id="0bbcf-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0bbcf-113">Application</span></span>|<span data-ttu-id="0bbcf-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bbcf-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0bbcf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0bbcf-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bbcf-116">Request headers</span></span>
|<span data-ttu-id="0bbcf-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bbcf-117">Header</span></span>|<span data-ttu-id="0bbcf-118">値</span><span class="sxs-lookup"><span data-stu-id="0bbcf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bbcf-119">承認</span><span class="sxs-lookup"><span data-stu-id="0bbcf-119">Authorization</span></span>|<span data-ttu-id="0bbcf-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bbcf-121">承諾</span><span class="sxs-lookup"><span data-stu-id="0bbcf-121">Accept</span></span>|<span data-ttu-id="0bbcf-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="0bbcf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bbcf-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0bbcf-123">Request body</span></span>
<span data-ttu-id="0bbcf-124">要求本文で、managedAndroidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-124">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="0bbcf-125">次の表に、managedAndroidStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-125">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="0bbcf-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bbcf-126">Property</span></span>|<span data-ttu-id="0bbcf-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="0bbcf-127">Type</span></span>|<span data-ttu-id="0bbcf-128">説明</span><span class="sxs-lookup"><span data-stu-id="0bbcf-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bbcf-129">ID</span><span class="sxs-lookup"><span data-stu-id="0bbcf-129">id</span></span>|<span data-ttu-id="0bbcf-130">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-130">String</span></span>|<span data-ttu-id="0bbcf-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-131">Key of the entity.</span></span> <span data-ttu-id="0bbcf-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0bbcf-133">displayName</span></span>|<span data-ttu-id="0bbcf-134">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-134">String</span></span>|<span data-ttu-id="0bbcf-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0bbcf-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-137">説明</span><span class="sxs-lookup"><span data-stu-id="0bbcf-137">description</span></span>|<span data-ttu-id="0bbcf-138">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-138">String</span></span>|<span data-ttu-id="0bbcf-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-139">The description of the app.</span></span> <span data-ttu-id="0bbcf-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-141">パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="0bbcf-141">publisher</span></span>|<span data-ttu-id="0bbcf-142">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-142">String</span></span>|<span data-ttu-id="0bbcf-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-143">The publisher of the app.</span></span> <span data-ttu-id="0bbcf-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0bbcf-145">largeIcon</span></span>|[<span data-ttu-id="0bbcf-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0bbcf-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="0bbcf-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0bbcf-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bbcf-149">createdDateTime</span></span>|<span data-ttu-id="0bbcf-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bbcf-150">DateTimeOffset</span></span>|<span data-ttu-id="0bbcf-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-151">The date and time the app was created.</span></span> <span data-ttu-id="0bbcf-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bbcf-153">lastModifiedDateTime</span></span>|<span data-ttu-id="0bbcf-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bbcf-154">DateTimeOffset</span></span>|<span data-ttu-id="0bbcf-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-155">The date and time the app was last modified.</span></span> <span data-ttu-id="0bbcf-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0bbcf-157">isFeatured</span></span>|<span data-ttu-id="0bbcf-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="0bbcf-158">Boolean</span></span>|<span data-ttu-id="0bbcf-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0bbcf-160">privacyInformationUrl</span></span>|<span data-ttu-id="0bbcf-161">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-161">String</span></span>|<span data-ttu-id="0bbcf-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-162">The privacy statement Url.</span></span> <span data-ttu-id="0bbcf-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0bbcf-164">informationUrl</span></span>|<span data-ttu-id="0bbcf-165">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-165">String</span></span>|<span data-ttu-id="0bbcf-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-166">The more information Url.</span></span> <span data-ttu-id="0bbcf-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-168">所有者</span><span class="sxs-lookup"><span data-stu-id="0bbcf-168">owner</span></span>|<span data-ttu-id="0bbcf-169">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-169">String</span></span>|<span data-ttu-id="0bbcf-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-170">The owner of the app.</span></span> <span data-ttu-id="0bbcf-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-172">開発者</span><span class="sxs-lookup"><span data-stu-id="0bbcf-172">developer</span></span>|<span data-ttu-id="0bbcf-173">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-173">String</span></span>|<span data-ttu-id="0bbcf-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-174">The developer of the app.</span></span> <span data-ttu-id="0bbcf-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-176">メモ</span><span class="sxs-lookup"><span data-stu-id="0bbcf-176">notes</span></span>|<span data-ttu-id="0bbcf-177">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-177">String</span></span>|<span data-ttu-id="0bbcf-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-178">Notes for the app.</span></span> <span data-ttu-id="0bbcf-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0bbcf-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="0bbcf-180">publishingState</span></span>|[<span data-ttu-id="0bbcf-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0bbcf-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="0bbcf-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-182">The publishing state for the app.</span></span> <span data-ttu-id="0bbcf-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0bbcf-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="0bbcf-185">指定できる値は、`notPublished`、`processing`、`published`です。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-185">The possible values are `notPublished`, `processing`, or `published`.</span></span>|
|<span data-ttu-id="0bbcf-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="0bbcf-186">appAvailability</span></span>|[<span data-ttu-id="0bbcf-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="0bbcf-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="0bbcf-188">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-188">The Application's availability.</span></span> <span data-ttu-id="0bbcf-189">[managedApp](../resources/intune_apps_managedapp.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="0bbcf-190">指定できる値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-190">The possible values are:</span></span>|
|<span data-ttu-id="0bbcf-191">バージョン</span><span class="sxs-lookup"><span data-stu-id="0bbcf-191">version</span></span>|<span data-ttu-id="0bbcf-192">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-192">String</span></span>|<span data-ttu-id="0bbcf-193">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-193">The Application's version.</span></span> <span data-ttu-id="0bbcf-194">[managedApp](../resources/intune_apps_managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bbcf-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="0bbcf-195">packageId</span><span class="sxs-lookup"><span data-stu-id="0bbcf-195">packageId</span></span>|<span data-ttu-id="0bbcf-196">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-196">String</span></span>|<span data-ttu-id="0bbcf-197">アプリのパッケージ ID。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-197">The app's package ID.</span></span>|
|<span data-ttu-id="0bbcf-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0bbcf-198">appStoreUrl</span></span>|<span data-ttu-id="0bbcf-199">文字列</span><span class="sxs-lookup"><span data-stu-id="0bbcf-199">String</span></span>|<span data-ttu-id="0bbcf-200">Android の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-200">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="0bbcf-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0bbcf-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0bbcf-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0bbcf-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="0bbcf-203">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-203">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="0bbcf-204">応答</span><span class="sxs-lookup"><span data-stu-id="0bbcf-204">Response</span></span>
<span data-ttu-id="0bbcf-205">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-205">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bbcf-206">例</span><span class="sxs-lookup"><span data-stu-id="0bbcf-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bbcf-207">要求</span><span class="sxs-lookup"><span data-stu-id="0bbcf-207">Request</span></span>
<span data-ttu-id="0bbcf-208">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-208">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0bbcf-209">応答</span><span class="sxs-lookup"><span data-stu-id="0bbcf-209">Response</span></span>
<span data-ttu-id="0bbcf-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0bbcf-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



