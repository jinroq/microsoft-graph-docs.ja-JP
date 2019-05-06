---
title: 写真を取得する
description: 指定した profilePhoto またはそのメタデータ (profilePhoto プロパティ) を取得します。
localization_priority: Priority
ms.openlocfilehash: e0b115ecf3ce05d87856e553b111af537ffad0e3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576284"
---
# <a name="get-photo"></a><span data-ttu-id="c6166-103">写真を取得する</span><span class="sxs-lookup"><span data-stu-id="c6166-103">Get photo</span></span>

<span data-ttu-id="c6166-104">指定した [profilePhoto](../resources/profilephoto.md) またはそのメタデータ (profilePhoto プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="c6166-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="c6166-105">**注**: バージョン 1.0 のこの操作では、ユーザーの職場用または学校用メールボックスのみがサポートされ、個人用メールボックスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6166-105">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="c6166-106">Office 365 上でサポートされている HD Photo のサイズは次のとおりです: 48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504、648x648。</span><span class="sxs-lookup"><span data-stu-id="c6166-106">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="c6166-107">写真が Azure Active Directory に格納されている場合は、サイズに関する制限はありません。</span><span class="sxs-lookup"><span data-stu-id="c6166-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="c6166-108">使用可能な最大の写真のメタデータを取得したり、サイズを指定してその写真サイズのメタデータを取得したりできます。</span><span class="sxs-lookup"><span data-stu-id="c6166-108">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="c6166-109">要求したサイズが使用できない場合でも、アップロードされて使用可能になっている、より小さいサイズを取得できます。</span><span class="sxs-lookup"><span data-stu-id="c6166-109">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="c6166-110">たとえば、アップロードした写真が 504x504 ピクセルの場合は、648×648 を除くすべてのサイズの写真がダウンロード可能になります。</span><span class="sxs-lookup"><span data-stu-id="c6166-110">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6166-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c6166-111">Permissions</span></span>

<span data-ttu-id="c6166-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6166-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6166-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c6166-114">Permission type</span></span>      | <span data-ttu-id="c6166-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c6166-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6166-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c6166-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c6166-117">**user** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="c6166-117">For **user** resource:</span></span><br/><span data-ttu-id="c6166-118">User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6166-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c6166-119">**group** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="c6166-119">For **group** resource:</span></span><br /><span data-ttu-id="c6166-120">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6166-120">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c6166-121">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="c6166-121">For **contact** resource:</span></span><br /><span data-ttu-id="c6166-122">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6166-122">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="c6166-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c6166-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6166-124">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="c6166-124">Not supported</span></span> |
|<span data-ttu-id="c6166-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c6166-125">Application</span></span>                        | <span data-ttu-id="c6166-126">**user** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="c6166-126">For **user** resource:</span></span><br/><span data-ttu-id="c6166-127">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6166-127">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c6166-128">**group** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="c6166-128">For **group** resource:</span></span><br /><span data-ttu-id="c6166-129">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6166-129">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c6166-130">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="c6166-130">For **contact** resource:</span></span><br /><span data-ttu-id="c6166-131">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6166-131">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="c6166-132">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c6166-132">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="c6166-133">写真を取得する</span><span class="sxs-lookup"><span data-stu-id="c6166-133">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="c6166-134">写真のメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="c6166-134">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="c6166-135">特定の写真サイズのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="c6166-135">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="c6166-136">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="c6166-136">Path parameters</span></span>

|<span data-ttu-id="c6166-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c6166-137">Parameter</span></span>|<span data-ttu-id="c6166-138">型</span><span class="sxs-lookup"><span data-stu-id="c6166-138">Type</span></span>|<span data-ttu-id="c6166-139">説明</span><span class="sxs-lookup"><span data-stu-id="c6166-139">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c6166-140">サイズ</span><span class="sxs-lookup"><span data-stu-id="c6166-140">size</span></span>  |<span data-ttu-id="c6166-141">String</span><span class="sxs-lookup"><span data-stu-id="c6166-141">String</span></span>  | <span data-ttu-id="c6166-142">写真のサイズ。</span><span class="sxs-lookup"><span data-stu-id="c6166-142">A photo size.</span></span> <span data-ttu-id="c6166-143">Office 365 上でサポートされている HD Photo のサイズは次のとおりです: 48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504、648x648。</span><span class="sxs-lookup"><span data-stu-id="c6166-143">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="c6166-144">写真が Azure Active Directory に格納されている場合は、サイズに関する制限はありません。</span><span class="sxs-lookup"><span data-stu-id="c6166-144">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="c6166-145">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c6166-145">Optional query parameters</span></span>
<span data-ttu-id="c6166-146">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c6166-146">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6166-147">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6166-147">Request headers</span></span>
| <span data-ttu-id="c6166-148">名前</span><span class="sxs-lookup"><span data-stu-id="c6166-148">Name</span></span>       | <span data-ttu-id="c6166-149">型</span><span class="sxs-lookup"><span data-stu-id="c6166-149">Type</span></span> | <span data-ttu-id="c6166-150">説明</span><span class="sxs-lookup"><span data-stu-id="c6166-150">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c6166-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6166-151">Authorization</span></span>  | <span data-ttu-id="c6166-152">string</span><span class="sxs-lookup"><span data-stu-id="c6166-152">string</span></span>  | <span data-ttu-id="c6166-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c6166-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6166-155">要求本文</span><span class="sxs-lookup"><span data-stu-id="c6166-155">Request body</span></span>
<span data-ttu-id="c6166-156">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c6166-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6166-157">応答</span><span class="sxs-lookup"><span data-stu-id="c6166-157">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="c6166-158">写真の取得に対する応答</span><span class="sxs-lookup"><span data-stu-id="c6166-158">Response for getting the photo</span></span>
<span data-ttu-id="c6166-p106">成功した場合、このメソッドは `200 OK` 応答コードと、要求した写真のバイナリ データを応答本文で返します。写真が存在しない場合、この操作により `404 Not Found` が返されます。</span><span class="sxs-lookup"><span data-stu-id="c6166-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="c6166-161">写真のメタデータの取得に対する応答</span><span class="sxs-lookup"><span data-stu-id="c6166-161">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="c6166-162">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [profilePhoto](../resources/profilephoto.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c6166-162">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="c6166-163">例</span><span class="sxs-lookup"><span data-stu-id="c6166-163">Examples</span></span>

### <a name="example-1-get-the-photo-for-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="c6166-164">例 1: サインインしているユーザーの写真を利用可能な最大のサイズで取得します。</span><span class="sxs-lookup"><span data-stu-id="c6166-164">Example 1: Get the photo of the signed-in user in the largest available size</span></span>
##### <a name="request"></a><span data-ttu-id="c6166-165">要求</span><span class="sxs-lookup"><span data-stu-id="c6166-165">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response"></a><span data-ttu-id="c6166-166">応答</span><span class="sxs-lookup"><span data-stu-id="c6166-166">Response</span></span> 
<span data-ttu-id="c6166-167">要求した写真のバイナリ データが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c6166-167">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="c6166-168">HTTP 応答コードは 200 です。</span><span class="sxs-lookup"><span data-stu-id="c6166-168">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-use"></a><span data-ttu-id="c6166-169">例 2: サインインしているユーザーの 48x48 の写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="c6166-169">Example 2: Get the 48x48 photo for the signed-in user</span></span>
##### <a name="request"></a><span data-ttu-id="c6166-170">要求</span><span class="sxs-lookup"><span data-stu-id="c6166-170">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="c6166-171">応答</span><span class="sxs-lookup"><span data-stu-id="c6166-171">Response</span></span>
<span data-ttu-id="c6166-172">要求した 48x48 の写真のバイナリ データが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c6166-172">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="c6166-173">HTTP 応答コードは 200 です。</span><span class="sxs-lookup"><span data-stu-id="c6166-173">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="c6166-174">例 3: サインインしているユーザーのユーザー写真のメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="c6166-174">Example 3: Get the metadata of the user photo of the signed-in user</span></span>
##### <a name="request"></a><span data-ttu-id="c6166-175">要求</span><span class="sxs-lookup"><span data-stu-id="c6166-175">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response"></a><span data-ttu-id="c6166-176">応答</span><span class="sxs-lookup"><span data-stu-id="c6166-176">Response</span></span>

<span data-ttu-id="c6166-177">次の応答データは、写真のメタデータを示しています。</span><span class="sxs-lookup"><span data-stu-id="c6166-177">The following response data shows the photo metadata.</span></span> 

><span data-ttu-id="c6166-178">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c6166-178">**Note:** The response object shown here might be shortened for readability.</span></span>
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

<span data-ttu-id="c6166-179">次の応答データは、そのユーザーの写真がまだアップロードされていないときの応答の内容を示しています。</span><span class="sxs-lookup"><span data-stu-id="c6166-179">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span>

><span data-ttu-id="c6166-180">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c6166-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="c6166-181">要求した写真のバイナリ データを使用する</span><span class="sxs-lookup"><span data-stu-id="c6166-181">Using the binary data of the requested photo</span></span>

<span data-ttu-id="c6166-182">`/photo/$value` エンドポイントを使用してプロフィール写真のバイナリ データを取得するときに、そのデータを電子メールの添付ファイルとして追加するには、ベース 64 の文字列に変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c6166-182">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="c6166-183">JavaScript で [Outlook メッセージ](user-post-messages.md)の `Attachments` パラメーターの値として渡すことができる配列を作成する方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c6166-183">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="c6166-184">この例の実装については、「[Node.js 用の Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6166-184">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="c6166-185">Web ページにイメージを表示する場合は、イメージからメモリ内オブジェクトを作成し、そのオブジェクトをイメージ要素のソースにします。</span><span class="sxs-lookup"><span data-stu-id="c6166-185">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="c6166-186">この操作の JavaScript の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c6166-186">Here is an example in JavaScript of this operation.</span></span>

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
