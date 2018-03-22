# <a name="update-iosvppapp"></a><span data-ttu-id="d128b-101">iosVppApp の更新</span><span class="sxs-lookup"><span data-stu-id="d128b-101">Update iosVppApp</span></span>

> <span data-ttu-id="d128b-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d128b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d128b-103">[iosVppApp](../resources/intune_apps_iosvppapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d128b-103">Update the properties of a [calendar](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d128b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="d128b-104">Prerequisites</span></span>
<span data-ttu-id="d128b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d128b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d128b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d128b-107">Permission type</span></span>|<span data-ttu-id="d128b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d128b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d128b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d128b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d128b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d128b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d128b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d128b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d128b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d128b-112">Not supported.</span></span>|
|<span data-ttu-id="d128b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d128b-113">Application</span></span>|<span data-ttu-id="d128b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d128b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d128b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d128b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d128b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d128b-116">Request headers</span></span>
|<span data-ttu-id="d128b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d128b-117">Header</span></span>|<span data-ttu-id="d128b-118">値</span><span class="sxs-lookup"><span data-stu-id="d128b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d128b-119">承認</span><span class="sxs-lookup"><span data-stu-id="d128b-119">Authorization</span></span>|<span data-ttu-id="d128b-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="d128b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d128b-121">承諾</span><span class="sxs-lookup"><span data-stu-id="d128b-121">Accept</span></span>|<span data-ttu-id="d128b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d128b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d128b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d128b-123">Request body</span></span>
<span data-ttu-id="d128b-124">要求本文で、[iosVppApp](../resources/intune_apps_iosvppapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d128b-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_iosvppapp.md) object.</span></span>

<span data-ttu-id="d128b-125">次の表に、[iosVppApp](../resources/intune_apps_iosvppapp.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d128b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d128b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d128b-126">Property</span></span>|<span data-ttu-id="d128b-127">型</span><span class="sxs-lookup"><span data-stu-id="d128b-127">Type</span></span>|<span data-ttu-id="d128b-128">説明</span><span class="sxs-lookup"><span data-stu-id="d128b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d128b-129">id</span><span class="sxs-lookup"><span data-stu-id="d128b-129">id</span></span>|<span data-ttu-id="d128b-130">String</span><span class="sxs-lookup"><span data-stu-id="d128b-130">String</span></span>|<span data-ttu-id="d128b-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d128b-131">Name of the entity.</span></span> <span data-ttu-id="d128b-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d128b-133">displayName</span></span>|<span data-ttu-id="d128b-134">String</span><span class="sxs-lookup"><span data-stu-id="d128b-134">String</span></span>|<span data-ttu-id="d128b-135">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="d128b-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d128b-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-137">description</span><span class="sxs-lookup"><span data-stu-id="d128b-137">description</span></span>|<span data-ttu-id="d128b-138">String</span><span class="sxs-lookup"><span data-stu-id="d128b-138">String</span></span>|<span data-ttu-id="d128b-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="d128b-139">The description of the app.</span></span> <span data-ttu-id="d128b-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-141">publisher</span><span class="sxs-lookup"><span data-stu-id="d128b-141">Publisher</span></span>|<span data-ttu-id="d128b-142">String</span><span class="sxs-lookup"><span data-stu-id="d128b-142">String</span></span>|<span data-ttu-id="d128b-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="d128b-143">The name of the app.</span></span> <span data-ttu-id="d128b-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d128b-145">largeIcon</span></span>|[<span data-ttu-id="d128b-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d128b-146">MimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="d128b-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="d128b-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d128b-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d128b-149">createdDateTime</span></span>|<span data-ttu-id="d128b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d128b-150">DateTimeOffset</span></span>|<span data-ttu-id="d128b-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d128b-151">The date and time when the page was created.</span></span> <span data-ttu-id="d128b-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d128b-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d128b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d128b-154">DateTimeOffset</span></span>|<span data-ttu-id="d128b-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="d128b-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="d128b-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d128b-157">isFeatured</span></span>|<span data-ttu-id="d128b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d128b-158">Boolean</span></span>|<span data-ttu-id="d128b-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d128b-160">privacyInformationUrl</span></span>|<span data-ttu-id="d128b-161">String</span><span class="sxs-lookup"><span data-stu-id="d128b-161">String</span></span>|<span data-ttu-id="d128b-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="d128b-162">The privacy statement Url.</span></span> <span data-ttu-id="d128b-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d128b-164">informationUrl</span></span>|<span data-ttu-id="d128b-165">String</span><span class="sxs-lookup"><span data-stu-id="d128b-165">String</span></span>|<span data-ttu-id="d128b-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="d128b-166">The more information Url.</span></span> <span data-ttu-id="d128b-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-168">owner</span><span class="sxs-lookup"><span data-stu-id="d128b-168">owner</span></span>|<span data-ttu-id="d128b-169">String</span><span class="sxs-lookup"><span data-stu-id="d128b-169">String</span></span>|<span data-ttu-id="d128b-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="d128b-170">The owner of the timesheet.</span></span> <span data-ttu-id="d128b-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-172">developer</span><span class="sxs-lookup"><span data-stu-id="d128b-172">developer</span></span>|<span data-ttu-id="d128b-173">String</span><span class="sxs-lookup"><span data-stu-id="d128b-173">String</span></span>|<span data-ttu-id="d128b-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="d128b-174">The name of the app.</span></span> <span data-ttu-id="d128b-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-176">notes</span><span class="sxs-lookup"><span data-stu-id="d128b-176">notes</span></span>|<span data-ttu-id="d128b-177">String</span><span class="sxs-lookup"><span data-stu-id="d128b-177">String</span></span>|<span data-ttu-id="d128b-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="d128b-178">Notes for the app.</span></span> <span data-ttu-id="d128b-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d128b-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d128b-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="d128b-180">publishingState</span></span>|<span data-ttu-id="d128b-181">String</span><span class="sxs-lookup"><span data-stu-id="d128b-181">String</span></span>|<span data-ttu-id="d128b-182">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="d128b-182">The publishing state for the app.</span></span> <span data-ttu-id="d128b-183">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="d128b-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d128b-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="d128b-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d128b-185">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d128b-185">usedLicenseCount</span></span>|<span data-ttu-id="d128b-186">Int32</span><span class="sxs-lookup"><span data-stu-id="d128b-186">Int32</span></span>|<span data-ttu-id="d128b-187">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="d128b-187">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="d128b-188">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d128b-188">totalLicenseCount</span></span>|<span data-ttu-id="d128b-189">Int32</span><span class="sxs-lookup"><span data-stu-id="d128b-189">Int32</span></span>|<span data-ttu-id="d128b-190">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="d128b-190">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="d128b-191">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="d128b-191">releaseDateTime</span></span>|<span data-ttu-id="d128b-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d128b-192">DateTimeOffset</span></span>|<span data-ttu-id="d128b-193">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="d128b-193">The VPP application release date and time.</span></span>|
|<span data-ttu-id="d128b-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d128b-194">appStoreUrl</span></span>|<span data-ttu-id="d128b-195">String</span><span class="sxs-lookup"><span data-stu-id="d128b-195">String</span></span>|<span data-ttu-id="d128b-196">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="d128b-196">The store URL.</span></span>|
|<span data-ttu-id="d128b-197">licensingType</span><span class="sxs-lookup"><span data-stu-id="d128b-197">licensingType</span></span>|[<span data-ttu-id="d128b-198">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="d128b-198">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="d128b-199">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="d128b-199">The supported License Type.</span></span>|
|<span data-ttu-id="d128b-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="d128b-200">applicableDeviceType</span></span>|[<span data-ttu-id="d128b-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d128b-201">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="d128b-202">該当する iOS デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="d128b-202">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="d128b-203">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="d128b-203">vppTokenOrganizationName</span></span>|<span data-ttu-id="d128b-204">String</span><span class="sxs-lookup"><span data-stu-id="d128b-204">String</span></span>|<span data-ttu-id="d128b-205">Apple ボリューム購入プログラムのトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="d128b-205">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="d128b-206">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="d128b-206">vppTokenAccountType</span></span>|<span data-ttu-id="d128b-207">String</span><span class="sxs-lookup"><span data-stu-id="d128b-207">String</span></span>|<span data-ttu-id="d128b-208">特定の Apple ボリューム購入プログラムのトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="d128b-208">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="d128b-209">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="d128b-209">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="d128b-210">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="d128b-210">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="d128b-211">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="d128b-211">vppTokenAppleId</span></span>|<span data-ttu-id="d128b-212">String</span><span class="sxs-lookup"><span data-stu-id="d128b-212">String</span></span>|<span data-ttu-id="d128b-213">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="d128b-213">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="d128b-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="d128b-214">bundleId</span></span>|<span data-ttu-id="d128b-215">String</span><span class="sxs-lookup"><span data-stu-id="d128b-215">String</span></span>|<span data-ttu-id="d128b-216">ID 名。</span><span class="sxs-lookup"><span data-stu-id="d128b-216">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="d128b-217">応答</span><span class="sxs-lookup"><span data-stu-id="d128b-217">Response</span></span>
<span data-ttu-id="d128b-218">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosVppApp](../resources/intune_apps_iosvppapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="d128b-218">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d128b-219">例</span><span class="sxs-lookup"><span data-stu-id="d128b-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="d128b-220">要求</span><span class="sxs-lookup"><span data-stu-id="d128b-220">Request</span></span>
<span data-ttu-id="d128b-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d128b-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1238

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

### <a name="response"></a><span data-ttu-id="d128b-222">応答</span><span class="sxs-lookup"><span data-stu-id="d128b-222">Response</span></span>
<span data-ttu-id="d128b-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d128b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



