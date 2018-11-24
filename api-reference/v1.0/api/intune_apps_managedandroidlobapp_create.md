# <a name="create-managedandroidlobapp"></a><span data-ttu-id="e59ac-101">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="e59ac-101">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="e59ac-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e59ac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e59ac-103">新しい [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e59ac-103">Create a new [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e59ac-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e59ac-104">Prerequisites</span></span>
<span data-ttu-id="e59ac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e59ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e59ac-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e59ac-107">Permission type</span></span>|<span data-ttu-id="e59ac-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e59ac-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e59ac-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e59ac-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e59ac-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e59ac-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e59ac-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e59ac-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e59ac-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e59ac-112">Not supported.</span></span>|
|<span data-ttu-id="e59ac-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e59ac-113">Application</span></span>|<span data-ttu-id="e59ac-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e59ac-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e59ac-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e59ac-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e59ac-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e59ac-116">Request headers</span></span>
|<span data-ttu-id="e59ac-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e59ac-117">Header</span></span>|<span data-ttu-id="e59ac-118">値</span><span class="sxs-lookup"><span data-stu-id="e59ac-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e59ac-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e59ac-119">Authorization</span></span>|<span data-ttu-id="e59ac-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e59ac-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e59ac-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e59ac-121">Accept</span></span>|<span data-ttu-id="e59ac-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e59ac-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e59ac-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e59ac-123">Request body</span></span>
<span data-ttu-id="e59ac-124">要求本文で、managedAndroidLobApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e59ac-124">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="e59ac-125">次の表に、managedAndroidLobApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e59ac-125">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="e59ac-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e59ac-126">Property</span></span>|<span data-ttu-id="e59ac-127">型</span><span class="sxs-lookup"><span data-stu-id="e59ac-127">Type</span></span>|<span data-ttu-id="e59ac-128">説明</span><span class="sxs-lookup"><span data-stu-id="e59ac-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e59ac-129">id</span><span class="sxs-lookup"><span data-stu-id="e59ac-129">id</span></span>|<span data-ttu-id="e59ac-130">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-130">String</span></span>|<span data-ttu-id="e59ac-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e59ac-131">Key of the entity.</span></span> <span data-ttu-id="e59ac-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e59ac-133">displayName</span></span>|<span data-ttu-id="e59ac-134">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-134">String</span></span>|<span data-ttu-id="e59ac-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="e59ac-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e59ac-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-137">description</span><span class="sxs-lookup"><span data-stu-id="e59ac-137">description</span></span>|<span data-ttu-id="e59ac-138">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-138">String</span></span>|<span data-ttu-id="e59ac-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e59ac-139">The description of the app.</span></span> <span data-ttu-id="e59ac-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-141">publisher</span><span class="sxs-lookup"><span data-stu-id="e59ac-141">publisher</span></span>|<span data-ttu-id="e59ac-142">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-142">String</span></span>|<span data-ttu-id="e59ac-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e59ac-143">The publisher of the app.</span></span> <span data-ttu-id="e59ac-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e59ac-145">largeIcon</span></span>|[<span data-ttu-id="e59ac-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e59ac-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="e59ac-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="e59ac-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e59ac-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e59ac-149">createdDateTime</span></span>|<span data-ttu-id="e59ac-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e59ac-150">DateTimeOffset</span></span>|<span data-ttu-id="e59ac-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e59ac-151">The date and time the app was created.</span></span> <span data-ttu-id="e59ac-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e59ac-153">lastModifiedDateTime</span></span>|<span data-ttu-id="e59ac-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e59ac-154">DateTimeOffset</span></span>|<span data-ttu-id="e59ac-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e59ac-155">The date and time the app was last modified.</span></span> <span data-ttu-id="e59ac-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e59ac-157">isFeatured</span></span>|<span data-ttu-id="e59ac-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e59ac-158">Boolean</span></span>|<span data-ttu-id="e59ac-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e59ac-160">privacyInformationUrl</span></span>|<span data-ttu-id="e59ac-161">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-161">String</span></span>|<span data-ttu-id="e59ac-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e59ac-162">The privacy statement Url.</span></span> <span data-ttu-id="e59ac-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e59ac-164">informationUrl</span></span>|<span data-ttu-id="e59ac-165">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-165">String</span></span>|<span data-ttu-id="e59ac-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e59ac-166">The more information Url.</span></span> <span data-ttu-id="e59ac-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-168">owner</span><span class="sxs-lookup"><span data-stu-id="e59ac-168">owner</span></span>|<span data-ttu-id="e59ac-169">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-169">String</span></span>|<span data-ttu-id="e59ac-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e59ac-170">The owner of the app.</span></span> <span data-ttu-id="e59ac-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-172">developer</span><span class="sxs-lookup"><span data-stu-id="e59ac-172">developer</span></span>|<span data-ttu-id="e59ac-173">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-173">String</span></span>|<span data-ttu-id="e59ac-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e59ac-174">The developer of the app.</span></span> <span data-ttu-id="e59ac-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-176">notes</span><span class="sxs-lookup"><span data-stu-id="e59ac-176">notes</span></span>|<span data-ttu-id="e59ac-177">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-177">String</span></span>|<span data-ttu-id="e59ac-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e59ac-178">Notes for the app.</span></span> <span data-ttu-id="e59ac-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e59ac-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="e59ac-180">publishingState</span></span>|[<span data-ttu-id="e59ac-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e59ac-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="e59ac-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e59ac-182">The publishing state for the app.</span></span> <span data-ttu-id="e59ac-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e59ac-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e59ac-184">[MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e59ac-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="e59ac-185">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e59ac-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e59ac-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e59ac-186">appAvailability</span></span>|[<span data-ttu-id="e59ac-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e59ac-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="e59ac-188">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="e59ac-188">The Application's availability.</span></span> <span data-ttu-id="e59ac-189">[ManagedApp](../resources/intune_apps_managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e59ac-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="e59ac-190">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="e59ac-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e59ac-191">version</span><span class="sxs-lookup"><span data-stu-id="e59ac-191">version</span></span>|<span data-ttu-id="e59ac-192">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-192">String</span></span>|<span data-ttu-id="e59ac-193">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e59ac-193">The Application's version.</span></span> <span data-ttu-id="e59ac-194">[managedApp](../resources/intune_apps_managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="e59ac-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e59ac-195">committedContentVersion</span></span>|<span data-ttu-id="e59ac-196">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-196">String</span></span>|<span data-ttu-id="e59ac-197">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e59ac-197">The internal committed content version.</span></span> <span data-ttu-id="e59ac-198">[managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e59ac-199">fileName</span><span class="sxs-lookup"><span data-stu-id="e59ac-199">fileName</span></span>|<span data-ttu-id="e59ac-200">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-200">String</span></span>|<span data-ttu-id="e59ac-201">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="e59ac-201">The name of the main Lob application file.</span></span> <span data-ttu-id="e59ac-202">[managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e59ac-203">size</span><span class="sxs-lookup"><span data-stu-id="e59ac-203">size</span></span>|<span data-ttu-id="e59ac-204">Int64</span><span class="sxs-lookup"><span data-stu-id="e59ac-204">Int64</span></span>|<span data-ttu-id="e59ac-205">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="e59ac-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="e59ac-206">[managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e59ac-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e59ac-207">packageId</span><span class="sxs-lookup"><span data-stu-id="e59ac-207">packageId</span></span>|<span data-ttu-id="e59ac-208">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-208">String</span></span>|<span data-ttu-id="e59ac-209">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="e59ac-209">The package identifier.</span></span>|
|<span data-ttu-id="e59ac-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e59ac-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e59ac-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e59ac-211">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="e59ac-212">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="e59ac-212">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e59ac-213">versionName</span><span class="sxs-lookup"><span data-stu-id="e59ac-213">versionName</span></span>|<span data-ttu-id="e59ac-214">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-214">String</span></span>|<span data-ttu-id="e59ac-215">管理対象 Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="e59ac-215">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e59ac-216">versionCode</span><span class="sxs-lookup"><span data-stu-id="e59ac-216">versionCode</span></span>|<span data-ttu-id="e59ac-217">String</span><span class="sxs-lookup"><span data-stu-id="e59ac-217">String</span></span>|<span data-ttu-id="e59ac-218">管理対象 Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="e59ac-218">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="e59ac-219">応答</span><span class="sxs-lookup"><span data-stu-id="e59ac-219">Response</span></span>
<span data-ttu-id="e59ac-220">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e59ac-220">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e59ac-221">例</span><span class="sxs-lookup"><span data-stu-id="e59ac-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="e59ac-222">要求</span><span class="sxs-lookup"><span data-stu-id="e59ac-222">Request</span></span>
<span data-ttu-id="e59ac-223">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e59ac-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1153

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="e59ac-224">応答</span><span class="sxs-lookup"><span data-stu-id="e59ac-224">Response</span></span>
<span data-ttu-id="e59ac-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e59ac-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1325

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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



