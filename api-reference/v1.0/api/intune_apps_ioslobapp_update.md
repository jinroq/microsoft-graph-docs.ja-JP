# <a name="update-ioslobapp"></a><span data-ttu-id="57c2b-101">iosLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="57c2b-101">Update iosLobApp</span></span>

> <span data-ttu-id="57c2b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="57c2b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57c2b-103">[iosLobApp](../resources/intune_apps_ioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="57c2b-103">Update the properties of a [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57c2b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="57c2b-104">Prerequisites</span></span>
<span data-ttu-id="57c2b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57c2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="57c2b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57c2b-107">Permission type</span></span>|<span data-ttu-id="57c2b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="57c2b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57c2b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57c2b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="57c2b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57c2b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="57c2b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57c2b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57c2b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57c2b-112">Not supported.</span></span>|
|<span data-ttu-id="57c2b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57c2b-113">Application</span></span>|<span data-ttu-id="57c2b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57c2b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57c2b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57c2b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="57c2b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57c2b-116">Request headers</span></span>
|<span data-ttu-id="57c2b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57c2b-117">Header</span></span>|<span data-ttu-id="57c2b-118">値</span><span class="sxs-lookup"><span data-stu-id="57c2b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57c2b-119">承認</span><span class="sxs-lookup"><span data-stu-id="57c2b-119">Authorization</span></span>|<span data-ttu-id="57c2b-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="57c2b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57c2b-121">承諾</span><span class="sxs-lookup"><span data-stu-id="57c2b-121">Accept</span></span>|<span data-ttu-id="57c2b-122">アプリケーションまたは JSON</span><span class="sxs-lookup"><span data-stu-id="57c2b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57c2b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="57c2b-123">Request body</span></span>
<span data-ttu-id="57c2b-124">要求本文で、[iosLobApp](../resources/intune_apps_ioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="57c2b-124">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>

<span data-ttu-id="57c2b-125">次の表に、[iosLobApp](../resources/intune_apps_ioslobapp.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="57c2b-125">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune_apps_ioslobapp.md).</span></span>

|<span data-ttu-id="57c2b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57c2b-126">Property</span></span>|<span data-ttu-id="57c2b-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="57c2b-127">Type</span></span>|<span data-ttu-id="57c2b-128">説明</span><span class="sxs-lookup"><span data-stu-id="57c2b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57c2b-129">ID</span><span class="sxs-lookup"><span data-stu-id="57c2b-129">id</span></span>|<span data-ttu-id="57c2b-130">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-130">String</span></span>|<span data-ttu-id="57c2b-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="57c2b-131">Key of the entity.</span></span> <span data-ttu-id="57c2b-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="57c2b-133">displayName</span></span>|<span data-ttu-id="57c2b-134">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-134">String</span></span>|<span data-ttu-id="57c2b-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="57c2b-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="57c2b-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-137">説明</span><span class="sxs-lookup"><span data-stu-id="57c2b-137">description</span></span>|<span data-ttu-id="57c2b-138">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-138">String</span></span>|<span data-ttu-id="57c2b-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="57c2b-139">The description of the app.</span></span> <span data-ttu-id="57c2b-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-141">パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="57c2b-141">publisher</span></span>|<span data-ttu-id="57c2b-142">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-142">String</span></span>|<span data-ttu-id="57c2b-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="57c2b-143">The publisher of the app.</span></span> <span data-ttu-id="57c2b-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="57c2b-145">largeIcon</span></span>|[<span data-ttu-id="57c2b-146">MIME コンテンツ</span><span class="sxs-lookup"><span data-stu-id="57c2b-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="57c2b-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="57c2b-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="57c2b-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57c2b-149">createdDateTime</span></span>|<span data-ttu-id="57c2b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57c2b-150">DateTimeOffset</span></span>|<span data-ttu-id="57c2b-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="57c2b-151">The date and time the app was created.</span></span> <span data-ttu-id="57c2b-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57c2b-153">lastModifiedDateTime</span></span>|<span data-ttu-id="57c2b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57c2b-154">DateTimeOffset</span></span>|<span data-ttu-id="57c2b-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="57c2b-155">The date and time the app was last modified.</span></span> <span data-ttu-id="57c2b-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="57c2b-157">isFeatured</span></span>|<span data-ttu-id="57c2b-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="57c2b-158">Boolean</span></span>|<span data-ttu-id="57c2b-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="57c2b-160">privacyInformationUrl</span></span>|<span data-ttu-id="57c2b-161">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-161">String</span></span>|<span data-ttu-id="57c2b-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="57c2b-162">The privacy statement Url.</span></span> <span data-ttu-id="57c2b-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="57c2b-164">informationUrl</span></span>|<span data-ttu-id="57c2b-165">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-165">String</span></span>|<span data-ttu-id="57c2b-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="57c2b-166">The more information Url.</span></span> <span data-ttu-id="57c2b-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-168">所有者</span><span class="sxs-lookup"><span data-stu-id="57c2b-168">owner</span></span>|<span data-ttu-id="57c2b-169">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-169">String</span></span>|<span data-ttu-id="57c2b-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="57c2b-170">The owner of the app.</span></span> <span data-ttu-id="57c2b-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-172">開発者</span><span class="sxs-lookup"><span data-stu-id="57c2b-172">developer</span></span>|<span data-ttu-id="57c2b-173">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-173">String</span></span>|<span data-ttu-id="57c2b-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="57c2b-174">The developer of the app.</span></span> <span data-ttu-id="57c2b-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-176">メモ</span><span class="sxs-lookup"><span data-stu-id="57c2b-176">notes</span></span>|<span data-ttu-id="57c2b-177">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-177">String</span></span>|<span data-ttu-id="57c2b-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="57c2b-178">Notes for the app.</span></span> <span data-ttu-id="57c2b-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="57c2b-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="57c2b-180">publishingState</span></span>|[<span data-ttu-id="57c2b-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="57c2b-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="57c2b-p114">アプリケーションの発行の状態です。アプリが公開されていない限り、アプリケーションを割り当てることができません。 [MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。使用可能な値は`notPublished`、`processing`、`published`です。</span><span class="sxs-lookup"><span data-stu-id="57c2b-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="57c2b-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="57c2b-186">committedContentVersion</span></span>|<span data-ttu-id="57c2b-187">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-187">String</span></span>|<span data-ttu-id="57c2b-188">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="57c2b-188">The internal committed content version.</span></span> <span data-ttu-id="57c2b-189">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="57c2b-190">fileName</span><span class="sxs-lookup"><span data-stu-id="57c2b-190">fileName</span></span>|<span data-ttu-id="57c2b-191">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-191">String</span></span>|<span data-ttu-id="57c2b-192">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="57c2b-192">The name of the main Lob application file.</span></span> <span data-ttu-id="57c2b-193">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="57c2b-194">サイズ</span><span class="sxs-lookup"><span data-stu-id="57c2b-194">size</span></span>|<span data-ttu-id="57c2b-195">Int64</span><span class="sxs-lookup"><span data-stu-id="57c2b-195">Int64</span></span>|<span data-ttu-id="57c2b-196">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="57c2b-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="57c2b-197">[mobileLobApp](../resources/intune_apps_mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="57c2b-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="57c2b-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="57c2b-198">bundleId</span></span>|<span data-ttu-id="57c2b-199">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-199">String</span></span>|<span data-ttu-id="57c2b-200">ID 名。</span><span class="sxs-lookup"><span data-stu-id="57c2b-200">The Identity Name.</span></span>|
|<span data-ttu-id="57c2b-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="57c2b-201">applicableDeviceType</span></span>|[<span data-ttu-id="57c2b-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="57c2b-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="57c2b-203">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="57c2b-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="57c2b-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="57c2b-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="57c2b-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="57c2b-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="57c2b-206">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="57c2b-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="57c2b-207">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="57c2b-207">expirationDateTime</span></span>|<span data-ttu-id="57c2b-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57c2b-208">DateTimeOffset</span></span>|<span data-ttu-id="57c2b-209">有効期限。</span><span class="sxs-lookup"><span data-stu-id="57c2b-209">The expiration time.</span></span>|
|<span data-ttu-id="57c2b-210">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="57c2b-210">versionNumber</span></span>|<span data-ttu-id="57c2b-211">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-211">String</span></span>|<span data-ttu-id="57c2b-212">iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="57c2b-212">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="57c2b-213">buildNumber</span><span class="sxs-lookup"><span data-stu-id="57c2b-213">buildNumber</span></span>|<span data-ttu-id="57c2b-214">文字列</span><span class="sxs-lookup"><span data-stu-id="57c2b-214">String</span></span>|<span data-ttu-id="57c2b-215">iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="57c2b-215">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="57c2b-216">応答</span><span class="sxs-lookup"><span data-stu-id="57c2b-216">Response</span></span>
<span data-ttu-id="57c2b-217">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosLobApp](../resources/intune_apps_ioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="57c2b-217">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57c2b-218">例</span><span class="sxs-lookup"><span data-stu-id="57c2b-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="57c2b-219">要求</span><span class="sxs-lookup"><span data-stu-id="57c2b-219">Request</span></span>
<span data-ttu-id="57c2b-220">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="57c2b-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1205

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

### <a name="response"></a><span data-ttu-id="57c2b-221">応答</span><span class="sxs-lookup"><span data-stu-id="57c2b-221">Response</span></span>
<span data-ttu-id="57c2b-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="57c2b-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








