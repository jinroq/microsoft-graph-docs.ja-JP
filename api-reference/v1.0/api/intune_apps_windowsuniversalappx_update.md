# <a name="update-windowsuniversalappx"></a><span data-ttu-id="ed824-101">windowsUniversalAppX の更新</span><span class="sxs-lookup"><span data-stu-id="ed824-101">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="ed824-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed824-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed824-103">[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ed824-103">Update the properties of a [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed824-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ed824-104">Prerequisites</span></span>
<span data-ttu-id="ed824-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed824-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ed824-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed824-107">Permission type</span></span>|<span data-ttu-id="ed824-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed824-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed824-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed824-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ed824-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed824-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed824-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed824-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed824-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed824-112">Not supported.</span></span>|
|<span data-ttu-id="ed824-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed824-113">Application</span></span>|<span data-ttu-id="ed824-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed824-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed824-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed824-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ed824-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed824-116">Request headers</span></span>
|<span data-ttu-id="ed824-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed824-117">Header</span></span>|<span data-ttu-id="ed824-118">値</span><span class="sxs-lookup"><span data-stu-id="ed824-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed824-119">承認</span><span class="sxs-lookup"><span data-stu-id="ed824-119">Authorization</span></span>|<span data-ttu-id="ed824-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ed824-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed824-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ed824-121">Accept</span></span>|<span data-ttu-id="ed824-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="ed824-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed824-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed824-123">Request body</span></span>
<span data-ttu-id="ed824-124">要求本文で、[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed824-124">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="ed824-125">次の表に、[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ed824-125">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span></span>

|<span data-ttu-id="ed824-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed824-126">Property</span></span>|<span data-ttu-id="ed824-127">型</span><span class="sxs-lookup"><span data-stu-id="ed824-127">Type</span></span>|<span data-ttu-id="ed824-128">説明</span><span class="sxs-lookup"><span data-stu-id="ed824-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed824-129">id</span><span class="sxs-lookup"><span data-stu-id="ed824-129">id</span></span>|<span data-ttu-id="ed824-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-130">String</span></span>|<span data-ttu-id="ed824-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ed824-131">Key of the entity.</span></span> <span data-ttu-id="ed824-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ed824-133">displayName</span></span>|<span data-ttu-id="ed824-134">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-134">String</span></span>|<span data-ttu-id="ed824-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="ed824-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ed824-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-137">説明</span><span class="sxs-lookup"><span data-stu-id="ed824-137">description</span></span>|<span data-ttu-id="ed824-138">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-138">String</span></span>|<span data-ttu-id="ed824-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="ed824-139">The description of the app.</span></span> <span data-ttu-id="ed824-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-141">発行元</span><span class="sxs-lookup"><span data-stu-id="ed824-141">publisher</span></span>|<span data-ttu-id="ed824-142">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-142">String</span></span>|<span data-ttu-id="ed824-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="ed824-143">The publisher of the app.</span></span> <span data-ttu-id="ed824-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ed824-145">largeIcon</span></span>|[<span data-ttu-id="ed824-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ed824-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="ed824-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="ed824-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ed824-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed824-149">createdDateTime</span></span>|<span data-ttu-id="ed824-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed824-150">DateTimeOffset</span></span>|<span data-ttu-id="ed824-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ed824-151">The date and time the app was created.</span></span> <span data-ttu-id="ed824-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed824-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ed824-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed824-154">DateTimeOffset</span></span>|<span data-ttu-id="ed824-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="ed824-155">The date and time the app was last modified.</span></span> <span data-ttu-id="ed824-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ed824-157">isFeatured</span></span>|<span data-ttu-id="ed824-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="ed824-158">Boolean</span></span>|<span data-ttu-id="ed824-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ed824-160">privacyInformationUrl</span></span>|<span data-ttu-id="ed824-161">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-161">String</span></span>|<span data-ttu-id="ed824-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="ed824-162">The privacy statement Url.</span></span> <span data-ttu-id="ed824-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ed824-164">informationUrl</span></span>|<span data-ttu-id="ed824-165">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-165">String</span></span>|<span data-ttu-id="ed824-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="ed824-166">The more information Url.</span></span> <span data-ttu-id="ed824-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-168">所有者</span><span class="sxs-lookup"><span data-stu-id="ed824-168">owner</span></span>|<span data-ttu-id="ed824-169">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-169">String</span></span>|<span data-ttu-id="ed824-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="ed824-170">The owner of the app.</span></span> <span data-ttu-id="ed824-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-172">開発者</span><span class="sxs-lookup"><span data-stu-id="ed824-172">developer</span></span>|<span data-ttu-id="ed824-173">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-173">String</span></span>|<span data-ttu-id="ed824-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="ed824-174">The developer of the app.</span></span> <span data-ttu-id="ed824-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-176">メモ</span><span class="sxs-lookup"><span data-stu-id="ed824-176">notes</span></span>|<span data-ttu-id="ed824-177">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-177">String</span></span>|<span data-ttu-id="ed824-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="ed824-178">Notes for the app.</span></span> <span data-ttu-id="ed824-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ed824-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ed824-180">publishingState</span></span>|[<span data-ttu-id="ed824-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ed824-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="ed824-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="ed824-182">The publishing state for the app.</span></span> <span data-ttu-id="ed824-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="ed824-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ed824-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="ed824-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="ed824-185">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="ed824-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ed824-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ed824-186">committedContentVersion</span></span>|<span data-ttu-id="ed824-187">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-187">String</span></span>|<span data-ttu-id="ed824-188">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ed824-188">The internal committed content version.</span></span> <span data-ttu-id="ed824-189">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ed824-190">fileName</span><span class="sxs-lookup"><span data-stu-id="ed824-190">fileName</span></span>|<span data-ttu-id="ed824-191">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-191">String</span></span>|<span data-ttu-id="ed824-192">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="ed824-192">The name of the main Lob application file.</span></span> <span data-ttu-id="ed824-193">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ed824-194">サイズ</span><span class="sxs-lookup"><span data-stu-id="ed824-194">size</span></span>|<span data-ttu-id="ed824-195">Int64</span><span class="sxs-lookup"><span data-stu-id="ed824-195">Int64</span></span>|<span data-ttu-id="ed824-196">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="ed824-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="ed824-197">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ed824-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ed824-198">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ed824-198">applicableArchitectures</span></span>|[<span data-ttu-id="ed824-199">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="ed824-199">windowsArchitecture</span></span>](../resources/intune_apps_windowsarchitecture.md)|<span data-ttu-id="ed824-200">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="ed824-200">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ed824-201">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="ed824-201">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="ed824-202">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="ed824-202">applicableDeviceTypes</span></span>|[<span data-ttu-id="ed824-203">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="ed824-203">windowsDeviceType</span></span>](../resources/intune_apps_windowsdevicetype.md)|<span data-ttu-id="ed824-204">このアプリを実行できる Windows デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="ed824-204">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="ed824-205">可能な値は、`none`、`desktop`、`mobile`、`holographic`、`team` です。</span><span class="sxs-lookup"><span data-stu-id="ed824-205">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="ed824-206">identityName</span><span class="sxs-lookup"><span data-stu-id="ed824-206">identityName</span></span>|<span data-ttu-id="ed824-207">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-207">String</span></span>|<span data-ttu-id="ed824-208">ID 名。</span><span class="sxs-lookup"><span data-stu-id="ed824-208">The Identity Name.</span></span>|
|<span data-ttu-id="ed824-209">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="ed824-209">identityPublisherHash</span></span>|<span data-ttu-id="ed824-210">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-210">String</span></span>|<span data-ttu-id="ed824-211">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="ed824-211">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="ed824-212">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed824-212">identityResourceIdentifier</span></span>|<span data-ttu-id="ed824-213">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-213">String</span></span>|<span data-ttu-id="ed824-214">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="ed824-214">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="ed824-215">isBundle</span><span class="sxs-lookup"><span data-stu-id="ed824-215">isBundle</span></span>|<span data-ttu-id="ed824-216">ブール値</span><span class="sxs-lookup"><span data-stu-id="ed824-216">Boolean</span></span>|<span data-ttu-id="ed824-217">アプリがバンドルかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ed824-217">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="ed824-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ed824-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ed824-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ed824-219">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="ed824-220">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="ed824-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ed824-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ed824-221">identityVersion</span></span>|<span data-ttu-id="ed824-222">文字列</span><span class="sxs-lookup"><span data-stu-id="ed824-222">String</span></span>|<span data-ttu-id="ed824-223">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ed824-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ed824-224">応答</span><span class="sxs-lookup"><span data-stu-id="ed824-224">Response</span></span>
<span data-ttu-id="ed824-225">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="ed824-225">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed824-226">例</span><span class="sxs-lookup"><span data-stu-id="ed824-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed824-227">要求</span><span class="sxs-lookup"><span data-stu-id="ed824-227">Request</span></span>
<span data-ttu-id="ed824-228">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed824-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ed824-229">応答</span><span class="sxs-lookup"><span data-stu-id="ed824-229">Response</span></span>
<span data-ttu-id="ed824-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed824-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








