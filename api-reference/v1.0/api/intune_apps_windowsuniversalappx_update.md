# <a name="update-windowsuniversalappx"></a><span data-ttu-id="40dfc-101">windowsUniversalAppX の更新</span><span class="sxs-lookup"><span data-stu-id="40dfc-101">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="40dfc-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="40dfc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40dfc-103">[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="40dfc-103">Update the properties of a [calendar](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40dfc-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="40dfc-104">Prerequisites</span></span>
<span data-ttu-id="40dfc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40dfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="40dfc-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40dfc-107">Permission type</span></span>|<span data-ttu-id="40dfc-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="40dfc-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40dfc-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40dfc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="40dfc-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40dfc-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40dfc-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40dfc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40dfc-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40dfc-112">Not supported.</span></span>|
|<span data-ttu-id="40dfc-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40dfc-113">Application</span></span>|<span data-ttu-id="40dfc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40dfc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40dfc-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40dfc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="40dfc-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40dfc-116">Request headers</span></span>
|<span data-ttu-id="40dfc-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40dfc-117">Header</span></span>|<span data-ttu-id="40dfc-118">値</span><span class="sxs-lookup"><span data-stu-id="40dfc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40dfc-119">承認</span><span class="sxs-lookup"><span data-stu-id="40dfc-119">Authorization</span></span>|<span data-ttu-id="40dfc-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="40dfc-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="40dfc-121">承諾</span><span class="sxs-lookup"><span data-stu-id="40dfc-121">Accept</span></span>|<span data-ttu-id="40dfc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="40dfc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40dfc-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="40dfc-123">Request body</span></span>
<span data-ttu-id="40dfc-124">要求本文で、[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="40dfc-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="40dfc-125">次の表に、[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="40dfc-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="40dfc-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40dfc-126">Property</span></span>|<span data-ttu-id="40dfc-127">型</span><span class="sxs-lookup"><span data-stu-id="40dfc-127">Type</span></span>|<span data-ttu-id="40dfc-128">説明</span><span class="sxs-lookup"><span data-stu-id="40dfc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40dfc-129">id</span><span class="sxs-lookup"><span data-stu-id="40dfc-129">id</span></span>|<span data-ttu-id="40dfc-130">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-130">String</span></span>|<span data-ttu-id="40dfc-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="40dfc-131">Name of the entity.</span></span> <span data-ttu-id="40dfc-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-133">displayName</span><span class="sxs-lookup"><span data-stu-id="40dfc-133">displayName</span></span>|<span data-ttu-id="40dfc-134">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-134">String</span></span>|<span data-ttu-id="40dfc-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="40dfc-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="40dfc-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-137">description</span><span class="sxs-lookup"><span data-stu-id="40dfc-137">description</span></span>|<span data-ttu-id="40dfc-138">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-138">String</span></span>|<span data-ttu-id="40dfc-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="40dfc-139">The description of the app.</span></span> <span data-ttu-id="40dfc-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-141">publisher</span><span class="sxs-lookup"><span data-stu-id="40dfc-141">Publisher</span></span>|<span data-ttu-id="40dfc-142">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-142">String</span></span>|<span data-ttu-id="40dfc-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="40dfc-143">The name of the app.</span></span> <span data-ttu-id="40dfc-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="40dfc-145">largeIcon</span></span>|[<span data-ttu-id="40dfc-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="40dfc-146">MimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="40dfc-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="40dfc-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="40dfc-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40dfc-149">createdDateTime</span></span>|<span data-ttu-id="40dfc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40dfc-150">DateTimeOffset</span></span>|<span data-ttu-id="40dfc-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="40dfc-151">The date and time when the page was created.</span></span> <span data-ttu-id="40dfc-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40dfc-153">lastModifiedDateTime</span></span>|<span data-ttu-id="40dfc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40dfc-154">DateTimeOffset</span></span>|<span data-ttu-id="40dfc-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="40dfc-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="40dfc-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="40dfc-157">isFeatured</span></span>|<span data-ttu-id="40dfc-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="40dfc-158">Boolean</span></span>|<span data-ttu-id="40dfc-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="40dfc-160">privacyInformationUrl</span></span>|<span data-ttu-id="40dfc-161">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-161">String</span></span>|<span data-ttu-id="40dfc-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="40dfc-162">The privacy statement Url.</span></span> <span data-ttu-id="40dfc-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="40dfc-164">informationUrl</span></span>|<span data-ttu-id="40dfc-165">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-165">String</span></span>|<span data-ttu-id="40dfc-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="40dfc-166">The more information Url.</span></span> <span data-ttu-id="40dfc-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-168">owner</span><span class="sxs-lookup"><span data-stu-id="40dfc-168">owner</span></span>|<span data-ttu-id="40dfc-169">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-169">String</span></span>|<span data-ttu-id="40dfc-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="40dfc-170">The owner of the timesheet.</span></span> <span data-ttu-id="40dfc-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-172">developer</span><span class="sxs-lookup"><span data-stu-id="40dfc-172">developer</span></span>|<span data-ttu-id="40dfc-173">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-173">String</span></span>|<span data-ttu-id="40dfc-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="40dfc-174">The name of the app.</span></span> <span data-ttu-id="40dfc-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-176">notes</span><span class="sxs-lookup"><span data-stu-id="40dfc-176">notes</span></span>|<span data-ttu-id="40dfc-177">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-177">String</span></span>|<span data-ttu-id="40dfc-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="40dfc-178">Notes for the app.</span></span> <span data-ttu-id="40dfc-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40dfc-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="40dfc-180">publishingState</span></span>|<span data-ttu-id="40dfc-181">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-181">String</span></span>|<span data-ttu-id="40dfc-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="40dfc-182">The publishing state for the app.</span></span> <span data-ttu-id="40dfc-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="40dfc-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="40dfc-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="40dfc-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="40dfc-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="40dfc-185">committedContentVersion</span></span>|<span data-ttu-id="40dfc-186">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-186">String</span></span>|<span data-ttu-id="40dfc-187">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="40dfc-187">The internal committed content version.</span></span> <span data-ttu-id="40dfc-188">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="40dfc-189">fileName</span><span class="sxs-lookup"><span data-stu-id="40dfc-189">FileName</span></span>|<span data-ttu-id="40dfc-190">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-190">String</span></span>|<span data-ttu-id="40dfc-191">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="40dfc-191">The name of the main Lob application file.</span></span> <span data-ttu-id="40dfc-192">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="40dfc-193">size</span><span class="sxs-lookup"><span data-stu-id="40dfc-193">size</span></span>|<span data-ttu-id="40dfc-194">Int64</span><span class="sxs-lookup"><span data-stu-id="40dfc-194">Int64</span></span>|<span data-ttu-id="40dfc-195">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="40dfc-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="40dfc-196">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="40dfc-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="40dfc-197">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="40dfc-197">applicableArchitectures</span></span>|<span data-ttu-id="40dfc-198">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-198">String</span></span>|<span data-ttu-id="40dfc-199">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="40dfc-199">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="40dfc-200">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="40dfc-200">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="40dfc-201">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="40dfc-201">applicableDeviceTypes</span></span>|<span data-ttu-id="40dfc-202">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-202">String</span></span>|<span data-ttu-id="40dfc-203">このアプリを実行できる Windows デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="40dfc-203">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="40dfc-204">可能な値は、`none`、`desktop`、`mobile`、`holographic`、`team` です。</span><span class="sxs-lookup"><span data-stu-id="40dfc-204">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="40dfc-205">identityName</span><span class="sxs-lookup"><span data-stu-id="40dfc-205">identityName</span></span>|<span data-ttu-id="40dfc-206">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-206">String</span></span>|<span data-ttu-id="40dfc-207">ID 名。</span><span class="sxs-lookup"><span data-stu-id="40dfc-207">The Identity Name.</span></span>|
|<span data-ttu-id="40dfc-208">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="40dfc-208">identityPublisherHash</span></span>|<span data-ttu-id="40dfc-209">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-209">String</span></span>|<span data-ttu-id="40dfc-210">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="40dfc-210">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="40dfc-211">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="40dfc-211">identityResourceIdentifier</span></span>|<span data-ttu-id="40dfc-212">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-212">String</span></span>|<span data-ttu-id="40dfc-213">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="40dfc-213">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="40dfc-214">isBundle</span><span class="sxs-lookup"><span data-stu-id="40dfc-214">isBundle</span></span>|<span data-ttu-id="40dfc-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="40dfc-215">Boolean</span></span>|<span data-ttu-id="40dfc-216">アプリがバンドルかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="40dfc-216">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="40dfc-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="40dfc-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="40dfc-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="40dfc-218">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="40dfc-219">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="40dfc-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="40dfc-220">identityVersion</span><span class="sxs-lookup"><span data-stu-id="40dfc-220">identityVersion</span></span>|<span data-ttu-id="40dfc-221">String</span><span class="sxs-lookup"><span data-stu-id="40dfc-221">String</span></span>|<span data-ttu-id="40dfc-222">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="40dfc-222">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="40dfc-223">応答</span><span class="sxs-lookup"><span data-stu-id="40dfc-223">Response</span></span>
<span data-ttu-id="40dfc-224">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="40dfc-224">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40dfc-225">例</span><span class="sxs-lookup"><span data-stu-id="40dfc-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="40dfc-226">要求</span><span class="sxs-lookup"><span data-stu-id="40dfc-226">Request</span></span>
<span data-ttu-id="40dfc-227">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40dfc-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1194

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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="40dfc-228">応答</span><span class="sxs-lookup"><span data-stu-id="40dfc-228">Response</span></span>
<span data-ttu-id="40dfc-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40dfc-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```



