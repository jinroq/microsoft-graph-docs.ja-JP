# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="b4fba-101">macOSOfficeSuiteApp の作成</span><span class="sxs-lookup"><span data-stu-id="b4fba-101">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="b4fba-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b4fba-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4fba-103">新しい [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b4fba-103">Create a new [plannerBucket](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4fba-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b4fba-104">Prerequisites</span></span>
<span data-ttu-id="b4fba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4fba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4fba-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4fba-107">Permission type</span></span>|<span data-ttu-id="b4fba-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4fba-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4fba-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4fba-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b4fba-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4fba-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4fba-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4fba-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4fba-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4fba-112">Not supported.</span></span>|
|<span data-ttu-id="b4fba-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4fba-113">Application</span></span>|<span data-ttu-id="b4fba-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4fba-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4fba-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4fba-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b4fba-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4fba-116">Request headers</span></span>
|<span data-ttu-id="b4fba-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4fba-117">Header</span></span>|<span data-ttu-id="b4fba-118">値</span><span class="sxs-lookup"><span data-stu-id="b4fba-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4fba-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4fba-119">Authorization</span></span>|<span data-ttu-id="b4fba-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b4fba-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b4fba-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b4fba-121">Accept</span></span>|<span data-ttu-id="b4fba-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b4fba-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4fba-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4fba-123">Request body</span></span>
<span data-ttu-id="b4fba-124">要求本文で、macOSOfficeSuiteApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b4fba-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="b4fba-125">次の表に、macOSOfficeSuiteApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b4fba-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="b4fba-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4fba-126">Property</span></span>|<span data-ttu-id="b4fba-127">型</span><span class="sxs-lookup"><span data-stu-id="b4fba-127">Type</span></span>|<span data-ttu-id="b4fba-128">説明</span><span class="sxs-lookup"><span data-stu-id="b4fba-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4fba-129">id</span><span class="sxs-lookup"><span data-stu-id="b4fba-129">id</span></span>|<span data-ttu-id="b4fba-130">String</span><span class="sxs-lookup"><span data-stu-id="b4fba-130">String</span></span>|<span data-ttu-id="b4fba-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b4fba-131">Name of the entity.</span></span> <span data-ttu-id="b4fba-132">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b4fba-133">displayName</span></span>|<span data-ttu-id="b4fba-134">String</span><span class="sxs-lookup"><span data-stu-id="b4fba-134">String</span></span>|<span data-ttu-id="b4fba-135">管理者が指定またはインポートした、アプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="b4fba-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b4fba-136">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-137">description</span><span class="sxs-lookup"><span data-stu-id="b4fba-137">description</span></span>|<span data-ttu-id="b4fba-138">String</span><span class="sxs-lookup"><span data-stu-id="b4fba-138">String</span></span>|<span data-ttu-id="b4fba-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b4fba-139">The description of the app.</span></span> <span data-ttu-id="b4fba-140">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-141">publisher</span><span class="sxs-lookup"><span data-stu-id="b4fba-141">Publisher</span></span>|<span data-ttu-id="b4fba-142">String</span><span class="sxs-lookup"><span data-stu-id="b4fba-142">String</span></span>|<span data-ttu-id="b4fba-143">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="b4fba-143">The name of the app.</span></span> <span data-ttu-id="b4fba-144">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b4fba-145">largeIcon</span></span>|[<span data-ttu-id="b4fba-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b4fba-146">MimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="b4fba-147">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="b4fba-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b4fba-148">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4fba-149">createdDateTime</span></span>|<span data-ttu-id="b4fba-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4fba-150">DateTimeOffset</span></span>|<span data-ttu-id="b4fba-151">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b4fba-151">The date and time when the page was created.</span></span> <span data-ttu-id="b4fba-152">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4fba-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b4fba-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4fba-154">DateTimeOffset</span></span>|<span data-ttu-id="b4fba-155">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="b4fba-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="b4fba-156">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b4fba-157">isFeatured</span></span>|<span data-ttu-id="b4fba-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fba-158">Boolean</span></span>|<span data-ttu-id="b4fba-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b4fba-160">privacyInformationUrl</span></span>|<span data-ttu-id="b4fba-161">String</span><span class="sxs-lookup"><span data-stu-id="b4fba-161">String</span></span>|<span data-ttu-id="b4fba-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="b4fba-162">The privacy statement Url.</span></span> <span data-ttu-id="b4fba-163">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b4fba-164">informationUrl</span></span>|<span data-ttu-id="b4fba-165">String</span><span class="sxs-lookup"><span data-stu-id="b4fba-165">String</span></span>|<span data-ttu-id="b4fba-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="b4fba-166">The more information Url.</span></span> <span data-ttu-id="b4fba-167">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-168">owner</span><span class="sxs-lookup"><span data-stu-id="b4fba-168">owner</span></span>|<span data-ttu-id="b4fba-169">String</span><span class="sxs-lookup"><span data-stu-id="b4fba-169">String</span></span>|<span data-ttu-id="b4fba-170">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="b4fba-170">The owner of the timesheet.</span></span> <span data-ttu-id="b4fba-171">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-172">developer</span><span class="sxs-lookup"><span data-stu-id="b4fba-172">developer</span></span>|<span data-ttu-id="b4fba-173">String</span><span class="sxs-lookup"><span data-stu-id="b4fba-173">String</span></span>|<span data-ttu-id="b4fba-174">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="b4fba-174">The name of the app.</span></span> <span data-ttu-id="b4fba-175">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-176">notes</span><span class="sxs-lookup"><span data-stu-id="b4fba-176">notes</span></span>|<span data-ttu-id="b4fba-177">String</span><span class="sxs-lookup"><span data-stu-id="b4fba-177">String</span></span>|<span data-ttu-id="b4fba-178">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="b4fba-178">Notes for the app.</span></span> <span data-ttu-id="b4fba-179">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b4fba-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4fba-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="b4fba-180">publishingState</span></span>|<span data-ttu-id="b4fba-181">String</span><span class="sxs-lookup"><span data-stu-id="b4fba-181">String</span></span>|<span data-ttu-id="b4fba-182">アプリの発行状態。</span><span class="sxs-lookup"><span data-stu-id="b4fba-182">The publishing state for the app.</span></span> <span data-ttu-id="b4fba-183">アプリが発行されていないと、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="b4fba-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b4fba-184">[mobileApp](../resources/intune_apps_mobileapp.md) から継承します。可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="b4fba-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="b4fba-185">応答</span><span class="sxs-lookup"><span data-stu-id="b4fba-185">Response</span></span>
<span data-ttu-id="b4fba-186">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b4fba-186">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4fba-187">例</span><span class="sxs-lookup"><span data-stu-id="b4fba-187">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4fba-188">要求</span><span class="sxs-lookup"><span data-stu-id="b4fba-188">Request</span></span>
<span data-ttu-id="b4fba-189">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4fba-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 648

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

### <a name="response"></a><span data-ttu-id="b4fba-190">応答</span><span class="sxs-lookup"><span data-stu-id="b4fba-190">Response</span></span>
<span data-ttu-id="b4fba-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b4fba-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



