# <a name="update-managediosstoreapp"></a><span data-ttu-id="d30af-101">managedIOSStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="d30af-101">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="d30af-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d30af-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d30af-103">[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d30af-103">Update the properties of a [calendar](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d30af-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="d30af-104">Prerequisites</span></span>
<span data-ttu-id="d30af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d30af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d30af-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d30af-107">Permission type</span></span>|<span data-ttu-id="d30af-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d30af-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d30af-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d30af-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d30af-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d30af-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d30af-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d30af-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d30af-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d30af-112">Not supported.</span></span>|
|<span data-ttu-id="d30af-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d30af-113">Application</span></span>|<span data-ttu-id="d30af-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d30af-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d30af-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d30af-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d30af-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d30af-116">Request headers</span></span>
|<span data-ttu-id="d30af-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d30af-117">Header</span></span>|<span data-ttu-id="d30af-118">値</span><span class="sxs-lookup"><span data-stu-id="d30af-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d30af-119">承認</span><span class="sxs-lookup"><span data-stu-id="d30af-119">Authorization</span></span>|<span data-ttu-id="d30af-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="d30af-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d30af-121">承諾</span><span class="sxs-lookup"><span data-stu-id="d30af-121">Accept</span></span>|<span data-ttu-id="d30af-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d30af-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d30af-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d30af-123">Request body</span></span>
<span data-ttu-id="d30af-124">要求本文で、[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d30af-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_managediosstoreapp.md) object.</span></span>

