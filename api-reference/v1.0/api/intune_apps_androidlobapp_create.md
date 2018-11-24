# <a name="create-androidlobapp"></a><span data-ttu-id="f60e3-101">androidLobApp の作成</span><span class="sxs-lookup"><span data-stu-id="f60e3-101">Create androidLobApp</span></span>

> <span data-ttu-id="f60e3-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f60e3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f60e3-103">新しい [androidLobApp](../resources/intune_apps_androidlobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f60e3-103">Create a new [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f60e3-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="f60e3-104">Prerequisites</span></span>
<span data-ttu-id="f60e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f60e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f60e3-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f60e3-107">Permission type</span></span>|<span data-ttu-id="f60e3-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f60e3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f60e3-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f60e3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f60e3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f60e3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f60e3-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f60e3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f60e3-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f60e3-112">Not supported.</span></span>|
|<span data-ttu-id="f60e3-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f60e3-113">Application</span></span>|<span data-ttu-id="f60e3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f60e3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f60e3-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f60e3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f60e3-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f60e3-116">Request headers</span></span>
|<span data-ttu-id="f60e3-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f60e3-117">Header</span></span>|<span data-ttu-id="f60e3-118">値</span><span class="sxs-lookup"><span data-stu-id="f60e3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f60e3-119">承認</span><span class="sxs-lookup"><span data-stu-id="f60e3-119">Authorization</span></span>|<span data-ttu-id="f60e3-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="f60e3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f60e3-121">承諾</span><span class="sxs-lookup"><span data-stu-id="f60e3-121">Accept</span></span>|<span data-ttu-id="f60e3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f60e3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f60e3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f60e3-123">Request body</span></span>
<span data-ttu-id="f60e3-124">要求本文で、androidLobApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f60e3-124">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="f60e3-125">次の表に、androidLobApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f60e3-125">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="f60e3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f60e3-126">Property</span></span>|<span data-ttu-id="f60e3-127">型</span><span class="sxs-lookup"><span data-stu-id="f60e3-127">Type</span></span>|<span data-ttu-id="f60e3-128">説明</span><span class="sxs-lookup"><span data-stu-id="f60e3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f60e3-129">id</span><span class="sxs-lookup"><span data-stu-id="f60e3-129">id</span></span>|<span data-ttu-id="f60e3-130">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-130">String</span></span>|<span data-ttu-id="f60e3-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f60e3-131">Key of the entity.</span></span> <span data-ttu-id="f60e3-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f60e3-133">displayName</span></span>|<span data-ttu-id="f60e3-134">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-134">String</span></span>|<span data-ttu-id="f60e3-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f60e3-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f60e3-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-137">description</span><span class="sxs-lookup"><span data-stu-id="f60e3-137">description</span></span>|<span data-ttu-id="f60e3-138">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-138">String</span></span>|<span data-ttu-id="f60e3-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f60e3-139">The description of the app.</span></span> <span data-ttu-id="f60e3-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-141">publisher</span><span class="sxs-lookup"><span data-stu-id="f60e3-141">publisher</span></span>|<span data-ttu-id="f60e3-142">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-142">String</span></span>|<span data-ttu-id="f60e3-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f60e3-143">The publisher of the app.</span></span> <span data-ttu-id="f60e3-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f60e3-145">largeIcon</span></span>|[<span data-ttu-id="f60e3-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f60e3-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="f60e3-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="f60e3-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f60e3-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f60e3-149">createdDateTime</span></span>|<span data-ttu-id="f60e3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f60e3-150">DateTimeOffset</span></span>|<span data-ttu-id="f60e3-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f60e3-151">The date and time the app was created.</span></span> <span data-ttu-id="f60e3-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f60e3-153">lastModifiedDateTime</span></span>|<span data-ttu-id="f60e3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f60e3-154">DateTimeOffset</span></span>|<span data-ttu-id="f60e3-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f60e3-155">The date and time the app was last modified.</span></span> <span data-ttu-id="f60e3-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f60e3-157">isFeatured</span></span>|<span data-ttu-id="f60e3-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="f60e3-158">Boolean</span></span>|<span data-ttu-id="f60e3-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f60e3-160">privacyInformationUrl</span></span>|<span data-ttu-id="f60e3-161">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-161">String</span></span>|<span data-ttu-id="f60e3-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f60e3-162">The privacy statement Url.</span></span> <span data-ttu-id="f60e3-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f60e3-164">informationUrl</span></span>|<span data-ttu-id="f60e3-165">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-165">String</span></span>|<span data-ttu-id="f60e3-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f60e3-166">The more information Url.</span></span> <span data-ttu-id="f60e3-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-168">owner</span><span class="sxs-lookup"><span data-stu-id="f60e3-168">owner</span></span>|<span data-ttu-id="f60e3-169">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-169">String</span></span>|<span data-ttu-id="f60e3-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f60e3-170">The owner of the app.</span></span> <span data-ttu-id="f60e3-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-172">developer</span><span class="sxs-lookup"><span data-stu-id="f60e3-172">developer</span></span>|<span data-ttu-id="f60e3-173">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-173">String</span></span>|<span data-ttu-id="f60e3-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f60e3-174">The developer of the app.</span></span> <span data-ttu-id="f60e3-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-176">notes</span><span class="sxs-lookup"><span data-stu-id="f60e3-176">notes</span></span>|<span data-ttu-id="f60e3-177">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-177">String</span></span>|<span data-ttu-id="f60e3-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f60e3-178">Notes for the app.</span></span> <span data-ttu-id="f60e3-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f60e3-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="f60e3-180">publishingState</span></span>|[<span data-ttu-id="f60e3-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f60e3-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="f60e3-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f60e3-182">The publishing state for the app.</span></span> <span data-ttu-id="f60e3-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f60e3-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f60e3-184">[MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f60e3-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="f60e3-185">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="f60e3-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f60e3-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f60e3-186">committedContentVersion</span></span>|<span data-ttu-id="f60e3-187">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-187">String</span></span>|<span data-ttu-id="f60e3-188">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f60e3-188">The internal committed content version.</span></span> <span data-ttu-id="f60e3-189">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="f60e3-190">fileName</span><span class="sxs-lookup"><span data-stu-id="f60e3-190">fileName</span></span>|<span data-ttu-id="f60e3-191">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-191">String</span></span>|<span data-ttu-id="f60e3-192">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="f60e3-192">The name of the main Lob application file.</span></span> <span data-ttu-id="f60e3-193">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="f60e3-194">size</span><span class="sxs-lookup"><span data-stu-id="f60e3-194">size</span></span>|<span data-ttu-id="f60e3-195">Int64</span><span class="sxs-lookup"><span data-stu-id="f60e3-195">Int64</span></span>|<span data-ttu-id="f60e3-196">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="f60e3-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="f60e3-197">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f60e3-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="f60e3-198">packageId</span><span class="sxs-lookup"><span data-stu-id="f60e3-198">packageId</span></span>|<span data-ttu-id="f60e3-199">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-199">String</span></span>|<span data-ttu-id="f60e3-200">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="f60e3-200">The package identifier.</span></span>|
|<span data-ttu-id="f60e3-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f60e3-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f60e3-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f60e3-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="f60e3-203">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="f60e3-203">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f60e3-204">versionName</span><span class="sxs-lookup"><span data-stu-id="f60e3-204">versionName</span></span>|<span data-ttu-id="f60e3-205">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-205">String</span></span>|<span data-ttu-id="f60e3-206">Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="f60e3-206">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f60e3-207">versionCode</span><span class="sxs-lookup"><span data-stu-id="f60e3-207">versionCode</span></span>|<span data-ttu-id="f60e3-208">String</span><span class="sxs-lookup"><span data-stu-id="f60e3-208">String</span></span>|<span data-ttu-id="f60e3-209">Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="f60e3-209">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="f60e3-210">応答</span><span class="sxs-lookup"><span data-stu-id="f60e3-210">Response</span></span>
<span data-ttu-id="f60e3-211">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidLobApp](../resources/intune_apps_androidlobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f60e3-211">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f60e3-212">例</span><span class="sxs-lookup"><span data-stu-id="f60e3-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="f60e3-213">要求</span><span class="sxs-lookup"><span data-stu-id="f60e3-213">Request</span></span>
<span data-ttu-id="f60e3-214">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f60e3-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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

### <a name="response"></a><span data-ttu-id="f60e3-215">応答</span><span class="sxs-lookup"><span data-stu-id="f60e3-215">Response</span></span>
<span data-ttu-id="f60e3-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f60e3-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



