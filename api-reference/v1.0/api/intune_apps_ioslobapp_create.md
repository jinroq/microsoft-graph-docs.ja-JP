# <a name="create-ioslobapp"></a><span data-ttu-id="133d9-101">iosLobApp の作成</span><span class="sxs-lookup"><span data-stu-id="133d9-101">Create iosLobApp</span></span>

> <span data-ttu-id="133d9-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="133d9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="133d9-103">新しい [iosLobApp](../resources/intune_apps_ioslobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="133d9-103">Create a new [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="133d9-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="133d9-104">Prerequisites</span></span>
<span data-ttu-id="133d9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="133d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="133d9-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="133d9-107">Permission type</span></span>|<span data-ttu-id="133d9-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="133d9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="133d9-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="133d9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="133d9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="133d9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="133d9-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="133d9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="133d9-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="133d9-112">Not supported.</span></span>|
|<span data-ttu-id="133d9-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="133d9-113">Application</span></span>|<span data-ttu-id="133d9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="133d9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="133d9-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="133d9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="133d9-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="133d9-116">Request headers</span></span>
|<span data-ttu-id="133d9-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="133d9-117">Header</span></span>|<span data-ttu-id="133d9-118">値</span><span class="sxs-lookup"><span data-stu-id="133d9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="133d9-119">承認</span><span class="sxs-lookup"><span data-stu-id="133d9-119">Authorization</span></span>|<span data-ttu-id="133d9-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="133d9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="133d9-121">承諾</span><span class="sxs-lookup"><span data-stu-id="133d9-121">Accept</span></span>|<span data-ttu-id="133d9-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="133d9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="133d9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="133d9-123">Request body</span></span>
<span data-ttu-id="133d9-124">要求本文で、iosLobApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="133d9-124">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="133d9-125">次の表に、iosLobApp 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="133d9-125">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="133d9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="133d9-126">Property</span></span>|<span data-ttu-id="133d9-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="133d9-127">Type</span></span>|<span data-ttu-id="133d9-128">説明</span><span class="sxs-lookup"><span data-stu-id="133d9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="133d9-129">ID</span><span class="sxs-lookup"><span data-stu-id="133d9-129">id</span></span>|<span data-ttu-id="133d9-130">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-130">String</span></span>|<span data-ttu-id="133d9-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="133d9-131">Key of the entity.</span></span> <span data-ttu-id="133d9-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="133d9-133">displayName</span></span>|<span data-ttu-id="133d9-134">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-134">String</span></span>|<span data-ttu-id="133d9-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="133d9-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="133d9-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-137">説明</span><span class="sxs-lookup"><span data-stu-id="133d9-137">description</span></span>|<span data-ttu-id="133d9-138">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-138">String</span></span>|<span data-ttu-id="133d9-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="133d9-139">The description of the app.</span></span> <span data-ttu-id="133d9-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-141">発行元</span><span class="sxs-lookup"><span data-stu-id="133d9-141">publisher</span></span>|<span data-ttu-id="133d9-142">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-142">String</span></span>|<span data-ttu-id="133d9-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="133d9-143">The publisher of the app.</span></span> <span data-ttu-id="133d9-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="133d9-145">largeIcon</span></span>|[<span data-ttu-id="133d9-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="133d9-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="133d9-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="133d9-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="133d9-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="133d9-149">createdDateTime</span></span>|<span data-ttu-id="133d9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="133d9-150">DateTimeOffset</span></span>|<span data-ttu-id="133d9-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="133d9-151">The date and time the app was created.</span></span> <span data-ttu-id="133d9-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="133d9-153">lastModifiedDateTime</span></span>|<span data-ttu-id="133d9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="133d9-154">DateTimeOffset</span></span>|<span data-ttu-id="133d9-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="133d9-155">The date and time the app was last modified.</span></span> <span data-ttu-id="133d9-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="133d9-157">isFeatured</span></span>|<span data-ttu-id="133d9-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="133d9-158">Boolean</span></span>|<span data-ttu-id="133d9-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="133d9-160">privacyInformationUrl</span></span>|<span data-ttu-id="133d9-161">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-161">String</span></span>|<span data-ttu-id="133d9-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="133d9-162">The privacy statement Url.</span></span> <span data-ttu-id="133d9-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="133d9-164">informationUrl</span></span>|<span data-ttu-id="133d9-165">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-165">String</span></span>|<span data-ttu-id="133d9-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="133d9-166">The more information Url.</span></span> <span data-ttu-id="133d9-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-168">所有者</span><span class="sxs-lookup"><span data-stu-id="133d9-168">owner</span></span>|<span data-ttu-id="133d9-169">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-169">String</span></span>|<span data-ttu-id="133d9-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="133d9-170">The owner of the app.</span></span> <span data-ttu-id="133d9-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-172">開発者</span><span class="sxs-lookup"><span data-stu-id="133d9-172">developer</span></span>|<span data-ttu-id="133d9-173">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-173">String</span></span>|<span data-ttu-id="133d9-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="133d9-174">The developer of the app.</span></span> <span data-ttu-id="133d9-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-176">メモ</span><span class="sxs-lookup"><span data-stu-id="133d9-176">notes</span></span>|<span data-ttu-id="133d9-177">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-177">String</span></span>|<span data-ttu-id="133d9-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="133d9-178">Notes for the app.</span></span> <span data-ttu-id="133d9-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="133d9-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="133d9-180">publishingState</span></span>|[<span data-ttu-id="133d9-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="133d9-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="133d9-p114">アプリケーションの発行の状態です。アプリが公開されていない限り、アプリケーションを割り当てることができません。 [MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。使用可能な値は`notPublished`、`processing`、`published`です。</span><span class="sxs-lookup"><span data-stu-id="133d9-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="133d9-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="133d9-186">committedContentVersion</span></span>|<span data-ttu-id="133d9-187">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-187">String</span></span>|<span data-ttu-id="133d9-188">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="133d9-188">The internal committed content version.</span></span> <span data-ttu-id="133d9-189">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="133d9-190">fileName</span><span class="sxs-lookup"><span data-stu-id="133d9-190">fileName</span></span>|<span data-ttu-id="133d9-191">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-191">String</span></span>|<span data-ttu-id="133d9-192">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="133d9-192">The name of the main Lob application file.</span></span> <span data-ttu-id="133d9-193">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="133d9-194">サイズ</span><span class="sxs-lookup"><span data-stu-id="133d9-194">size</span></span>|<span data-ttu-id="133d9-195">Int64</span><span class="sxs-lookup"><span data-stu-id="133d9-195">Int64</span></span>|<span data-ttu-id="133d9-196">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="133d9-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="133d9-197">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="133d9-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="133d9-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="133d9-198">bundleId</span></span>|<span data-ttu-id="133d9-199">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-199">String</span></span>|<span data-ttu-id="133d9-200">ID 名。</span><span class="sxs-lookup"><span data-stu-id="133d9-200">The Identity Name.</span></span>|
|<span data-ttu-id="133d9-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="133d9-201">applicableDeviceType</span></span>|[<span data-ttu-id="133d9-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="133d9-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="133d9-203">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="133d9-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="133d9-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="133d9-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="133d9-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="133d9-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="133d9-206">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="133d9-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="133d9-207">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="133d9-207">expirationDateTime</span></span>|<span data-ttu-id="133d9-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="133d9-208">DateTimeOffset</span></span>|<span data-ttu-id="133d9-209">有効期限。</span><span class="sxs-lookup"><span data-stu-id="133d9-209">The expiration time.</span></span>|
|<span data-ttu-id="133d9-210">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="133d9-210">versionNumber</span></span>|<span data-ttu-id="133d9-211">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-211">String</span></span>|<span data-ttu-id="133d9-212">iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="133d9-212">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="133d9-213">buildNumber</span><span class="sxs-lookup"><span data-stu-id="133d9-213">buildNumber</span></span>|<span data-ttu-id="133d9-214">文字列</span><span class="sxs-lookup"><span data-stu-id="133d9-214">String</span></span>|<span data-ttu-id="133d9-215">iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="133d9-215">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="133d9-216">応答</span><span class="sxs-lookup"><span data-stu-id="133d9-216">Response</span></span>
<span data-ttu-id="133d9-217">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosLobApp](../resources/intune_apps_ioslobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="133d9-217">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="133d9-218">例</span><span class="sxs-lookup"><span data-stu-id="133d9-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="133d9-219">要求</span><span class="sxs-lookup"><span data-stu-id="133d9-219">Request</span></span>
<span data-ttu-id="133d9-220">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="133d9-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1253

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="133d9-221">応答</span><span class="sxs-lookup"><span data-stu-id="133d9-221">Response</span></span>
<span data-ttu-id="133d9-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="133d9-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```








