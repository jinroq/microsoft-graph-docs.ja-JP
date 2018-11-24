# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="c0ece-101">macOSOfficeSuiteApp の作成</span><span class="sxs-lookup"><span data-stu-id="c0ece-101">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="c0ece-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0ece-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0ece-103">新しい [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c0ece-103">Create a new [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0ece-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="c0ece-104">Prerequisites</span></span>
<span data-ttu-id="c0ece-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0ece-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c0ece-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0ece-107">Permission type</span></span>|<span data-ttu-id="c0ece-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0ece-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0ece-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0ece-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c0ece-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0ece-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c0ece-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0ece-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0ece-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0ece-112">Not supported.</span></span>|
|<span data-ttu-id="c0ece-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0ece-113">Application</span></span>|<span data-ttu-id="c0ece-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0ece-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0ece-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0ece-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c0ece-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0ece-116">Request headers</span></span>
|<span data-ttu-id="c0ece-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0ece-117">Header</span></span>|<span data-ttu-id="c0ece-118">値</span><span class="sxs-lookup"><span data-stu-id="c0ece-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0ece-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0ece-119">Authorization</span></span>|<span data-ttu-id="c0ece-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c0ece-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0ece-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c0ece-121">Accept</span></span>|<span data-ttu-id="c0ece-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c0ece-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0ece-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0ece-123">Request body</span></span>
<span data-ttu-id="c0ece-124">要求本文で、macOSOfficeSuiteApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0ece-124">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="c0ece-125">次の表に、macOSOfficeSuiteApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c0ece-125">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="c0ece-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0ece-126">Property</span></span>|<span data-ttu-id="c0ece-127">型</span><span class="sxs-lookup"><span data-stu-id="c0ece-127">Type</span></span>|<span data-ttu-id="c0ece-128">説明</span><span class="sxs-lookup"><span data-stu-id="c0ece-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0ece-129">id</span><span class="sxs-lookup"><span data-stu-id="c0ece-129">id</span></span>|<span data-ttu-id="c0ece-130">String</span><span class="sxs-lookup"><span data-stu-id="c0ece-130">String</span></span>|<span data-ttu-id="c0ece-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c0ece-131">Key of the entity.</span></span> <span data-ttu-id="c0ece-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c0ece-133">displayName</span></span>|<span data-ttu-id="c0ece-134">String</span><span class="sxs-lookup"><span data-stu-id="c0ece-134">String</span></span>|<span data-ttu-id="c0ece-135">管理者が指定またはインポートした、アプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="c0ece-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c0ece-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-137">description</span><span class="sxs-lookup"><span data-stu-id="c0ece-137">description</span></span>|<span data-ttu-id="c0ece-138">String</span><span class="sxs-lookup"><span data-stu-id="c0ece-138">String</span></span>|<span data-ttu-id="c0ece-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="c0ece-139">The description of the app.</span></span> <span data-ttu-id="c0ece-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-141">publisher</span><span class="sxs-lookup"><span data-stu-id="c0ece-141">publisher</span></span>|<span data-ttu-id="c0ece-142">String</span><span class="sxs-lookup"><span data-stu-id="c0ece-142">String</span></span>|<span data-ttu-id="c0ece-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="c0ece-143">The publisher of the app.</span></span> <span data-ttu-id="c0ece-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c0ece-145">largeIcon</span></span>|[<span data-ttu-id="c0ece-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c0ece-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="c0ece-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="c0ece-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c0ece-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0ece-149">createdDateTime</span></span>|<span data-ttu-id="c0ece-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0ece-150">DateTimeOffset</span></span>|<span data-ttu-id="c0ece-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c0ece-151">The date and time the app was created.</span></span> <span data-ttu-id="c0ece-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0ece-153">lastModifiedDateTime</span></span>|<span data-ttu-id="c0ece-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0ece-154">DateTimeOffset</span></span>|<span data-ttu-id="c0ece-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="c0ece-155">The date and time the app was last modified.</span></span> <span data-ttu-id="c0ece-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c0ece-157">isFeatured</span></span>|<span data-ttu-id="c0ece-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0ece-158">Boolean</span></span>|<span data-ttu-id="c0ece-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c0ece-160">privacyInformationUrl</span></span>|<span data-ttu-id="c0ece-161">String</span><span class="sxs-lookup"><span data-stu-id="c0ece-161">String</span></span>|<span data-ttu-id="c0ece-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="c0ece-162">The privacy statement Url.</span></span> <span data-ttu-id="c0ece-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c0ece-164">informationUrl</span></span>|<span data-ttu-id="c0ece-165">String</span><span class="sxs-lookup"><span data-stu-id="c0ece-165">String</span></span>|<span data-ttu-id="c0ece-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="c0ece-166">The more information Url.</span></span> <span data-ttu-id="c0ece-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-168">owner</span><span class="sxs-lookup"><span data-stu-id="c0ece-168">owner</span></span>|<span data-ttu-id="c0ece-169">String</span><span class="sxs-lookup"><span data-stu-id="c0ece-169">String</span></span>|<span data-ttu-id="c0ece-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="c0ece-170">The owner of the app.</span></span> <span data-ttu-id="c0ece-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-172">developer</span><span class="sxs-lookup"><span data-stu-id="c0ece-172">developer</span></span>|<span data-ttu-id="c0ece-173">String</span><span class="sxs-lookup"><span data-stu-id="c0ece-173">String</span></span>|<span data-ttu-id="c0ece-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="c0ece-174">The developer of the app.</span></span> <span data-ttu-id="c0ece-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-176">notes</span><span class="sxs-lookup"><span data-stu-id="c0ece-176">notes</span></span>|<span data-ttu-id="c0ece-177">String</span><span class="sxs-lookup"><span data-stu-id="c0ece-177">String</span></span>|<span data-ttu-id="c0ece-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="c0ece-178">Notes for the app.</span></span> <span data-ttu-id="c0ece-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c0ece-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c0ece-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="c0ece-180">publishingState</span></span>|[<span data-ttu-id="c0ece-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c0ece-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="c0ece-182">アプリの発行状態。</span><span class="sxs-lookup"><span data-stu-id="c0ece-182">The publishing state for the app.</span></span> <span data-ttu-id="c0ece-183">アプリが発行されていないと、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="c0ece-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c0ece-184">[MobileApp](../resources/intune_apps_mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c0ece-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="c0ece-185">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="c0ece-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="c0ece-186">応答</span><span class="sxs-lookup"><span data-stu-id="c0ece-186">Response</span></span>
<span data-ttu-id="c0ece-187">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c0ece-187">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0ece-188">例</span><span class="sxs-lookup"><span data-stu-id="c0ece-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0ece-189">要求</span><span class="sxs-lookup"><span data-stu-id="c0ece-189">Request</span></span>
<span data-ttu-id="c0ece-190">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0ece-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 584

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="c0ece-191">応答</span><span class="sxs-lookup"><span data-stu-id="c0ece-191">Response</span></span>
<span data-ttu-id="c0ece-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0ece-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 756

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "publishingState": "processing"
}
```



