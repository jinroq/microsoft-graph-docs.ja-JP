# <a name="get-photo"></a><span data-ttu-id="e72b8-101">写真を取得する</span><span class="sxs-lookup"><span data-stu-id="e72b8-101">Get photo</span></span>

<span data-ttu-id="e72b8-102">指定した [profilePhoto](../resources/profilephoto.md) またはそのメタデータ (profilePhoto プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="e72b8-102">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="e72b8-103">**注**: バージョン 1.0 のこの操作では、ユーザーの職場用または学校用メールボックスのみがサポートされ、個人用メールボックスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e72b8-103">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="e72b8-104">Office 365 上でサポートされている HD Photo のサイズは次のとおりです: '48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。</span><span class="sxs-lookup"><span data-stu-id="e72b8-104">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="e72b8-105">写真が Azure Active Directory に格納されている場合は、サイズに関する制限はありません。</span><span class="sxs-lookup"><span data-stu-id="e72b8-105">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="e72b8-106">使用可能な最大の写真のメタデータを取得したり、サイズを指定してその写真サイズのメタデータを取得したりできます。</span><span class="sxs-lookup"><span data-stu-id="e72b8-106">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="e72b8-107">要求したサイズが使用できない場合でも、アップロードされて使用可能になっている、より小さいサイズを取得できます。</span><span class="sxs-lookup"><span data-stu-id="e72b8-107">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="e72b8-108">たとえば、アップロードした写真が 504x504 ピクセルの場合は、648×648 を除くすべてのサイズの写真がダウンロード可能になります。</span><span class="sxs-lookup"><span data-stu-id="e72b8-108">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="e72b8-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e72b8-109">Permissions</span></span>

<span data-ttu-id="e72b8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e72b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e72b8-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e72b8-112">Permission type</span></span>      | <span data-ttu-id="e72b8-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e72b8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e72b8-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e72b8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e72b8-115">**user** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="e72b8-115">For **user** resource:</span></span><br/><span data-ttu-id="e72b8-116">User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e72b8-116">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e72b8-117">**group** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="e72b8-117">For **group** resource:</span></span><br /><span data-ttu-id="e72b8-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e72b8-118">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e72b8-119">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="e72b8-119">For **contact** resource:</span></span><br /><span data-ttu-id="e72b8-120">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e72b8-120">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="e72b8-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e72b8-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e72b8-122">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="e72b8-122">Not supported</span></span> |
|<span data-ttu-id="e72b8-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e72b8-123">Application</span></span>                        | <span data-ttu-id="e72b8-124">**user** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="e72b8-124">For **user** resource:</span></span><br/><span data-ttu-id="e72b8-125">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e72b8-125">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e72b8-126">**group** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="e72b8-126">For **group** resource:</span></span><br /><span data-ttu-id="e72b8-127">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e72b8-127">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e72b8-128">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="e72b8-128">For **contact** resource:</span></span><br /><span data-ttu-id="e72b8-129">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e72b8-129">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="e72b8-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e72b8-130">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="e72b8-131">写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="e72b8-131">Get the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="e72b8-132">写真のメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="e72b8-132">Get the metadata of the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /me/photos
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="e72b8-133">特定の写真サイズのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="e72b8-133">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
GET /me/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contacts/{id}/photos/{size}
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="e72b8-134">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="e72b8-134">Path parameters</span></span>

|<span data-ttu-id="e72b8-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e72b8-135">Parameter</span></span>|<span data-ttu-id="e72b8-136">型</span><span class="sxs-lookup"><span data-stu-id="e72b8-136">Type</span></span>|<span data-ttu-id="e72b8-137">説明</span><span class="sxs-lookup"><span data-stu-id="e72b8-137">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e72b8-138">size</span><span class="sxs-lookup"><span data-stu-id="e72b8-138">size</span></span>  |<span data-ttu-id="e72b8-139">String</span><span class="sxs-lookup"><span data-stu-id="e72b8-139">String</span></span>  | <span data-ttu-id="e72b8-140">写真のサイズ。</span><span class="sxs-lookup"><span data-stu-id="e72b8-140">A photo size.</span></span> <span data-ttu-id="e72b8-141">Office 365 上でサポートされている HD Photo のサイズは次のとおりです: '48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。</span><span class="sxs-lookup"><span data-stu-id="e72b8-141">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="e72b8-142">写真が Azure Active Directory に格納されている場合は、サイズに関する制限はありません。</span><span class="sxs-lookup"><span data-stu-id="e72b8-142">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e72b8-143">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e72b8-143">Optional query parameters</span></span>
<span data-ttu-id="e72b8-144">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e72b8-144">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e72b8-145">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e72b8-145">Request headers</span></span>
| <span data-ttu-id="e72b8-146">名前</span><span class="sxs-lookup"><span data-stu-id="e72b8-146">Name</span></span>       | <span data-ttu-id="e72b8-147">型</span><span class="sxs-lookup"><span data-stu-id="e72b8-147">Type</span></span> | <span data-ttu-id="e72b8-148">説明</span><span class="sxs-lookup"><span data-stu-id="e72b8-148">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e72b8-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="e72b8-149">Authorization</span></span>  | <span data-ttu-id="e72b8-150">string</span><span class="sxs-lookup"><span data-stu-id="e72b8-150">string</span></span>  | <span data-ttu-id="e72b8-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e72b8-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e72b8-153">要求本文</span><span class="sxs-lookup"><span data-stu-id="e72b8-153">Request body</span></span>
<span data-ttu-id="e72b8-154">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e72b8-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e72b8-155">応答</span><span class="sxs-lookup"><span data-stu-id="e72b8-155">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="e72b8-156">写真の取得に対する応答</span><span class="sxs-lookup"><span data-stu-id="e72b8-156">Response for getting the photo</span></span>
<span data-ttu-id="e72b8-p106">成功した場合、このメソッドは `200 OK` 応答コードと、要求した写真のバイナリ データを応答本文で返します。写真が存在しない場合、この操作により `404 Not Found` が返されます。</span><span class="sxs-lookup"><span data-stu-id="e72b8-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="e72b8-159">写真のメタデータの取得に対する応答</span><span class="sxs-lookup"><span data-stu-id="e72b8-159">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="e72b8-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [profilePhoto](../resources/profilePhoto.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e72b8-160">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilePhoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e72b8-161">例</span><span class="sxs-lookup"><span data-stu-id="e72b8-161">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e72b8-162">要求 1</span><span class="sxs-lookup"><span data-stu-id="e72b8-162">Request 1</span></span>
<span data-ttu-id="e72b8-163">この要求では、サインインしているユーザーの写真を利用可能な最大のサイズで取得します。</span><span class="sxs-lookup"><span data-stu-id="e72b8-163">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="e72b8-164">応答 1</span><span class="sxs-lookup"><span data-stu-id="e72b8-164">Response 1</span></span>
<span data-ttu-id="e72b8-p107">要求した写真のバイナリ データが含まれています。HTTP 応答コードは 200 です。</span><span class="sxs-lookup"><span data-stu-id="e72b8-p107">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="e72b8-167">要求 2</span><span class="sxs-lookup"><span data-stu-id="e72b8-167">Request 2</span></span>
<span data-ttu-id="e72b8-168">この要求は、サインインしているユーザーの 48x48 の写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="e72b8-168">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="e72b8-169">応答 2</span><span class="sxs-lookup"><span data-stu-id="e72b8-169">Response 2</span></span>
<span data-ttu-id="e72b8-p108">要求した 48x48 の写真のバイナリ データが含まれています。HTTP 応答コードは 200 です。</span><span class="sxs-lookup"><span data-stu-id="e72b8-p108">Contains the binary data of the requested 48x48 photo. The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="e72b8-172">要求 3</span><span class="sxs-lookup"><span data-stu-id="e72b8-172">Request 3</span></span>
<span data-ttu-id="e72b8-173">この要求は、サインインしているユーザーのユーザー写真のメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="e72b8-173">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="e72b8-174">応答 3</span><span class="sxs-lookup"><span data-stu-id="e72b8-174">Response 3</span></span>

<span data-ttu-id="e72b8-p109">次の応答データは、写真のメタデータを示しています。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e72b8-p109">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="e72b8-p110">次の応答データは、そのユーザーの写真がまだアップロードされていないときの応答の内容を示しています。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e72b8-p110">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="e72b8-179">要求した写真のバイナリ データを使用する</span><span class="sxs-lookup"><span data-stu-id="e72b8-179">Using the binary data of the requested photo</span></span>

<span data-ttu-id="e72b8-180">`/photo/$value` エンドポイントを使用してプロフィール写真のバイナリ データを取得するときに、そのデータを電子メールの添付ファイルとして追加するには、ベース 64 の文字列に変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e72b8-180">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="e72b8-181">JavaScript で [Outlook メッセージ](user_post_messages.md)の `Attachments` パラメーターの値として渡すことができる配列を作成する方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e72b8-181">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user_post_messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="e72b8-182">この例の実装については、「[Node.js 用の Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e72b8-182">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="e72b8-183">Web ページにイメージを表示する場合は、イメージからメモリ内オブジェクトを作成し、そのオブジェクトをイメージ要素のソースにします。</span><span class="sxs-lookup"><span data-stu-id="e72b8-183">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="e72b8-184">この操作の JavaScript の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e72b8-184">Here is an example in JavaScript of this operation.</span></span>

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
