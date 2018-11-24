# <a name="update-iosvppebook"></a><span data-ttu-id="0f09e-101">iosVppEBook の更新</span><span class="sxs-lookup"><span data-stu-id="0f09e-101">Update iosVppEBook</span></span>

> <span data-ttu-id="0f09e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f09e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f09e-103">[iosVppEBook](../resources/intune_books_iosvppebook.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0f09e-103">Update the properties of a [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f09e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="0f09e-104">Prerequisites</span></span>
<span data-ttu-id="0f09e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f09e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0f09e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f09e-107">Permission type</span></span>|<span data-ttu-id="0f09e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f09e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f09e-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f09e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0f09e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f09e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f09e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f09e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f09e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f09e-112">Not supported.</span></span>|
|<span data-ttu-id="0f09e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f09e-113">Application</span></span>|<span data-ttu-id="0f09e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f09e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f09e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f09e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="0f09e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f09e-116">Request headers</span></span>
|<span data-ttu-id="0f09e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f09e-117">Header</span></span>|<span data-ttu-id="0f09e-118">値</span><span class="sxs-lookup"><span data-stu-id="0f09e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f09e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f09e-119">Authorization</span></span>|<span data-ttu-id="0f09e-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0f09e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f09e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0f09e-121">Accept</span></span>|<span data-ttu-id="0f09e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0f09e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f09e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f09e-123">Request body</span></span>
<span data-ttu-id="0f09e-124">要求本文で、[iosVppEBook](../resources/intune_books_iosvppebook.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f09e-124">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>

<span data-ttu-id="0f09e-125">次の表に、[iosVppEBook](../resources/intune_books_iosvppebook.md) の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0f09e-125">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune_books_iosvppebook.md).</span></span>

|<span data-ttu-id="0f09e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f09e-126">Property</span></span>|<span data-ttu-id="0f09e-127">型</span><span class="sxs-lookup"><span data-stu-id="0f09e-127">Type</span></span>|<span data-ttu-id="0f09e-128">説明</span><span class="sxs-lookup"><span data-stu-id="0f09e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f09e-129">id</span><span class="sxs-lookup"><span data-stu-id="0f09e-129">id</span></span>|<span data-ttu-id="0f09e-130">String</span><span class="sxs-lookup"><span data-stu-id="0f09e-130">String</span></span>|<span data-ttu-id="0f09e-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0f09e-131">Key of the entity.</span></span> <span data-ttu-id="0f09e-132">[managedEBook](../resources/intune_books_managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f09e-132">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="0f09e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0f09e-133">displayName</span></span>|<span data-ttu-id="0f09e-134">String</span><span class="sxs-lookup"><span data-stu-id="0f09e-134">String</span></span>|<span data-ttu-id="0f09e-135">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="0f09e-135">Name of the eBook.</span></span> <span data-ttu-id="0f09e-136">[managedEBook](../resources/intune_books_managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f09e-136">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="0f09e-137">description</span><span class="sxs-lookup"><span data-stu-id="0f09e-137">description</span></span>|<span data-ttu-id="0f09e-138">String</span><span class="sxs-lookup"><span data-stu-id="0f09e-138">String</span></span>|<span data-ttu-id="0f09e-139">説明。</span><span class="sxs-lookup"><span data-stu-id="0f09e-139">Description.</span></span> <span data-ttu-id="0f09e-140">[managedEBook](../resources/intune_books_managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f09e-140">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="0f09e-141">publisher</span><span class="sxs-lookup"><span data-stu-id="0f09e-141">publisher</span></span>|<span data-ttu-id="0f09e-142">String</span><span class="sxs-lookup"><span data-stu-id="0f09e-142">String</span></span>|<span data-ttu-id="0f09e-143">発行元。</span><span class="sxs-lookup"><span data-stu-id="0f09e-143">Publisher.</span></span> <span data-ttu-id="0f09e-144">[managedEBook](../resources/intune_books_managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f09e-144">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="0f09e-145">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f09e-145">publishedDateTime</span></span>|<span data-ttu-id="0f09e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f09e-146">DateTimeOffset</span></span>|<span data-ttu-id="0f09e-147">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="0f09e-147">The date and time when the eBook was published.</span></span> <span data-ttu-id="0f09e-148">[managedEBook](../resources/intune_books_managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f09e-148">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="0f09e-149">largeCover</span><span class="sxs-lookup"><span data-stu-id="0f09e-149">largeCover</span></span>|[<span data-ttu-id="0f09e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f09e-150">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="0f09e-151">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="0f09e-151">Book cover.</span></span> <span data-ttu-id="0f09e-152">[managedEBook](../resources/intune_books_managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f09e-152">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="0f09e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f09e-153">createdDateTime</span></span>|<span data-ttu-id="0f09e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f09e-154">DateTimeOffset</span></span>|<span data-ttu-id="0f09e-155">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="0f09e-155">The date and time when the eBook file was created.</span></span> <span data-ttu-id="0f09e-156">[managedEBook](../resources/intune_books_managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f09e-156">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="0f09e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f09e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="0f09e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f09e-158">DateTimeOffset</span></span>|<span data-ttu-id="0f09e-159">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="0f09e-159">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="0f09e-160">[managedEBook](../resources/intune_books_managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f09e-160">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="0f09e-161">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0f09e-161">informationUrl</span></span>|<span data-ttu-id="0f09e-162">String</span><span class="sxs-lookup"><span data-stu-id="0f09e-162">String</span></span>|<span data-ttu-id="0f09e-163">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="0f09e-163">The more information Url.</span></span> <span data-ttu-id="0f09e-164">[managedEBook](../resources/intune_books_managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f09e-164">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="0f09e-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0f09e-165">privacyInformationUrl</span></span>|<span data-ttu-id="0f09e-166">String</span><span class="sxs-lookup"><span data-stu-id="0f09e-166">String</span></span>|<span data-ttu-id="0f09e-167">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="0f09e-167">The privacy statement Url.</span></span> <span data-ttu-id="0f09e-168">[managedEBook](../resources/intune_books_managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f09e-168">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="0f09e-169">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="0f09e-169">vppTokenId</span></span>|<span data-ttu-id="0f09e-170">Guid</span><span class="sxs-lookup"><span data-stu-id="0f09e-170">Guid</span></span>|<span data-ttu-id="0f09e-171">Vpp トークン ID。</span><span class="sxs-lookup"><span data-stu-id="0f09e-171">The Vpp token ID.</span></span>|
|<span data-ttu-id="0f09e-172">appleId</span><span class="sxs-lookup"><span data-stu-id="0f09e-172">appleId</span></span>|<span data-ttu-id="0f09e-173">String</span><span class="sxs-lookup"><span data-stu-id="0f09e-173">String</span></span>|<span data-ttu-id="0f09e-174">Vpp トークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="0f09e-174">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="0f09e-175">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="0f09e-175">vppOrganizationName</span></span>|<span data-ttu-id="0f09e-176">String</span><span class="sxs-lookup"><span data-stu-id="0f09e-176">String</span></span>|<span data-ttu-id="0f09e-177">Vpp トークンの組織の名前。</span><span class="sxs-lookup"><span data-stu-id="0f09e-177">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="0f09e-178">genres</span><span class="sxs-lookup"><span data-stu-id="0f09e-178">genres</span></span>|<span data-ttu-id="0f09e-179">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0f09e-179">String collection</span></span>|<span data-ttu-id="0f09e-180">ジャンル。</span><span class="sxs-lookup"><span data-stu-id="0f09e-180">Genres.</span></span>|
|<span data-ttu-id="0f09e-181">language</span><span class="sxs-lookup"><span data-stu-id="0f09e-181">language</span></span>|<span data-ttu-id="0f09e-182">String</span><span class="sxs-lookup"><span data-stu-id="0f09e-182">String</span></span>|<span data-ttu-id="0f09e-183">言語。</span><span class="sxs-lookup"><span data-stu-id="0f09e-183">Language.</span></span>|
|<span data-ttu-id="0f09e-184">seller</span><span class="sxs-lookup"><span data-stu-id="0f09e-184">seller</span></span>|<span data-ttu-id="0f09e-185">String</span><span class="sxs-lookup"><span data-stu-id="0f09e-185">String</span></span>|<span data-ttu-id="0f09e-186">販売元。</span><span class="sxs-lookup"><span data-stu-id="0f09e-186">Seller.</span></span>|
|<span data-ttu-id="0f09e-187">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0f09e-187">totalLicenseCount</span></span>|<span data-ttu-id="0f09e-188">Int32</span><span class="sxs-lookup"><span data-stu-id="0f09e-188">Int32</span></span>|<span data-ttu-id="0f09e-189">ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="0f09e-189">Total license count.</span></span>|
|<span data-ttu-id="0f09e-190">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0f09e-190">usedLicenseCount</span></span>|<span data-ttu-id="0f09e-191">Int32</span><span class="sxs-lookup"><span data-stu-id="0f09e-191">Int32</span></span>|<span data-ttu-id="0f09e-192">使用されているライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="0f09e-192">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="0f09e-193">応答</span><span class="sxs-lookup"><span data-stu-id="0f09e-193">Response</span></span>
<span data-ttu-id="0f09e-194">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosVppEBook](../resources/intune_books_iosvppebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0f09e-194">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune_books_iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f09e-195">例</span><span class="sxs-lookup"><span data-stu-id="0f09e-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f09e-196">要求</span><span class="sxs-lookup"><span data-stu-id="0f09e-196">Request</span></span>
<span data-ttu-id="0f09e-197">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f09e-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```

### <a name="response"></a><span data-ttu-id="0f09e-198">応答</span><span class="sxs-lookup"><span data-stu-id="0f09e-198">Response</span></span>
<span data-ttu-id="0f09e-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f09e-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```



