# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="ee7f1-101">microsoftStoreForBusinessApp の更新</span><span class="sxs-lookup"><span data-stu-id="ee7f1-101">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="ee7f1-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee7f1-103">[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-103">Update the properties of a [calendar](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee7f1-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee7f1-104">Prerequisites</span></span>
<span data-ttu-id="ee7f1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ee7f1-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee7f1-107">Permission type</span></span>|<span data-ttu-id="ee7f1-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee7f1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee7f1-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee7f1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ee7f1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee7f1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ee7f1-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee7f1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee7f1-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-112">Not supported.</span></span>|
|<span data-ttu-id="ee7f1-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee7f1-113">Application</span></span>|<span data-ttu-id="ee7f1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee7f1-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee7f1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ee7f1-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee7f1-116">Request headers</span></span>
|<span data-ttu-id="ee7f1-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee7f1-117">Header</span></span>|<span data-ttu-id="ee7f1-118">値</span><span class="sxs-lookup"><span data-stu-id="ee7f1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee7f1-119">承認</span><span class="sxs-lookup"><span data-stu-id="ee7f1-119">Authorization</span></span>|<span data-ttu-id="ee7f1-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ee7f1-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ee7f1-121">Accept</span></span>|<span data-ttu-id="ee7f1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ee7f1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee7f1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee7f1-123">Request body</span></span>
<span data-ttu-id="ee7f1-124">要求本文で、[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="ee7f1-125">次の表に、[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ee7f1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee7f1-126">Property</span></span>|<span data-ttu-id="ee7f1-127">型</span><span class="sxs-lookup"><span data-stu-id="ee7f1-127">Type</span></span>|<span data-ttu-id="ee7f1-128">説明</span><span class="sxs-lookup"><span data-stu-id="ee7f1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee7f1-129">id</span><span class="sxs-lookup"><span data-stu-id="ee7f1-129">id</span></span>|<span data-ttu-id="ee7f1-130">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-130">String</span></span>|<span data-ttu-id="ee7f1-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-131">Name of the entity.</span></span> <span data-ttu-id="ee7f1-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ee7f1-133">displayName</span></span>|<span data-ttu-id="ee7f1-134">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-134">String</span></span>|<span data-ttu-id="ee7f1-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ee7f1-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-137">description</span><span class="sxs-lookup"><span data-stu-id="ee7f1-137">description</span></span>|<span data-ttu-id="ee7f1-138">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-138">String</span></span>|<span data-ttu-id="ee7f1-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-139">The description of the app.</span></span> <span data-ttu-id="ee7f1-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-141">publisher</span><span class="sxs-lookup"><span data-stu-id="ee7f1-141">Publisher</span></span>|<span data-ttu-id="ee7f1-142">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-142">String</span></span>|<span data-ttu-id="ee7f1-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-143">The name of the app.</span></span> <span data-ttu-id="ee7f1-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ee7f1-145">largeIcon</span></span>|[<span data-ttu-id="ee7f1-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ee7f1-146">MimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="ee7f1-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ee7f1-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee7f1-149">createdDateTime</span></span>|<span data-ttu-id="ee7f1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee7f1-150">DateTimeOffset</span></span>|<span data-ttu-id="ee7f1-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-151">The date and time when the page was created.</span></span> <span data-ttu-id="ee7f1-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee7f1-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ee7f1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee7f1-154">DateTimeOffset</span></span>|<span data-ttu-id="ee7f1-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="ee7f1-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ee7f1-157">isFeatured</span></span>|<span data-ttu-id="ee7f1-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee7f1-158">Boolean</span></span>|<span data-ttu-id="ee7f1-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ee7f1-160">privacyInformationUrl</span></span>|<span data-ttu-id="ee7f1-161">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-161">String</span></span>|<span data-ttu-id="ee7f1-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-162">The privacy statement Url.</span></span> <span data-ttu-id="ee7f1-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ee7f1-164">informationUrl</span></span>|<span data-ttu-id="ee7f1-165">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-165">String</span></span>|<span data-ttu-id="ee7f1-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-166">The more information Url.</span></span> <span data-ttu-id="ee7f1-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-168">owner</span><span class="sxs-lookup"><span data-stu-id="ee7f1-168">owner</span></span>|<span data-ttu-id="ee7f1-169">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-169">String</span></span>|<span data-ttu-id="ee7f1-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-170">The owner of the timesheet.</span></span> <span data-ttu-id="ee7f1-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-172">developer</span><span class="sxs-lookup"><span data-stu-id="ee7f1-172">developer</span></span>|<span data-ttu-id="ee7f1-173">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-173">String</span></span>|<span data-ttu-id="ee7f1-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-174">The name of the app.</span></span> <span data-ttu-id="ee7f1-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-176">notes</span><span class="sxs-lookup"><span data-stu-id="ee7f1-176">notes</span></span>|<span data-ttu-id="ee7f1-177">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-177">String</span></span>|<span data-ttu-id="ee7f1-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-178">Notes for the app.</span></span> <span data-ttu-id="ee7f1-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ee7f1-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ee7f1-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ee7f1-180">publishingState</span></span>|<span data-ttu-id="ee7f1-181">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-181">String</span></span>|<span data-ttu-id="ee7f1-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-182">The publishing state for the app.</span></span> <span data-ttu-id="ee7f1-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ee7f1-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ee7f1-185">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ee7f1-185">usedLicenseCount</span></span>|<span data-ttu-id="ee7f1-186">Int32</span><span class="sxs-lookup"><span data-stu-id="ee7f1-186">Int32</span></span>|<span data-ttu-id="ee7f1-187">使用中の、ビジネス向け Microsoft Store ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-187">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="ee7f1-188">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ee7f1-188">totalLicenseCount</span></span>|<span data-ttu-id="ee7f1-189">Int32</span><span class="sxs-lookup"><span data-stu-id="ee7f1-189">Int32</span></span>|<span data-ttu-id="ee7f1-190">ビジネス向け Microsoft Store ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-190">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="ee7f1-191">productKey</span><span class="sxs-lookup"><span data-stu-id="ee7f1-191">productKey</span></span>|<span data-ttu-id="ee7f1-192">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-192">String</span></span>|<span data-ttu-id="ee7f1-193">アプリのプロダクト キー</span><span class="sxs-lookup"><span data-stu-id="ee7f1-193">The app product key</span></span>|
|<span data-ttu-id="ee7f1-194">licenseType</span><span class="sxs-lookup"><span data-stu-id="ee7f1-194">licenseType</span></span>|<span data-ttu-id="ee7f1-195">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-195">String</span></span>|<span data-ttu-id="ee7f1-196">アプリ ライセンスの種類。可能な値は、`offline`、`online` です。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-196">The app license type Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="ee7f1-197">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="ee7f1-197">packageIdentityName</span></span>|<span data-ttu-id="ee7f1-198">String</span><span class="sxs-lookup"><span data-stu-id="ee7f1-198">String</span></span>|<span data-ttu-id="ee7f1-199">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="ee7f1-199">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="ee7f1-200">応答</span><span class="sxs-lookup"><span data-stu-id="ee7f1-200">Response</span></span>
<span data-ttu-id="ee7f1-201">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-201">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee7f1-202">例</span><span class="sxs-lookup"><span data-stu-id="ee7f1-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee7f1-203">要求</span><span class="sxs-lookup"><span data-stu-id="ee7f1-203">Request</span></span>
<span data-ttu-id="ee7f1-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 766

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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="ee7f1-205">応答</span><span class="sxs-lookup"><span data-stu-id="ee7f1-205">Response</span></span>
<span data-ttu-id="ee7f1-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee7f1-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



