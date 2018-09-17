# <a name="update-iosstoreapp"></a><span data-ttu-id="2047c-101">iosStoreApp を更新する</span><span class="sxs-lookup"><span data-stu-id="2047c-101">Update iosStoreApp</span></span>

> <span data-ttu-id="2047c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2047c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2047c-103">[iosStoreApp](../resources/intune_apps_iosstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2047c-103">Update the properties of a [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2047c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2047c-104">Prerequisites</span></span>
<span data-ttu-id="2047c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2047c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2047c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2047c-107">Permission type</span></span>|<span data-ttu-id="2047c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2047c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2047c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2047c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2047c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2047c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2047c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2047c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2047c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2047c-112">Not supported.</span></span>|
|<span data-ttu-id="2047c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2047c-113">Application</span></span>|<span data-ttu-id="2047c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2047c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2047c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2047c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2047c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2047c-116">Request headers</span></span>
|<span data-ttu-id="2047c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2047c-117">Header</span></span>|<span data-ttu-id="2047c-118">値</span><span class="sxs-lookup"><span data-stu-id="2047c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2047c-119">承認</span><span class="sxs-lookup"><span data-stu-id="2047c-119">Authorization</span></span>|<span data-ttu-id="2047c-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2047c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2047c-121">承諾</span><span class="sxs-lookup"><span data-stu-id="2047c-121">Accept</span></span>|<span data-ttu-id="2047c-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="2047c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2047c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2047c-123">Request body</span></span>
<span data-ttu-id="2047c-124">要求本文で、[iosStoreApp](../resources/intune_apps_iosstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2047c-124">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object.</span></span>

<span data-ttu-id="2047c-125">次の表に、[iosStoreApp](../resources/intune_apps_iosstoreapp.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2047c-125">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span></span>

|<span data-ttu-id="2047c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2047c-126">Property</span></span>|<span data-ttu-id="2047c-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="2047c-127">Type</span></span>|<span data-ttu-id="2047c-128">説明</span><span class="sxs-lookup"><span data-stu-id="2047c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2047c-129">id</span><span class="sxs-lookup"><span data-stu-id="2047c-129">id</span></span>|<span data-ttu-id="2047c-130">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-130">String</span></span>|<span data-ttu-id="2047c-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2047c-131">Key of the entity.</span></span> <span data-ttu-id="2047c-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2047c-133">displayName</span></span>|<span data-ttu-id="2047c-134">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-134">String</span></span>|<span data-ttu-id="2047c-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="2047c-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2047c-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-137">description</span><span class="sxs-lookup"><span data-stu-id="2047c-137">description</span></span>|<span data-ttu-id="2047c-138">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-138">String</span></span>|<span data-ttu-id="2047c-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="2047c-139">The description of the app.</span></span> <span data-ttu-id="2047c-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-141">パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="2047c-141">publisher</span></span>|<span data-ttu-id="2047c-142">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-142">String</span></span>|<span data-ttu-id="2047c-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="2047c-143">The publisher of the app.</span></span> <span data-ttu-id="2047c-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2047c-145">largeIcon</span></span>|[<span data-ttu-id="2047c-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2047c-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="2047c-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="2047c-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2047c-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2047c-149">createdDateTime</span></span>|<span data-ttu-id="2047c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2047c-150">DateTimeOffset</span></span>|<span data-ttu-id="2047c-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="2047c-151">The date and time the app was created.</span></span> <span data-ttu-id="2047c-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2047c-153">lastModifiedDateTime</span></span>|<span data-ttu-id="2047c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2047c-154">DateTimeOffset</span></span>|<span data-ttu-id="2047c-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="2047c-155">The date and time the app was last modified.</span></span> <span data-ttu-id="2047c-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2047c-157">isFeatured</span></span>|<span data-ttu-id="2047c-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="2047c-158">Boolean</span></span>|<span data-ttu-id="2047c-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2047c-160">privacyInformationUrl</span></span>|<span data-ttu-id="2047c-161">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-161">String</span></span>|<span data-ttu-id="2047c-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="2047c-162">The privacy statement Url.</span></span> <span data-ttu-id="2047c-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2047c-164">informationUrl</span></span>|<span data-ttu-id="2047c-165">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-165">String</span></span>|<span data-ttu-id="2047c-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="2047c-166">The more information Url.</span></span> <span data-ttu-id="2047c-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-168">所有者</span><span class="sxs-lookup"><span data-stu-id="2047c-168">owner</span></span>|<span data-ttu-id="2047c-169">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-169">String</span></span>|<span data-ttu-id="2047c-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="2047c-170">The owner of the app.</span></span> <span data-ttu-id="2047c-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-172">開発者</span><span class="sxs-lookup"><span data-stu-id="2047c-172">developer</span></span>|<span data-ttu-id="2047c-173">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-173">String</span></span>|<span data-ttu-id="2047c-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="2047c-174">The developer of the app.</span></span> <span data-ttu-id="2047c-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-176">メモ</span><span class="sxs-lookup"><span data-stu-id="2047c-176">notes</span></span>|<span data-ttu-id="2047c-177">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-177">String</span></span>|<span data-ttu-id="2047c-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="2047c-178">Notes for the app.</span></span> <span data-ttu-id="2047c-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2047c-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2047c-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="2047c-180">publishingState</span></span>|[<span data-ttu-id="2047c-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2047c-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="2047c-p114">アプリケーションの発行の状態です。アプリが公開されていない限り、アプリケーションを割り当てることができません。[mobileApp](../resources/intune_apps_mobileapp.md) から継承されます。使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="2047c-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2047c-186">bundleId</span><span class="sxs-lookup"><span data-stu-id="2047c-186">bundleId</span></span>|<span data-ttu-id="2047c-187">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-187">String</span></span>|<span data-ttu-id="2047c-188">ID 名。</span><span class="sxs-lookup"><span data-stu-id="2047c-188">The Identity Name.</span></span>|
|<span data-ttu-id="2047c-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2047c-189">appStoreUrl</span></span>|<span data-ttu-id="2047c-190">文字列</span><span class="sxs-lookup"><span data-stu-id="2047c-190">String</span></span>|<span data-ttu-id="2047c-191">Apple App Store の URL。</span><span class="sxs-lookup"><span data-stu-id="2047c-191">The Apple App Store URL</span></span>|
|<span data-ttu-id="2047c-192">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2047c-192">applicableDeviceType</span></span>|[<span data-ttu-id="2047c-193">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2047c-193">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="2047c-194">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="2047c-194">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="2047c-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2047c-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2047c-196">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2047c-196">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="2047c-197">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="2047c-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="2047c-198">応答</span><span class="sxs-lookup"><span data-stu-id="2047c-198">Response</span></span>
<span data-ttu-id="2047c-199">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosStoreApp](../resources/intune_apps_iosstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="2047c-199">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2047c-200">例</span><span class="sxs-lookup"><span data-stu-id="2047c-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="2047c-201">要求</span><span class="sxs-lookup"><span data-stu-id="2047c-201">Request</span></span>
<span data-ttu-id="2047c-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2047c-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1000

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

### <a name="response"></a><span data-ttu-id="2047c-203">応答</span><span class="sxs-lookup"><span data-stu-id="2047c-203">Response</span></span>
<span data-ttu-id="2047c-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2047c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1158

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
    "v11_0": true
  }
}
```








