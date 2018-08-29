# <a name="update-androidlobapp"></a><span data-ttu-id="7b596-101">androidLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="7b596-101">Update androidLobApp</span></span>

> <span data-ttu-id="7b596-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b596-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b596-103">[androidLobApp](../resources/intune_apps_androidlobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7b596-103">Update the properties of a [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b596-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7b596-104">Prerequisites</span></span>
<span data-ttu-id="7b596-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b596-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7b596-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b596-107">Permission type</span></span>|<span data-ttu-id="7b596-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b596-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b596-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b596-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7b596-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b596-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7b596-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b596-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b596-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b596-112">Not supported.</span></span>|
|<span data-ttu-id="7b596-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b596-113">Application</span></span>|<span data-ttu-id="7b596-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b596-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b596-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b596-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="7b596-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b596-116">Request headers</span></span>
|<span data-ttu-id="7b596-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b596-117">Header</span></span>|<span data-ttu-id="7b596-118">値</span><span class="sxs-lookup"><span data-stu-id="7b596-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b596-119">承認</span><span class="sxs-lookup"><span data-stu-id="7b596-119">Authorization</span></span>|<span data-ttu-id="7b596-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7b596-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b596-121">承諾</span><span class="sxs-lookup"><span data-stu-id="7b596-121">Accept</span></span>|<span data-ttu-id="7b596-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7b596-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b596-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b596-123">Request body</span></span>
<span data-ttu-id="7b596-124">要求本文で、[androidLobApp](../resources/intune_apps_androidlobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b596-124">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>

<span data-ttu-id="7b596-125">次の表に、[androidLobApp](../resources/intune_apps_androidlobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7b596-125">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune_apps_androidlobapp.md).</span></span>

|<span data-ttu-id="7b596-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b596-126">Property</span></span>|<span data-ttu-id="7b596-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="7b596-127">Type</span></span>|<span data-ttu-id="7b596-128">説明</span><span class="sxs-lookup"><span data-stu-id="7b596-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b596-129">ID</span><span class="sxs-lookup"><span data-stu-id="7b596-129">id</span></span>|<span data-ttu-id="7b596-130">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-130">String</span></span>|<span data-ttu-id="7b596-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7b596-131">Key of the entity.</span></span> <span data-ttu-id="7b596-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7b596-133">displayName</span></span>|<span data-ttu-id="7b596-134">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-134">String</span></span>|<span data-ttu-id="7b596-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="7b596-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7b596-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-137">説明</span><span class="sxs-lookup"><span data-stu-id="7b596-137">description</span></span>|<span data-ttu-id="7b596-138">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-138">String</span></span>|<span data-ttu-id="7b596-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="7b596-139">The description of the app.</span></span> <span data-ttu-id="7b596-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-141">publisher</span><span class="sxs-lookup"><span data-stu-id="7b596-141">publisher</span></span>|<span data-ttu-id="7b596-142">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-142">String</span></span>|<span data-ttu-id="7b596-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="7b596-143">The publisher of the app.</span></span> <span data-ttu-id="7b596-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7b596-145">largeIcon</span></span>|[<span data-ttu-id="7b596-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7b596-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="7b596-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="7b596-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7b596-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b596-149">createdDateTime</span></span>|<span data-ttu-id="7b596-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b596-150">DateTimeOffset</span></span>|<span data-ttu-id="7b596-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7b596-151">The date and time the app was created.</span></span> <span data-ttu-id="7b596-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b596-153">lastModifiedDateTime</span></span>|<span data-ttu-id="7b596-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b596-154">DateTimeOffset</span></span>|<span data-ttu-id="7b596-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="7b596-155">The date and time the app was last modified.</span></span> <span data-ttu-id="7b596-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7b596-157">isFeatured</span></span>|<span data-ttu-id="7b596-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="7b596-158">Boolean</span></span>|<span data-ttu-id="7b596-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7b596-160">privacyInformationUrl</span></span>|<span data-ttu-id="7b596-161">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-161">String</span></span>|<span data-ttu-id="7b596-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="7b596-162">The privacy statement Url.</span></span> <span data-ttu-id="7b596-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7b596-164">informationUrl</span></span>|<span data-ttu-id="7b596-165">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-165">String</span></span>|<span data-ttu-id="7b596-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="7b596-166">The more information Url.</span></span> <span data-ttu-id="7b596-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-168">owner</span><span class="sxs-lookup"><span data-stu-id="7b596-168">owner</span></span>|<span data-ttu-id="7b596-169">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-169">String</span></span>|<span data-ttu-id="7b596-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="7b596-170">The owner of the app.</span></span> <span data-ttu-id="7b596-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-172">developer</span><span class="sxs-lookup"><span data-stu-id="7b596-172">developer</span></span>|<span data-ttu-id="7b596-173">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-173">String</span></span>|<span data-ttu-id="7b596-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="7b596-174">The developer of the app.</span></span> <span data-ttu-id="7b596-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-176">notes</span><span class="sxs-lookup"><span data-stu-id="7b596-176">notes</span></span>|<span data-ttu-id="7b596-177">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-177">String</span></span>|<span data-ttu-id="7b596-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="7b596-178">Notes for the app.</span></span> <span data-ttu-id="7b596-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7b596-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="7b596-180">publishingState</span></span>|[<span data-ttu-id="7b596-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7b596-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="7b596-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="7b596-182">The publishing state for the app.</span></span> <span data-ttu-id="7b596-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="7b596-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7b596-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="7b596-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="7b596-185">指定できる値は、 `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="7b596-185">The possible values are `notPublished`, `processing`, or `published`.</span></span>|
|<span data-ttu-id="7b596-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7b596-186">committedContentVersion</span></span>|<span data-ttu-id="7b596-187">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-187">String</span></span>|<span data-ttu-id="7b596-188">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7b596-188">The internal committed content version.</span></span> <span data-ttu-id="7b596-189">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="7b596-190">fileName</span><span class="sxs-lookup"><span data-stu-id="7b596-190">fileName</span></span>|<span data-ttu-id="7b596-191">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-191">String</span></span>|<span data-ttu-id="7b596-192">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="7b596-192">The name of the main Lob application file.</span></span> <span data-ttu-id="7b596-193">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="7b596-194">size</span><span class="sxs-lookup"><span data-stu-id="7b596-194">size</span></span>|<span data-ttu-id="7b596-195">Int64</span><span class="sxs-lookup"><span data-stu-id="7b596-195">Int64</span></span>|<span data-ttu-id="7b596-196">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="7b596-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="7b596-197">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7b596-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="7b596-198">packageId</span><span class="sxs-lookup"><span data-stu-id="7b596-198">packageId</span></span>|<span data-ttu-id="7b596-199">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-199">String</span></span>|<span data-ttu-id="7b596-200">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="7b596-200">The package identifier.</span></span>|
|<span data-ttu-id="7b596-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7b596-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7b596-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7b596-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="7b596-203">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="7b596-203">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7b596-204">versionName</span><span class="sxs-lookup"><span data-stu-id="7b596-204">versionName</span></span>|<span data-ttu-id="7b596-205">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-205">String</span></span>|<span data-ttu-id="7b596-206">Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="7b596-206">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7b596-207">versionCode</span><span class="sxs-lookup"><span data-stu-id="7b596-207">versionCode</span></span>|<span data-ttu-id="7b596-208">文字列</span><span class="sxs-lookup"><span data-stu-id="7b596-208">String</span></span>|<span data-ttu-id="7b596-209">Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="7b596-209">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="7b596-210">応答</span><span class="sxs-lookup"><span data-stu-id="7b596-210">Response</span></span>
<span data-ttu-id="7b596-211">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidLobApp](../resources/intune_apps_androidlobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="7b596-211">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b596-212">例</span><span class="sxs-lookup"><span data-stu-id="7b596-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b596-213">要求</span><span class="sxs-lookup"><span data-stu-id="7b596-213">Request</span></span>
<span data-ttu-id="7b596-214">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b596-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1087

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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="7b596-215">応答</span><span class="sxs-lookup"><span data-stu-id="7b596-215">Response</span></span>
<span data-ttu-id="7b596-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7b596-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