<span data-ttu-id="d30af-125">次の表に、[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d30af-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d30af-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d30af-126">Property</span></span>|<span data-ttu-id="d30af-127">型</span><span class="sxs-lookup"><span data-stu-id="d30af-127">Type</span></span>|<span data-ttu-id="d30af-128">説明</span><span class="sxs-lookup"><span data-stu-id="d30af-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d30af-129">id</span><span class="sxs-lookup"><span data-stu-id="d30af-129">id</span></span>|<span data-ttu-id="d30af-130">String</span><span class="sxs-lookup"><span data-stu-id="d30af-130">String</span></span>|<span data-ttu-id="d30af-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d30af-131">Name of the entity.</span></span> <span data-ttu-id="d30af-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d30af-133">displayName</span></span>|<span data-ttu-id="d30af-134">String</span><span class="sxs-lookup"><span data-stu-id="d30af-134">String</span></span>|<span data-ttu-id="d30af-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="d30af-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d30af-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-137">description</span><span class="sxs-lookup"><span data-stu-id="d30af-137">description</span></span>|<span data-ttu-id="d30af-138">String</span><span class="sxs-lookup"><span data-stu-id="d30af-138">String</span></span>|<span data-ttu-id="d30af-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="d30af-139">The description of the app.</span></span> <span data-ttu-id="d30af-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-141">publisher</span><span class="sxs-lookup"><span data-stu-id="d30af-141">Publisher</span></span>|<span data-ttu-id="d30af-142">String</span><span class="sxs-lookup"><span data-stu-id="d30af-142">String</span></span>|<span data-ttu-id="d30af-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="d30af-143">The name of the app.</span></span> <span data-ttu-id="d30af-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d30af-145">largeIcon</span></span>|[<span data-ttu-id="d30af-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d30af-146">MimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="d30af-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="d30af-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d30af-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d30af-149">createdDateTime</span></span>|<span data-ttu-id="d30af-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d30af-150">DateTimeOffset</span></span>|<span data-ttu-id="d30af-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d30af-151">The date and time when the page was created.</span></span> <span data-ttu-id="d30af-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d30af-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d30af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d30af-154">DateTimeOffset</span></span>|<span data-ttu-id="d30af-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="d30af-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="d30af-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d30af-157">isFeatured</span></span>|<span data-ttu-id="d30af-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d30af-158">Boolean</span></span>|<span data-ttu-id="d30af-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d30af-160">privacyInformationUrl</span></span>|<span data-ttu-id="d30af-161">String</span><span class="sxs-lookup"><span data-stu-id="d30af-161">String</span></span>|<span data-ttu-id="d30af-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="d30af-162">The privacy statement Url.</span></span> <span data-ttu-id="d30af-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d30af-164">informationUrl</span></span>|<span data-ttu-id="d30af-165">String</span><span class="sxs-lookup"><span data-stu-id="d30af-165">String</span></span>|<span data-ttu-id="d30af-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="d30af-166">The more information Url.</span></span> <span data-ttu-id="d30af-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-168">owner</span><span class="sxs-lookup"><span data-stu-id="d30af-168">owner</span></span>|<span data-ttu-id="d30af-169">String</span><span class="sxs-lookup"><span data-stu-id="d30af-169">String</span></span>|<span data-ttu-id="d30af-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="d30af-170">The owner of the timesheet.</span></span> <span data-ttu-id="d30af-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-172">developer</span><span class="sxs-lookup"><span data-stu-id="d30af-172">developer</span></span>|<span data-ttu-id="d30af-173">String</span><span class="sxs-lookup"><span data-stu-id="d30af-173">String</span></span>|<span data-ttu-id="d30af-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="d30af-174">The name of the app.</span></span> <span data-ttu-id="d30af-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-176">notes</span><span class="sxs-lookup"><span data-stu-id="d30af-176">notes</span></span>|<span data-ttu-id="d30af-177">String</span><span class="sxs-lookup"><span data-stu-id="d30af-177">String</span></span>|<span data-ttu-id="d30af-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="d30af-178">Notes for the app.</span></span> <span data-ttu-id="d30af-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d30af-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="d30af-180">publishingState</span></span>|<span data-ttu-id="d30af-181">String</span><span class="sxs-lookup"><span data-stu-id="d30af-181">String</span></span>|<span data-ttu-id="d30af-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="d30af-182">The publishing state for the app.</span></span> <span data-ttu-id="d30af-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="d30af-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d30af-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="d30af-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d30af-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="d30af-185">appAvailability</span></span>|<span data-ttu-id="d30af-186">String</span><span class="sxs-lookup"><span data-stu-id="d30af-186">String</span></span>|<span data-ttu-id="d30af-187">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="d30af-187">The Application's availability.</span></span> <span data-ttu-id="d30af-188">[managedApp](../resources/intune_apps_managedapp.md) から継承します。可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="d30af-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="d30af-189">version</span><span class="sxs-lookup"><span data-stu-id="d30af-189">version</span></span>|<span data-ttu-id="d30af-190">String</span><span class="sxs-lookup"><span data-stu-id="d30af-190">String</span></span>|<span data-ttu-id="d30af-191">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d30af-191">The Application's version.</span></span> <span data-ttu-id="d30af-192">[managedApp](../resources/intune_apps_managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d30af-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="d30af-193">bundleId</span><span class="sxs-lookup"><span data-stu-id="d30af-193">bundleId</span></span>|<span data-ttu-id="d30af-194">String</span><span class="sxs-lookup"><span data-stu-id="d30af-194">String</span></span>|<span data-ttu-id="d30af-195">アプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="d30af-195">The app's Bundle ID.</span></span>|
|<span data-ttu-id="d30af-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d30af-196">appStoreUrl</span></span>|<span data-ttu-id="d30af-197">String</span><span class="sxs-lookup"><span data-stu-id="d30af-197">String</span></span>|<span data-ttu-id="d30af-198">Apple の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="d30af-198">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="d30af-199">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="d30af-199">applicableDeviceType</span></span>|[<span data-ttu-id="d30af-200">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d30af-200">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="d30af-201">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="d30af-201">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="d30af-202">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d30af-202">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d30af-203">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d30af-203">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="d30af-204">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="d30af-204">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="d30af-205">応答</span><span class="sxs-lookup"><span data-stu-id="d30af-205">Response</span></span>
<span data-ttu-id="d30af-206">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="d30af-206">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d30af-207">例</span><span class="sxs-lookup"><span data-stu-id="d30af-207">Example</span></span>
### <a name="request"></a><span data-ttu-id="d30af-208">要求</span><span class="sxs-lookup"><span data-stu-id="d30af-208">Request</span></span>
<span data-ttu-id="d30af-209">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d30af-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1071

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

### <a name="response"></a><span data-ttu-id="d30af-210">応答</span><span class="sxs-lookup"><span data-stu-id="d30af-210">Response</span></span>
<span data-ttu-id="d30af-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d30af-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



