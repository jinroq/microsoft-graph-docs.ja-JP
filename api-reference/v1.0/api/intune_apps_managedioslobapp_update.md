# <a name="update-managedioslobapp"></a><span data-ttu-id="f133e-101">managedIOSLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="f133e-101">Update managedIOSLobApp</span></span>

> <span data-ttu-id="f133e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f133e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f133e-103">[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f133e-103">Update the properties of a [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f133e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="f133e-104">Prerequisites</span></span>
<span data-ttu-id="f133e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f133e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f133e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f133e-107">Permission type</span></span>|<span data-ttu-id="f133e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f133e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f133e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f133e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f133e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f133e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f133e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f133e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f133e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f133e-112">Not supported.</span></span>|
|<span data-ttu-id="f133e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f133e-113">Application</span></span>|<span data-ttu-id="f133e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f133e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f133e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f133e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f133e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f133e-116">Request headers</span></span>
|<span data-ttu-id="f133e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f133e-117">Header</span></span>|<span data-ttu-id="f133e-118">値</span><span class="sxs-lookup"><span data-stu-id="f133e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f133e-119">承認</span><span class="sxs-lookup"><span data-stu-id="f133e-119">Authorization</span></span>|<span data-ttu-id="f133e-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f133e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f133e-121">承諾</span><span class="sxs-lookup"><span data-stu-id="f133e-121">Accept</span></span>|<span data-ttu-id="f133e-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="f133e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f133e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f133e-123">Request body</span></span>
<span data-ttu-id="f133e-124">要求本文で、[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f133e-124">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>

<span data-ttu-id="f133e-125">次の表に、[managedDeviceOverview](../resources/intune_apps_managedioslobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f133e-125">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span></span>

|<span data-ttu-id="f133e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f133e-126">Property</span></span>|<span data-ttu-id="f133e-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="f133e-127">Type</span></span>|<span data-ttu-id="f133e-128">説明</span><span class="sxs-lookup"><span data-stu-id="f133e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f133e-129">ID</span><span class="sxs-lookup"><span data-stu-id="f133e-129">id</span></span>|<span data-ttu-id="f133e-130">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-130">String</span></span>|<span data-ttu-id="f133e-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f133e-131">Key of the entity.</span></span> <span data-ttu-id="f133e-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f133e-133">displayName</span></span>|<span data-ttu-id="f133e-134">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-134">String</span></span>|<span data-ttu-id="f133e-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f133e-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f133e-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-137">説明</span><span class="sxs-lookup"><span data-stu-id="f133e-137">description</span></span>|<span data-ttu-id="f133e-138">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-138">String</span></span>|<span data-ttu-id="f133e-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f133e-139">The description of the app.</span></span> <span data-ttu-id="f133e-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-141">パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="f133e-141">publisher</span></span>|<span data-ttu-id="f133e-142">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-142">String</span></span>|<span data-ttu-id="f133e-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f133e-143">The publisher of the app.</span></span> <span data-ttu-id="f133e-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f133e-145">largeIcon</span></span>|[<span data-ttu-id="f133e-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f133e-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="f133e-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="f133e-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f133e-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f133e-149">createdDateTime</span></span>|<span data-ttu-id="f133e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f133e-150">DateTimeOffset</span></span>|<span data-ttu-id="f133e-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f133e-151">The date and time the app was created.</span></span> <span data-ttu-id="f133e-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f133e-153">lastModifiedDateTime</span></span>|<span data-ttu-id="f133e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f133e-154">DateTimeOffset</span></span>|<span data-ttu-id="f133e-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f133e-155">The date and time the app was last modified.</span></span> <span data-ttu-id="f133e-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f133e-157">isFeatured</span></span>|<span data-ttu-id="f133e-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="f133e-158">Boolean</span></span>|<span data-ttu-id="f133e-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f133e-160">privacyInformationUrl</span></span>|<span data-ttu-id="f133e-161">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-161">String</span></span>|<span data-ttu-id="f133e-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f133e-162">The privacy statement Url.</span></span> <span data-ttu-id="f133e-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f133e-164">informationUrl</span></span>|<span data-ttu-id="f133e-165">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-165">String</span></span>|<span data-ttu-id="f133e-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f133e-166">The more information Url.</span></span> <span data-ttu-id="f133e-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-168">所有者</span><span class="sxs-lookup"><span data-stu-id="f133e-168">owner</span></span>|<span data-ttu-id="f133e-169">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-169">String</span></span>|<span data-ttu-id="f133e-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f133e-170">The owner of the app.</span></span> <span data-ttu-id="f133e-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-172">開発者</span><span class="sxs-lookup"><span data-stu-id="f133e-172">developer</span></span>|<span data-ttu-id="f133e-173">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-173">String</span></span>|<span data-ttu-id="f133e-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f133e-174">The developer of the app.</span></span> <span data-ttu-id="f133e-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-176">メモ</span><span class="sxs-lookup"><span data-stu-id="f133e-176">notes</span></span>|<span data-ttu-id="f133e-177">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-177">String</span></span>|<span data-ttu-id="f133e-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f133e-178">Notes for the app.</span></span> <span data-ttu-id="f133e-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f133e-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="f133e-180">publishingState</span></span>|[<span data-ttu-id="f133e-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f133e-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="f133e-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f133e-182">The publishing state for the app.</span></span> <span data-ttu-id="f133e-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f133e-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f133e-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="f133e-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="f133e-185">指定できる値は、`notPublished`、`processing`、`published`です。</span><span class="sxs-lookup"><span data-stu-id="f133e-185">The possible values are `notPublished`, `processing`, or `published`.</span></span>|
|<span data-ttu-id="f133e-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f133e-186">appAvailability</span></span>|[<span data-ttu-id="f133e-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f133e-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="f133e-188">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="f133e-188">The Application's availability.</span></span> <span data-ttu-id="f133e-189">[managedApp](../resources/intune_apps_managedapp.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="f133e-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="f133e-190">指定できる値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="f133e-190">The possible values are:</span></span>|
|<span data-ttu-id="f133e-191">バージョン</span><span class="sxs-lookup"><span data-stu-id="f133e-191">version</span></span>|<span data-ttu-id="f133e-192">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-192">String</span></span>|<span data-ttu-id="f133e-193">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f133e-193">The Application's version.</span></span> <span data-ttu-id="f133e-194">[managedApp](../resources/intune_apps_managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="f133e-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f133e-195">committedContentVersion</span></span>|<span data-ttu-id="f133e-196">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-196">String</span></span>|<span data-ttu-id="f133e-197">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f133e-197">The internal committed content version.</span></span> <span data-ttu-id="f133e-198">[managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f133e-199">fileName</span><span class="sxs-lookup"><span data-stu-id="f133e-199">fileName</span></span>|<span data-ttu-id="f133e-200">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-200">String</span></span>|<span data-ttu-id="f133e-201">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="f133e-201">The name of the main Lob application file.</span></span> <span data-ttu-id="f133e-202">[managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f133e-203">サイズ</span><span class="sxs-lookup"><span data-stu-id="f133e-203">size</span></span>|<span data-ttu-id="f133e-204">Int64</span><span class="sxs-lookup"><span data-stu-id="f133e-204">Int64</span></span>|<span data-ttu-id="f133e-205">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="f133e-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="f133e-206">[managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f133e-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f133e-207">bundleId</span><span class="sxs-lookup"><span data-stu-id="f133e-207">bundleId</span></span>|<span data-ttu-id="f133e-208">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-208">String</span></span>|<span data-ttu-id="f133e-209">ID 名。</span><span class="sxs-lookup"><span data-stu-id="f133e-209">The Identity Name.</span></span>|
|<span data-ttu-id="f133e-210">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f133e-210">applicableDeviceType</span></span>|[<span data-ttu-id="f133e-211">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f133e-211">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="f133e-212">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="f133e-212">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f133e-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f133e-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f133e-214">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f133e-214">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="f133e-215">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="f133e-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f133e-216">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f133e-216">expirationDateTime</span></span>|<span data-ttu-id="f133e-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f133e-217">DateTimeOffset</span></span>|<span data-ttu-id="f133e-218">有効期限。</span><span class="sxs-lookup"><span data-stu-id="f133e-218">The expiration time.</span></span>|
|<span data-ttu-id="f133e-219">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="f133e-219">versionNumber</span></span>|<span data-ttu-id="f133e-220">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-220">String</span></span>|<span data-ttu-id="f133e-221">管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="f133e-221">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f133e-222">buildNumber</span><span class="sxs-lookup"><span data-stu-id="f133e-222">buildNumber</span></span>|<span data-ttu-id="f133e-223">文字列</span><span class="sxs-lookup"><span data-stu-id="f133e-223">String</span></span>|<span data-ttu-id="f133e-224">管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="f133e-224">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="f133e-225">応答</span><span class="sxs-lookup"><span data-stu-id="f133e-225">Response</span></span>
<span data-ttu-id="f133e-226">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="f133e-226">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f133e-227">例</span><span class="sxs-lookup"><span data-stu-id="f133e-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="f133e-228">要求</span><span class="sxs-lookup"><span data-stu-id="f133e-228">Request</span></span>
<span data-ttu-id="f133e-229">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f133e-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1276

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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="f133e-230">応答</span><span class="sxs-lookup"><span data-stu-id="f133e-230">Response</span></span>
<span data-ttu-id="f133e-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f133e-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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



