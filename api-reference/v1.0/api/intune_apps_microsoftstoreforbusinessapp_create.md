# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="ae2c5-101">microsoftStoreForBusinessApp の作成</span><span class="sxs-lookup"><span data-stu-id="ae2c5-101">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="ae2c5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae2c5-103">新しい [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-103">Create a new [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae2c5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae2c5-104">Prerequisites</span></span>
<span data-ttu-id="ae2c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae2c5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae2c5-107">Permission type</span></span>|<span data-ttu-id="ae2c5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae2c5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae2c5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae2c5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ae2c5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae2c5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae2c5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae2c5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae2c5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-112">Not supported.</span></span>|
|<span data-ttu-id="ae2c5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae2c5-113">Application</span></span>|<span data-ttu-id="ae2c5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae2c5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae2c5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ae2c5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae2c5-116">Request headers</span></span>
|<span data-ttu-id="ae2c5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae2c5-117">Header</span></span>|<span data-ttu-id="ae2c5-118">値</span><span class="sxs-lookup"><span data-stu-id="ae2c5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae2c5-119">承認</span><span class="sxs-lookup"><span data-stu-id="ae2c5-119">Authorization</span></span>|<span data-ttu-id="ae2c5-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae2c5-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ae2c5-121">Accept</span></span>|<span data-ttu-id="ae2c5-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="ae2c5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae2c5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae2c5-123">Request body</span></span>
<span data-ttu-id="ae2c5-124">要求本文で、microsoftStoreForBusinessApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-124">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="ae2c5-125">次の表に、microsoftStoreForBusinessApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-125">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="ae2c5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae2c5-126">Property</span></span>|<span data-ttu-id="ae2c5-127">型</span><span class="sxs-lookup"><span data-stu-id="ae2c5-127">Type</span></span>|<span data-ttu-id="ae2c5-128">説明</span><span class="sxs-lookup"><span data-stu-id="ae2c5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae2c5-129">ID</span><span class="sxs-lookup"><span data-stu-id="ae2c5-129">id</span></span>|<span data-ttu-id="ae2c5-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-130">String</span></span>|<span data-ttu-id="ae2c5-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-131">Key of the entity.</span></span> <span data-ttu-id="ae2c5-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ae2c5-133">displayName</span></span>|<span data-ttu-id="ae2c5-134">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-134">String</span></span>|<span data-ttu-id="ae2c5-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ae2c5-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-137">説明</span><span class="sxs-lookup"><span data-stu-id="ae2c5-137">description</span></span>|<span data-ttu-id="ae2c5-138">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-138">String</span></span>|<span data-ttu-id="ae2c5-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-139">The description of the app.</span></span> <span data-ttu-id="ae2c5-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-141">発行元</span><span class="sxs-lookup"><span data-stu-id="ae2c5-141">publisher</span></span>|<span data-ttu-id="ae2c5-142">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-142">String</span></span>|<span data-ttu-id="ae2c5-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-143">The publisher of the app.</span></span> <span data-ttu-id="ae2c5-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ae2c5-145">largeIcon</span></span>|[<span data-ttu-id="ae2c5-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ae2c5-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="ae2c5-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ae2c5-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae2c5-149">createdDateTime</span></span>|<span data-ttu-id="ae2c5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae2c5-150">DateTimeOffset</span></span>|<span data-ttu-id="ae2c5-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-151">The date and time the app was created.</span></span> <span data-ttu-id="ae2c5-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae2c5-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ae2c5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae2c5-154">DateTimeOffset</span></span>|<span data-ttu-id="ae2c5-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-155">The date and time the app was last modified.</span></span> <span data-ttu-id="ae2c5-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ae2c5-157">isFeatured</span></span>|<span data-ttu-id="ae2c5-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="ae2c5-158">Boolean</span></span>|<span data-ttu-id="ae2c5-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ae2c5-160">privacyInformationUrl</span></span>|<span data-ttu-id="ae2c5-161">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-161">String</span></span>|<span data-ttu-id="ae2c5-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-162">The privacy statement Url.</span></span> <span data-ttu-id="ae2c5-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ae2c5-164">informationUrl</span></span>|<span data-ttu-id="ae2c5-165">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-165">String</span></span>|<span data-ttu-id="ae2c5-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-166">The more information Url.</span></span> <span data-ttu-id="ae2c5-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-168">所有者</span><span class="sxs-lookup"><span data-stu-id="ae2c5-168">owner</span></span>|<span data-ttu-id="ae2c5-169">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-169">String</span></span>|<span data-ttu-id="ae2c5-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-170">The owner of the app.</span></span> <span data-ttu-id="ae2c5-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-172">開発者</span><span class="sxs-lookup"><span data-stu-id="ae2c5-172">developer</span></span>|<span data-ttu-id="ae2c5-173">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-173">String</span></span>|<span data-ttu-id="ae2c5-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-174">The developer of the app.</span></span> <span data-ttu-id="ae2c5-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-176">メモ</span><span class="sxs-lookup"><span data-stu-id="ae2c5-176">notes</span></span>|<span data-ttu-id="ae2c5-177">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-177">String</span></span>|<span data-ttu-id="ae2c5-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-178">Notes for the app.</span></span> <span data-ttu-id="ae2c5-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae2c5-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ae2c5-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ae2c5-180">publishingState</span></span>|[<span data-ttu-id="ae2c5-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ae2c5-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="ae2c5-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-182">The publishing state for the app.</span></span> <span data-ttu-id="ae2c5-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ae2c5-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="ae2c5-185">使用可能な値は`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ae2c5-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ae2c5-186">usedLicenseCount</span></span>|<span data-ttu-id="ae2c5-187">Int32</span><span class="sxs-lookup"><span data-stu-id="ae2c5-187">Int32</span></span>|<span data-ttu-id="ae2c5-188">使用中の、ビジネス向け Microsoft Store ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-188">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="ae2c5-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ae2c5-189">totalLicenseCount</span></span>|<span data-ttu-id="ae2c5-190">Int32</span><span class="sxs-lookup"><span data-stu-id="ae2c5-190">Int32</span></span>|<span data-ttu-id="ae2c5-191">ビジネス向け Microsoft Store ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-191">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="ae2c5-192">productKey</span><span class="sxs-lookup"><span data-stu-id="ae2c5-192">productKey</span></span>|<span data-ttu-id="ae2c5-193">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-193">String</span></span>|<span data-ttu-id="ae2c5-194">アプリのプロダクト キー</span><span class="sxs-lookup"><span data-stu-id="ae2c5-194">The app product key</span></span>|
|<span data-ttu-id="ae2c5-195">licenseType</span><span class="sxs-lookup"><span data-stu-id="ae2c5-195">licenseType</span></span>|[<span data-ttu-id="ae2c5-196">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="ae2c5-196">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune_apps_microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="ae2c5-197">アプリのライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-197">The app license type Possible values are: , .</span></span> <span data-ttu-id="ae2c5-198">使用可能な値は`offline`、`online` です。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-198">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="ae2c5-199">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="ae2c5-199">packageIdentityName</span></span>|<span data-ttu-id="ae2c5-200">文字列</span><span class="sxs-lookup"><span data-stu-id="ae2c5-200">String</span></span>|<span data-ttu-id="ae2c5-201">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="ae2c5-201">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="ae2c5-202">応答</span><span class="sxs-lookup"><span data-stu-id="ae2c5-202">Response</span></span>
<span data-ttu-id="ae2c5-203">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-203">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae2c5-204">例</span><span class="sxs-lookup"><span data-stu-id="ae2c5-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae2c5-205">要求</span><span class="sxs-lookup"><span data-stu-id="ae2c5-205">Request</span></span>
<span data-ttu-id="ae2c5-206">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 833

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="ae2c5-207">応答</span><span class="sxs-lookup"><span data-stu-id="ae2c5-207">Response</span></span>
<span data-ttu-id="ae2c5-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae2c5-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```








