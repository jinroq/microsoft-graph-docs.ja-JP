# <a name="update-managediosstoreapp"></a><span data-ttu-id="51574-101">managedIOSStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="51574-101">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="51574-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="51574-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51574-103">[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="51574-103">Update the properties of a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51574-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="51574-104">Prerequisites</span></span>
<span data-ttu-id="51574-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51574-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51574-107">Permission type</span></span>|<span data-ttu-id="51574-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="51574-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51574-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51574-109">Delegated (work or school account)</span></span>|<span data-ttu-id="51574-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51574-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51574-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51574-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51574-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51574-112">Not supported.</span></span>|
|<span data-ttu-id="51574-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51574-113">Application</span></span>|<span data-ttu-id="51574-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51574-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51574-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51574-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="51574-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51574-116">Request headers</span></span>
|<span data-ttu-id="51574-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51574-117">Header</span></span>|<span data-ttu-id="51574-118">値</span><span class="sxs-lookup"><span data-stu-id="51574-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51574-119">承認</span><span class="sxs-lookup"><span data-stu-id="51574-119">Authorization</span></span>|<span data-ttu-id="51574-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="51574-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51574-121">承諾</span><span class="sxs-lookup"><span data-stu-id="51574-121">Accept</span></span>|<span data-ttu-id="51574-122">application/json</span><span class="sxs-lookup"><span data-stu-id="51574-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51574-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="51574-123">Request body</span></span>
<span data-ttu-id="51574-124">要求本文で、[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="51574-124">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>

<span data-ttu-id="51574-125">次の表に、[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="51574-125">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span></span>

|<span data-ttu-id="51574-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51574-126">Property</span></span>|<span data-ttu-id="51574-127">型</span><span class="sxs-lookup"><span data-stu-id="51574-127">Type</span></span>|<span data-ttu-id="51574-128">説明</span><span class="sxs-lookup"><span data-stu-id="51574-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51574-129">id</span><span class="sxs-lookup"><span data-stu-id="51574-129">id</span></span>|<span data-ttu-id="51574-130">String</span><span class="sxs-lookup"><span data-stu-id="51574-130">String</span></span>|<span data-ttu-id="51574-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="51574-131">Key of the entity.</span></span> <span data-ttu-id="51574-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-133">displayName</span><span class="sxs-lookup"><span data-stu-id="51574-133">displayName</span></span>|<span data-ttu-id="51574-134">String</span><span class="sxs-lookup"><span data-stu-id="51574-134">String</span></span>|<span data-ttu-id="51574-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="51574-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="51574-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-137">description</span><span class="sxs-lookup"><span data-stu-id="51574-137">description</span></span>|<span data-ttu-id="51574-138">String</span><span class="sxs-lookup"><span data-stu-id="51574-138">String</span></span>|<span data-ttu-id="51574-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="51574-139">The description of the app.</span></span> <span data-ttu-id="51574-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-141">publisher</span><span class="sxs-lookup"><span data-stu-id="51574-141">publisher</span></span>|<span data-ttu-id="51574-142">String</span><span class="sxs-lookup"><span data-stu-id="51574-142">String</span></span>|<span data-ttu-id="51574-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="51574-143">The publisher of the app.</span></span> <span data-ttu-id="51574-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="51574-145">largeIcon</span></span>|[<span data-ttu-id="51574-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="51574-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="51574-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="51574-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="51574-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51574-149">createdDateTime</span></span>|<span data-ttu-id="51574-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51574-150">DateTimeOffset</span></span>|<span data-ttu-id="51574-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="51574-151">The date and time the app was created.</span></span> <span data-ttu-id="51574-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51574-153">lastModifiedDateTime</span></span>|<span data-ttu-id="51574-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51574-154">DateTimeOffset</span></span>|<span data-ttu-id="51574-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="51574-155">The date and time the app was last modified.</span></span> <span data-ttu-id="51574-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="51574-157">isFeatured</span></span>|<span data-ttu-id="51574-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="51574-158">Boolean</span></span>|<span data-ttu-id="51574-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="51574-160">privacyInformationUrl</span></span>|<span data-ttu-id="51574-161">String</span><span class="sxs-lookup"><span data-stu-id="51574-161">String</span></span>|<span data-ttu-id="51574-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="51574-162">The privacy statement Url.</span></span> <span data-ttu-id="51574-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="51574-164">informationUrl</span></span>|<span data-ttu-id="51574-165">String</span><span class="sxs-lookup"><span data-stu-id="51574-165">String</span></span>|<span data-ttu-id="51574-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="51574-166">The more information Url.</span></span> <span data-ttu-id="51574-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-168">owner</span><span class="sxs-lookup"><span data-stu-id="51574-168">owner</span></span>|<span data-ttu-id="51574-169">String</span><span class="sxs-lookup"><span data-stu-id="51574-169">String</span></span>|<span data-ttu-id="51574-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="51574-170">The owner of the app.</span></span> <span data-ttu-id="51574-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-172">developer</span><span class="sxs-lookup"><span data-stu-id="51574-172">developer</span></span>|<span data-ttu-id="51574-173">String</span><span class="sxs-lookup"><span data-stu-id="51574-173">String</span></span>|<span data-ttu-id="51574-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="51574-174">The developer of the app.</span></span> <span data-ttu-id="51574-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-176">notes</span><span class="sxs-lookup"><span data-stu-id="51574-176">notes</span></span>|<span data-ttu-id="51574-177">String</span><span class="sxs-lookup"><span data-stu-id="51574-177">String</span></span>|<span data-ttu-id="51574-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="51574-178">Notes for the app.</span></span> <span data-ttu-id="51574-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="51574-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="51574-180">publishingState</span></span>|[<span data-ttu-id="51574-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="51574-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="51574-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="51574-182">The publishing state for the app.</span></span> <span data-ttu-id="51574-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="51574-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="51574-184">[MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="51574-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="51574-185">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="51574-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="51574-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="51574-186">appAvailability</span></span>|[<span data-ttu-id="51574-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="51574-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="51574-188">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="51574-188">The Application's availability.</span></span> <span data-ttu-id="51574-189">[ManagedApp](../resources/intune_apps_managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="51574-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="51574-190">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="51574-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="51574-191">version</span><span class="sxs-lookup"><span data-stu-id="51574-191">version</span></span>|<span data-ttu-id="51574-192">String</span><span class="sxs-lookup"><span data-stu-id="51574-192">String</span></span>|<span data-ttu-id="51574-193">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="51574-193">The Application's version.</span></span> <span data-ttu-id="51574-194">[managedApp](../resources/intune_apps_managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51574-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="51574-195">bundleId</span><span class="sxs-lookup"><span data-stu-id="51574-195">bundleId</span></span>|<span data-ttu-id="51574-196">String</span><span class="sxs-lookup"><span data-stu-id="51574-196">String</span></span>|<span data-ttu-id="51574-197">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="51574-197">The app's Bundle ID.</span></span>|
|<span data-ttu-id="51574-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="51574-198">appStoreUrl</span></span>|<span data-ttu-id="51574-199">String</span><span class="sxs-lookup"><span data-stu-id="51574-199">String</span></span>|<span data-ttu-id="51574-200">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="51574-200">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="51574-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="51574-201">applicableDeviceType</span></span>|[<span data-ttu-id="51574-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="51574-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="51574-203">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="51574-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="51574-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51574-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="51574-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51574-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="51574-206">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="51574-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="51574-207">応答</span><span class="sxs-lookup"><span data-stu-id="51574-207">Response</span></span>
<span data-ttu-id="51574-208">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="51574-208">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51574-209">例</span><span class="sxs-lookup"><span data-stu-id="51574-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="51574-210">要求</span><span class="sxs-lookup"><span data-stu-id="51574-210">Request</span></span>
<span data-ttu-id="51574-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51574-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1084

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
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="51574-212">応答</span><span class="sxs-lookup"><span data-stu-id="51574-212">Response</span></span>
<span data-ttu-id="51574-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51574-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1256

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
    "v11_0": true,
    "v12_0": true
  }
}
```



