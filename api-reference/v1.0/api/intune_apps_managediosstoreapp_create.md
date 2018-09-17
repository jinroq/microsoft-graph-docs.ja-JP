# <a name="create-managediosstoreapp"></a><span data-ttu-id="128d8-101">managedIOSStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="128d8-101">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="128d8-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="128d8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="128d8-103">新しい [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="128d8-103">Create a new [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="128d8-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="128d8-104">Prerequisites</span></span>
<span data-ttu-id="128d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="128d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="128d8-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="128d8-107">Permission type</span></span>|<span data-ttu-id="128d8-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="128d8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="128d8-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="128d8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="128d8-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="128d8-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="128d8-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="128d8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="128d8-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="128d8-112">Not supported.</span></span>|
|<span data-ttu-id="128d8-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="128d8-113">Application</span></span>|<span data-ttu-id="128d8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="128d8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="128d8-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="128d8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="128d8-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="128d8-116">Request headers</span></span>
|<span data-ttu-id="128d8-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="128d8-117">Header</span></span>|<span data-ttu-id="128d8-118">値</span><span class="sxs-lookup"><span data-stu-id="128d8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="128d8-119">承認</span><span class="sxs-lookup"><span data-stu-id="128d8-119">Authorization</span></span>|<span data-ttu-id="128d8-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="128d8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="128d8-121">承諾</span><span class="sxs-lookup"><span data-stu-id="128d8-121">Accept</span></span>|<span data-ttu-id="128d8-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="128d8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="128d8-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="128d8-123">Request body</span></span>
<span data-ttu-id="128d8-124">要求本文で、managedIOSStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="128d8-124">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="128d8-125">次の表に、managedIOSStoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="128d8-125">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="128d8-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="128d8-126">Property</span></span>|<span data-ttu-id="128d8-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="128d8-127">Type</span></span>|<span data-ttu-id="128d8-128">説明</span><span class="sxs-lookup"><span data-stu-id="128d8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="128d8-129">id</span><span class="sxs-lookup"><span data-stu-id="128d8-129">id</span></span>|<span data-ttu-id="128d8-130">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-130">String</span></span>|<span data-ttu-id="128d8-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="128d8-131">Key of the entity.</span></span> <span data-ttu-id="128d8-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="128d8-133">displayName</span></span>|<span data-ttu-id="128d8-134">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-134">String</span></span>|<span data-ttu-id="128d8-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="128d8-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="128d8-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-137">description</span><span class="sxs-lookup"><span data-stu-id="128d8-137">description</span></span>|<span data-ttu-id="128d8-138">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-138">String</span></span>|<span data-ttu-id="128d8-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="128d8-139">The description of the app.</span></span> <span data-ttu-id="128d8-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-141">パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="128d8-141">publisher</span></span>|<span data-ttu-id="128d8-142">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-142">String</span></span>|<span data-ttu-id="128d8-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="128d8-143">The publisher of the app.</span></span> <span data-ttu-id="128d8-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="128d8-145">largeIcon</span></span>|[<span data-ttu-id="128d8-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="128d8-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="128d8-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="128d8-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="128d8-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="128d8-149">createdDateTime</span></span>|<span data-ttu-id="128d8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="128d8-150">DateTimeOffset</span></span>|<span data-ttu-id="128d8-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="128d8-151">The date and time the app was created.</span></span> <span data-ttu-id="128d8-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="128d8-153">lastModifiedDateTime</span></span>|<span data-ttu-id="128d8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="128d8-154">DateTimeOffset</span></span>|<span data-ttu-id="128d8-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="128d8-155">The date and time the app was last modified.</span></span> <span data-ttu-id="128d8-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="128d8-157">isFeatured</span></span>|<span data-ttu-id="128d8-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="128d8-158">Boolean</span></span>|<span data-ttu-id="128d8-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="128d8-160">privacyInformationUrl</span></span>|<span data-ttu-id="128d8-161">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-161">String</span></span>|<span data-ttu-id="128d8-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="128d8-162">The privacy statement Url.</span></span> <span data-ttu-id="128d8-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="128d8-164">informationUrl</span></span>|<span data-ttu-id="128d8-165">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-165">String</span></span>|<span data-ttu-id="128d8-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="128d8-166">The more information Url.</span></span> <span data-ttu-id="128d8-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-168">所有者</span><span class="sxs-lookup"><span data-stu-id="128d8-168">owner</span></span>|<span data-ttu-id="128d8-169">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-169">String</span></span>|<span data-ttu-id="128d8-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="128d8-170">The owner of the app.</span></span> <span data-ttu-id="128d8-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-172">開発者</span><span class="sxs-lookup"><span data-stu-id="128d8-172">developer</span></span>|<span data-ttu-id="128d8-173">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-173">String</span></span>|<span data-ttu-id="128d8-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="128d8-174">The developer of the app.</span></span> <span data-ttu-id="128d8-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-176">メモ</span><span class="sxs-lookup"><span data-stu-id="128d8-176">notes</span></span>|<span data-ttu-id="128d8-177">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-177">String</span></span>|<span data-ttu-id="128d8-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="128d8-178">Notes for the app.</span></span> <span data-ttu-id="128d8-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="128d8-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="128d8-180">publishingState</span></span>|[<span data-ttu-id="128d8-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="128d8-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="128d8-p114">アプリケーションの発行の状態です。アプリが公開されていない限り、アプリケーションを割り当てることができません。[mobileApp](../resources/intune_apps_mobileapp.md) から継承されます。使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="128d8-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="128d8-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="128d8-186">appAvailability</span></span>|[<span data-ttu-id="128d8-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="128d8-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="128d8-p115">アプリケーションの可用性です。[managedApp](../resources/intune_apps_managedapp.md) から継承されます。使用可能な値は `global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="128d8-p115">The Application's availability. Inherited from [managedApp](../resources/intune_apps_managedapp.md). The possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="128d8-191">version</span><span class="sxs-lookup"><span data-stu-id="128d8-191">version</span></span>|<span data-ttu-id="128d8-192">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-192">String</span></span>|<span data-ttu-id="128d8-193">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="128d8-193">The Application's version.</span></span> <span data-ttu-id="128d8-194">[managedApp](../resources/intune_apps_managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="128d8-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="128d8-195">bundleId</span><span class="sxs-lookup"><span data-stu-id="128d8-195">bundleId</span></span>|<span data-ttu-id="128d8-196">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-196">String</span></span>|<span data-ttu-id="128d8-197">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="128d8-197">The app's Bundle ID.</span></span>|
|<span data-ttu-id="128d8-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="128d8-198">appStoreUrl</span></span>|<span data-ttu-id="128d8-199">文字列</span><span class="sxs-lookup"><span data-stu-id="128d8-199">String</span></span>|<span data-ttu-id="128d8-200">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="128d8-200">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="128d8-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="128d8-201">applicableDeviceType</span></span>|[<span data-ttu-id="128d8-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="128d8-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="128d8-203">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="128d8-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="128d8-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="128d8-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="128d8-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="128d8-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="128d8-206">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="128d8-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="128d8-207">応答</span><span class="sxs-lookup"><span data-stu-id="128d8-207">Response</span></span>
<span data-ttu-id="128d8-208">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="128d8-208">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="128d8-209">例</span><span class="sxs-lookup"><span data-stu-id="128d8-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="128d8-210">要求</span><span class="sxs-lookup"><span data-stu-id="128d8-210">Request</span></span>
<span data-ttu-id="128d8-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="128d8-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1128

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="128d8-212">応答</span><span class="sxs-lookup"><span data-stu-id="128d8-212">Response</span></span>
<span data-ttu-id="128d8-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="128d8-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1236

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
    "v11_0": true
  }
}
```








