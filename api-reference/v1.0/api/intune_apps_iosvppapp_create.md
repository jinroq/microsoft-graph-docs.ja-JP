# <a name="create-iosvppapp"></a><span data-ttu-id="246db-101">iosVppApp を作成する</span><span class="sxs-lookup"><span data-stu-id="246db-101">Create iosVppApp</span></span>

> <span data-ttu-id="246db-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="246db-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="246db-103">新しい [iosVppApp](../resources/intune_apps_iosvppapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="246db-103">Create a new [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="246db-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="246db-104">Prerequisites</span></span>
<span data-ttu-id="246db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="246db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="246db-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="246db-107">Permission type</span></span>|<span data-ttu-id="246db-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="246db-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="246db-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="246db-109">Delegated (work or school account)</span></span>|<span data-ttu-id="246db-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="246db-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="246db-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="246db-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="246db-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="246db-112">Not supported.</span></span>|
|<span data-ttu-id="246db-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="246db-113">Application</span></span>|<span data-ttu-id="246db-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="246db-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="246db-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="246db-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="246db-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="246db-116">Request headers</span></span>
|<span data-ttu-id="246db-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="246db-117">Header</span></span>|<span data-ttu-id="246db-118">値</span><span class="sxs-lookup"><span data-stu-id="246db-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="246db-119">承認</span><span class="sxs-lookup"><span data-stu-id="246db-119">Authorization</span></span>|<span data-ttu-id="246db-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="246db-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="246db-121">承諾</span><span class="sxs-lookup"><span data-stu-id="246db-121">Accept</span></span>|<span data-ttu-id="246db-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="246db-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="246db-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="246db-123">Request body</span></span>
<span data-ttu-id="246db-124">要求本文で、iosVppApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="246db-124">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="246db-125">次の表に、iosVppApp 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="246db-125">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="246db-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="246db-126">Property</span></span>|<span data-ttu-id="246db-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="246db-127">Type</span></span>|<span data-ttu-id="246db-128">説明</span><span class="sxs-lookup"><span data-stu-id="246db-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="246db-129">ID</span><span class="sxs-lookup"><span data-stu-id="246db-129">id</span></span>|<span data-ttu-id="246db-130">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-130">String</span></span>|<span data-ttu-id="246db-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="246db-131">Key of the entity.</span></span> <span data-ttu-id="246db-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-133">displayName</span><span class="sxs-lookup"><span data-stu-id="246db-133">displayName</span></span>|<span data-ttu-id="246db-134">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-134">String</span></span>|<span data-ttu-id="246db-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="246db-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="246db-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-137">説明</span><span class="sxs-lookup"><span data-stu-id="246db-137">description</span></span>|<span data-ttu-id="246db-138">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-138">String</span></span>|<span data-ttu-id="246db-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="246db-139">The description of the app.</span></span> <span data-ttu-id="246db-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-141">パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="246db-141">publisher</span></span>|<span data-ttu-id="246db-142">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-142">String</span></span>|<span data-ttu-id="246db-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="246db-143">The publisher of the app.</span></span> <span data-ttu-id="246db-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="246db-145">largeIcon</span></span>|[<span data-ttu-id="246db-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="246db-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="246db-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="246db-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="246db-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="246db-149">createdDateTime</span></span>|<span data-ttu-id="246db-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="246db-150">DateTimeOffset</span></span>|<span data-ttu-id="246db-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="246db-151">The date and time the app was created.</span></span> <span data-ttu-id="246db-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="246db-153">lastModifiedDateTime</span></span>|<span data-ttu-id="246db-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="246db-154">DateTimeOffset</span></span>|<span data-ttu-id="246db-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="246db-155">The date and time the app was last modified.</span></span> <span data-ttu-id="246db-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="246db-157">isFeatured</span></span>|<span data-ttu-id="246db-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="246db-158">Boolean</span></span>|<span data-ttu-id="246db-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="246db-160">privacyInformationUrl</span></span>|<span data-ttu-id="246db-161">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-161">String</span></span>|<span data-ttu-id="246db-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="246db-162">The privacy statement Url.</span></span> <span data-ttu-id="246db-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="246db-164">informationUrl</span></span>|<span data-ttu-id="246db-165">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-165">String</span></span>|<span data-ttu-id="246db-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="246db-166">The more information Url.</span></span> <span data-ttu-id="246db-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-168">所有者</span><span class="sxs-lookup"><span data-stu-id="246db-168">owner</span></span>|<span data-ttu-id="246db-169">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-169">String</span></span>|<span data-ttu-id="246db-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="246db-170">The owner of the app.</span></span> <span data-ttu-id="246db-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-172">開発者</span><span class="sxs-lookup"><span data-stu-id="246db-172">developer</span></span>|<span data-ttu-id="246db-173">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-173">String</span></span>|<span data-ttu-id="246db-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="246db-174">The developer of the app.</span></span> <span data-ttu-id="246db-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-176">備考</span><span class="sxs-lookup"><span data-stu-id="246db-176">notes</span></span>|<span data-ttu-id="246db-177">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-177">String</span></span>|<span data-ttu-id="246db-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="246db-178">Notes for the app.</span></span> <span data-ttu-id="246db-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="246db-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="246db-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="246db-180">publishingState</span></span>|[<span data-ttu-id="246db-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="246db-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="246db-p114">アプリケーションの発行の状態です。アプリが公開されていない限り、アプリケーションを割り当てることができません。[mobileApp](../resources/intune_apps_mobileapp.md) から継承されます。指定できる値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="246db-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="246db-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="246db-186">usedLicenseCount</span></span>|<span data-ttu-id="246db-187">Int32</span><span class="sxs-lookup"><span data-stu-id="246db-187">Int32</span></span>|<span data-ttu-id="246db-188">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="246db-188">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="246db-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="246db-189">totalLicenseCount</span></span>|<span data-ttu-id="246db-190">Int32</span><span class="sxs-lookup"><span data-stu-id="246db-190">Int32</span></span>|<span data-ttu-id="246db-191">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="246db-191">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="246db-192">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="246db-192">releaseDateTime</span></span>|<span data-ttu-id="246db-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="246db-193">DateTimeOffset</span></span>|<span data-ttu-id="246db-194">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="246db-194">The VPP application release date and time.</span></span>|
|<span data-ttu-id="246db-195">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="246db-195">appStoreUrl</span></span>|<span data-ttu-id="246db-196">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-196">String</span></span>|<span data-ttu-id="246db-197">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="246db-197">The store URL.</span></span>|
|<span data-ttu-id="246db-198">licensingType</span><span class="sxs-lookup"><span data-stu-id="246db-198">licensingType</span></span>|[<span data-ttu-id="246db-199">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="246db-199">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="246db-200">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="246db-200">The supported License Type.</span></span>|
|<span data-ttu-id="246db-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="246db-201">applicableDeviceType</span></span>|[<span data-ttu-id="246db-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="246db-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="246db-203">該当する iOS デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="246db-203">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="246db-204">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="246db-204">vppTokenOrganizationName</span></span>|<span data-ttu-id="246db-205">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-205">String</span></span>|<span data-ttu-id="246db-206">Apple Volume Purchase Program のトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="246db-206">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="246db-207">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="246db-207">vppTokenAccountType</span></span>|[<span data-ttu-id="246db-208">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="246db-208">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="246db-p115">特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類です。指定できる値は、`business`、`education` です。指定できる値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="246db-p115">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. The possible values are: `business`, `education`. The possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="246db-212">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="246db-212">vppTokenAppleId</span></span>|<span data-ttu-id="246db-213">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-213">String</span></span>|<span data-ttu-id="246db-214">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="246db-214">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="246db-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="246db-215">bundleId</span></span>|<span data-ttu-id="246db-216">文字列</span><span class="sxs-lookup"><span data-stu-id="246db-216">String</span></span>|<span data-ttu-id="246db-217">ID 名。</span><span class="sxs-lookup"><span data-stu-id="246db-217">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="246db-218">応答</span><span class="sxs-lookup"><span data-stu-id="246db-218">Response</span></span>
<span data-ttu-id="246db-219">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppApp](../resources/intune_apps_iosvppapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="246db-219">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="246db-220">例</span><span class="sxs-lookup"><span data-stu-id="246db-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="246db-221">要求</span><span class="sxs-lookup"><span data-stu-id="246db-221">Request</span></span>
<span data-ttu-id="246db-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="246db-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1286

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="246db-223">応答</span><span class="sxs-lookup"><span data-stu-id="246db-223">Response</span></span>
<span data-ttu-id="246db-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="246db-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```








