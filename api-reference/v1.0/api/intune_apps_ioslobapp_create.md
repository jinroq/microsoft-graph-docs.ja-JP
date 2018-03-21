# <a name="create-ioslobapp"></a><span data-ttu-id="f012c-101">iosLobApp の作成</span><span class="sxs-lookup"><span data-stu-id="f012c-101">Create iosLobApp</span></span>

> <span data-ttu-id="f012c-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f012c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f012c-103">新しい [iosLobApp](../resources/intune_apps_ioslobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f012c-103">Create a new [plannerBucket](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f012c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="f012c-104">Prerequisites</span></span>
<span data-ttu-id="f012c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f012c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f012c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f012c-107">Permission type</span></span>|<span data-ttu-id="f012c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f012c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f012c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f012c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f012c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f012c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f012c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f012c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f012c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f012c-112">Not supported.</span></span>|
|<span data-ttu-id="f012c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f012c-113">Application</span></span>|<span data-ttu-id="f012c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f012c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f012c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f012c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f012c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f012c-116">Request headers</span></span>
|<span data-ttu-id="f012c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f012c-117">Header</span></span>|<span data-ttu-id="f012c-118">値</span><span class="sxs-lookup"><span data-stu-id="f012c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f012c-119">承認</span><span class="sxs-lookup"><span data-stu-id="f012c-119">Authorization</span></span>|<span data-ttu-id="f012c-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="f012c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f012c-121">承諾</span><span class="sxs-lookup"><span data-stu-id="f012c-121">Accept</span></span>|<span data-ttu-id="f012c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f012c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f012c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f012c-123">Request body</span></span>
<span data-ttu-id="f012c-124">要求本文で、iosLobApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f012c-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="f012c-125">次の表に、iosLobApp 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f012c-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="f012c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f012c-126">Property</span></span>|<span data-ttu-id="f012c-127">型</span><span class="sxs-lookup"><span data-stu-id="f012c-127">Type</span></span>|<span data-ttu-id="f012c-128">説明</span><span class="sxs-lookup"><span data-stu-id="f012c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f012c-129">id</span><span class="sxs-lookup"><span data-stu-id="f012c-129">id</span></span>|<span data-ttu-id="f012c-130">String</span><span class="sxs-lookup"><span data-stu-id="f012c-130">String</span></span>|<span data-ttu-id="f012c-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f012c-131">Name of the entity.</span></span> <span data-ttu-id="f012c-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f012c-133">displayName</span></span>|<span data-ttu-id="f012c-134">String</span><span class="sxs-lookup"><span data-stu-id="f012c-134">String</span></span>|<span data-ttu-id="f012c-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f012c-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f012c-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-137">description</span><span class="sxs-lookup"><span data-stu-id="f012c-137">description</span></span>|<span data-ttu-id="f012c-138">String</span><span class="sxs-lookup"><span data-stu-id="f012c-138">String</span></span>|<span data-ttu-id="f012c-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f012c-139">The description of the app.</span></span> <span data-ttu-id="f012c-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-141">publisher</span><span class="sxs-lookup"><span data-stu-id="f012c-141">Publisher</span></span>|<span data-ttu-id="f012c-142">String</span><span class="sxs-lookup"><span data-stu-id="f012c-142">String</span></span>|<span data-ttu-id="f012c-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f012c-143">The name of the app.</span></span> <span data-ttu-id="f012c-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f012c-145">largeIcon</span></span>|[<span data-ttu-id="f012c-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f012c-146">MimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="f012c-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="f012c-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f012c-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f012c-149">createdDateTime</span></span>|<span data-ttu-id="f012c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f012c-150">DateTimeOffset</span></span>|<span data-ttu-id="f012c-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f012c-151">The date and time when the page was created.</span></span> <span data-ttu-id="f012c-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f012c-153">lastModifiedDateTime</span></span>|<span data-ttu-id="f012c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f012c-154">DateTimeOffset</span></span>|<span data-ttu-id="f012c-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f012c-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="f012c-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f012c-157">isFeatured</span></span>|<span data-ttu-id="f012c-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="f012c-158">Boolean</span></span>|<span data-ttu-id="f012c-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f012c-160">privacyInformationUrl</span></span>|<span data-ttu-id="f012c-161">String</span><span class="sxs-lookup"><span data-stu-id="f012c-161">String</span></span>|<span data-ttu-id="f012c-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f012c-162">The privacy statement Url.</span></span> <span data-ttu-id="f012c-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f012c-164">informationUrl</span></span>|<span data-ttu-id="f012c-165">String</span><span class="sxs-lookup"><span data-stu-id="f012c-165">String</span></span>|<span data-ttu-id="f012c-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f012c-166">The more information Url.</span></span> <span data-ttu-id="f012c-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-168">owner</span><span class="sxs-lookup"><span data-stu-id="f012c-168">owner</span></span>|<span data-ttu-id="f012c-169">String</span><span class="sxs-lookup"><span data-stu-id="f012c-169">String</span></span>|<span data-ttu-id="f012c-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f012c-170">The owner of the timesheet.</span></span> <span data-ttu-id="f012c-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-172">developer</span><span class="sxs-lookup"><span data-stu-id="f012c-172">developer</span></span>|<span data-ttu-id="f012c-173">String</span><span class="sxs-lookup"><span data-stu-id="f012c-173">String</span></span>|<span data-ttu-id="f012c-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f012c-174">The name of the app.</span></span> <span data-ttu-id="f012c-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-176">notes</span><span class="sxs-lookup"><span data-stu-id="f012c-176">notes</span></span>|<span data-ttu-id="f012c-177">String</span><span class="sxs-lookup"><span data-stu-id="f012c-177">String</span></span>|<span data-ttu-id="f012c-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f012c-178">Notes for the app.</span></span> <span data-ttu-id="f012c-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f012c-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="f012c-180">publishingState</span></span>|<span data-ttu-id="f012c-181">String</span><span class="sxs-lookup"><span data-stu-id="f012c-181">String</span></span>|<span data-ttu-id="f012c-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f012c-182">The publishing state for the app.</span></span> <span data-ttu-id="f012c-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f012c-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f012c-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="f012c-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f012c-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f012c-185">committedContentVersion</span></span>|<span data-ttu-id="f012c-186">String</span><span class="sxs-lookup"><span data-stu-id="f012c-186">String</span></span>|<span data-ttu-id="f012c-187">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f012c-187">The internal committed content version.</span></span> <span data-ttu-id="f012c-188">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="f012c-189">fileName</span><span class="sxs-lookup"><span data-stu-id="f012c-189">FileName</span></span>|<span data-ttu-id="f012c-190">String</span><span class="sxs-lookup"><span data-stu-id="f012c-190">String</span></span>|<span data-ttu-id="f012c-191">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="f012c-191">The name of the main Lob application file.</span></span> <span data-ttu-id="f012c-192">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="f012c-193">size</span><span class="sxs-lookup"><span data-stu-id="f012c-193">size</span></span>|<span data-ttu-id="f012c-194">Int64</span><span class="sxs-lookup"><span data-stu-id="f012c-194">Int64</span></span>|<span data-ttu-id="f012c-195">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="f012c-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="f012c-196">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f012c-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="f012c-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="f012c-197">bundleId</span></span>|<span data-ttu-id="f012c-198">String</span><span class="sxs-lookup"><span data-stu-id="f012c-198">String</span></span>|<span data-ttu-id="f012c-199">ID 名。</span><span class="sxs-lookup"><span data-stu-id="f012c-199">The Identity Name.</span></span>|
|<span data-ttu-id="f012c-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f012c-200">applicableDeviceType</span></span>|[<span data-ttu-id="f012c-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f012c-201">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="f012c-202">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="f012c-202">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f012c-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f012c-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f012c-204">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f012c-204">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="f012c-205">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="f012c-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f012c-206">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f012c-206">expirationDateTime</span></span>|<span data-ttu-id="f012c-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f012c-207">DateTimeOffset</span></span>|<span data-ttu-id="f012c-208">有効期限。</span><span class="sxs-lookup"><span data-stu-id="f012c-208">: The expiration time for the subscription.</span></span>|
|<span data-ttu-id="f012c-209">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="f012c-209">versionNumber</span></span>|<span data-ttu-id="f012c-210">String</span><span class="sxs-lookup"><span data-stu-id="f012c-210">String</span></span>|<span data-ttu-id="f012c-211">iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="f012c-211">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f012c-212">buildNumber</span><span class="sxs-lookup"><span data-stu-id="f012c-212">buildNumber</span></span>|<span data-ttu-id="f012c-213">String</span><span class="sxs-lookup"><span data-stu-id="f012c-213">String</span></span>|<span data-ttu-id="f012c-214">iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="f012c-214">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="f012c-215">応答</span><span class="sxs-lookup"><span data-stu-id="f012c-215">Response</span></span>
<span data-ttu-id="f012c-216">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosLobApp](../resources/intune_apps_ioslobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f012c-216">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f012c-217">例</span><span class="sxs-lookup"><span data-stu-id="f012c-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="f012c-218">要求</span><span class="sxs-lookup"><span data-stu-id="f012c-218">Request</span></span>
<span data-ttu-id="f012c-219">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f012c-219">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f012c-220">応答</span><span class="sxs-lookup"><span data-stu-id="f012c-220">Response</span></span>
<span data-ttu-id="f012c-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f012c-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



