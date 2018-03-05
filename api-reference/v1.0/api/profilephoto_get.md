# <a name="get-photo"></a><span data-ttu-id="6da7b-101">写真を取得する</span><span class="sxs-lookup"><span data-stu-id="6da7b-101">Get photo</span></span>

<span data-ttu-id="6da7b-102">指定した [profilePhoto](../resources/profilephoto.md) またはそのメタデータ (profilePhoto プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="6da7b-102">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

<span data-ttu-id="6da7b-103">GET 操作により、Exchange Online のユーザーのメールボックス内で、指定された写真が検索されます。</span><span class="sxs-lookup"><span data-stu-id="6da7b-103">A GET operation looks for the specified photo in the user's mailbox on Exchange Online.</span></span>

> <span data-ttu-id="6da7b-104">**注** バージョン 1.0 のこの操作では、ユーザーの職場用または学校用メールボックスのみがサポートされ、個人用メールボックスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6da7b-104">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="6da7b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6da7b-105">Permissions</span></span>
<span data-ttu-id="6da7b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6da7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

*   <span data-ttu-id="6da7b-108">サインインしているユーザーを含むテナント内の任意のユーザーのプロファイル写真 - User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da7b-108">Profile photo of any user in the tenant including the signed-in user - User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>
*   <span data-ttu-id="6da7b-109">明確にサインインしているユーザーのプロファイル写真 - User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da7b-109">Profile photo of specifically the signed-in user - User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>
* <span data-ttu-id="6da7b-110">**グループ**のプロファイル写真 - Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da7b-110">Profile photo of a **group** - Group.Read.All, Group.ReadWrite.All</span></span>
* <span data-ttu-id="6da7b-111">**連絡先**の写真 - Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6da7b-111">Photo of a **contact** - Contacts.Read, Contacts.ReadWrite</span></span>

## <a name="http-request-to-get-the-photo"></a><span data-ttu-id="6da7b-112">写真を取得する HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6da7b-112">HTTP request to get the photo</span></span>
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
## <a name="http-request-to-get-the-metadata-of-the-photo"></a><span data-ttu-id="6da7b-113">写真のメタデータを取得する HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6da7b-113">HTTP request to get the metadata of the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6da7b-114">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6da7b-114">Optional query parameters</span></span>
<span data-ttu-id="6da7b-115">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6da7b-115">This method supports the [OData Query Parameters](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6da7b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6da7b-116">Request headers</span></span>
| <span data-ttu-id="6da7b-117">名前</span><span class="sxs-lookup"><span data-stu-id="6da7b-117">Name</span></span>       | <span data-ttu-id="6da7b-118">型</span><span class="sxs-lookup"><span data-stu-id="6da7b-118">Type</span></span> | <span data-ttu-id="6da7b-119">説明</span><span class="sxs-lookup"><span data-stu-id="6da7b-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6da7b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6da7b-120">Authorization</span></span>  | <span data-ttu-id="6da7b-121">string</span><span class="sxs-lookup"><span data-stu-id="6da7b-121">string</span></span>  | <span data-ttu-id="6da7b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6da7b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6da7b-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="6da7b-124">Request body</span></span>
<span data-ttu-id="6da7b-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6da7b-125">Do not supply a request body for this method.</span></span>
## <a name="response-for-getting-the-photo"></a><span data-ttu-id="6da7b-126">写真の取得に対する応答</span><span class="sxs-lookup"><span data-stu-id="6da7b-126">Response for getting the photo</span></span>
<span data-ttu-id="6da7b-p103">成功した場合、このメソッドは `200 OK` 応答コードと、要求した写真のバイナリ データを応答本文で返します。写真が存在しない場合、この操作により `404 Not Found` が返されます。</span><span class="sxs-lookup"><span data-stu-id="6da7b-p103">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
## <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="6da7b-129">写真のメタデータの取得に対する応答</span><span class="sxs-lookup"><span data-stu-id="6da7b-129">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="6da7b-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [profilePhoto](../resources/profilePhoto.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6da7b-130">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilePhoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6da7b-131">例</span><span class="sxs-lookup"><span data-stu-id="6da7b-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="6da7b-132">要求 1</span><span class="sxs-lookup"><span data-stu-id="6da7b-132">Request 1</span></span>
<span data-ttu-id="6da7b-133">この要求では、サインインしているユーザーの写真を利用可能な最大のサイズで取得します。</span><span class="sxs-lookup"><span data-stu-id="6da7b-133">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="6da7b-134">応答 1</span><span class="sxs-lookup"><span data-stu-id="6da7b-134">Response 1</span></span>
<span data-ttu-id="6da7b-p104">要求した写真のバイナリ データが含まれています。HTTP 応答コードは 200 です。</span><span class="sxs-lookup"><span data-stu-id="6da7b-p104">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="6da7b-137">要求 2</span><span class="sxs-lookup"><span data-stu-id="6da7b-137">Request 2</span></span>
<span data-ttu-id="6da7b-138">この要求は、サインインしているユーザーのユーザー写真のメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="6da7b-138">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-2"></a><span data-ttu-id="6da7b-139">応答 2</span><span class="sxs-lookup"><span data-stu-id="6da7b-139">Response 2</span></span>

<span data-ttu-id="6da7b-p105">次の応答データは、写真のメタデータを示しています。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6da7b-p105">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
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

<span data-ttu-id="6da7b-p106">次の応答データは、そのユーザーの写真がまだアップロードされていないときの応答の内容を示しています。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6da7b-p106">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="6da7b-144">要求した写真のバイナリ データを使用する</span><span class="sxs-lookup"><span data-stu-id="6da7b-144">Contains the binary data of the requested photo.</span></span>

<span data-ttu-id="6da7b-145">`/photo/$value` エンドポイントを使用してプロフィール写真のバイナリ データを取得するときに、そのデータを電子メールの添付ファイルとして追加するには、ベース 64 の文字列に変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6da7b-145">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="6da7b-146">JavaScript で [Outlook メッセージ](user_post_messages.md)の `Attachments` パラメーターの値として渡すことができる配列を作成する方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6da7b-146">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user_post_messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="6da7b-147">この例の実装については、「[Node.js 用の Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6da7b-147">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="6da7b-148">Web ページにイメージを表示する場合は、イメージからメモリ内オブジェクトを作成し、そのオブジェクトをイメージ要素のソースにします。</span><span class="sxs-lookup"><span data-stu-id="6da7b-148">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="6da7b-149">この操作の JavaScript の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6da7b-149">Here is an example in JavaScript of this operation.</span></span>

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
