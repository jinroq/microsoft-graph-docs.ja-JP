---
title: 写真を取得する
description: 指定した profilePhoto またはそのメタデータ (**profilePhoto** プロパティ) を取得します。
localization_priority: Priority
ms.openlocfilehash: 422b9cb39b7af6527341070cbe35f3bfb59d504d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337174"
---
# <a name="get-photo"></a><span data-ttu-id="6c444-103">写真を取得する</span><span class="sxs-lookup"><span data-stu-id="6c444-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c444-104">指定した [profilePhoto](../resources/profilephoto.md) またはそのメタデータ (**profilePhoto** プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="6c444-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="6c444-105">写真取得メソッドでは、まず Office 365 から指定した写真の取得を試行します。</span><span class="sxs-lookup"><span data-stu-id="6c444-105">A GET photo method first attempts to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="6c444-106">Office 365 に利用できる写真がない場合は、API により Azure Active Directory から写真の取得を試行します。</span><span class="sxs-lookup"><span data-stu-id="6c444-106">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="6c444-107">Office 365 上でサポートされている HD Photo のサイズは次のとおりです: 48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504、648x648。</span><span class="sxs-lookup"><span data-stu-id="6c444-107">The supported sizes of HD photos in Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="6c444-108">写真が Azure Active Directory に格納されている場合は、サイズに関する制限はありません。</span><span class="sxs-lookup"><span data-stu-id="6c444-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="6c444-109">使用可能な最大の写真のメタデータを取得したり、サイズを指定してその写真サイズのメタデータを取得したりできます。</span><span class="sxs-lookup"><span data-stu-id="6c444-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="6c444-110">要求したサイズが使用できない場合でも、アップロードされて使用可能になっている、より小さいサイズを取得できます。</span><span class="sxs-lookup"><span data-stu-id="6c444-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="6c444-111">たとえば、アップロードした写真が 504x504 ピクセルの場合は、648×648 を除くすべてのサイズの写真がダウンロード可能になります。</span><span class="sxs-lookup"><span data-stu-id="6c444-111">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span>
<span data-ttu-id="6c444-112">指定したサイズがユーザーのメールボックスにも Azure Active Directory にもない場合は、1x1 のサイズがメタデータの残りの部分とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="6c444-112">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size 1x1 is returned with the rest of the  metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c444-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c444-113">Permissions</span></span>
<span data-ttu-id="6c444-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c444-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="6c444-116">**注:** ベータ版の写真取得メソッドでは、ユーザーの職場用、学校用、個人用アカウントがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="6c444-116">**Note:** The GET photo method in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="6c444-117">ただし、写真メタデータ取得メソッドでは、ユーザーの職場用または学校用アカウントのみがサポートされ、個人用アカウントはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c444-117">The GET photo metadata method, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="6c444-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c444-118">Permission type</span></span>      | <span data-ttu-id="6c444-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c444-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c444-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c444-120">Delegated (work or school account)</span></span> | <span data-ttu-id="6c444-121">**user** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="6c444-121">For **user** resource:</span></span><br/><span data-ttu-id="6c444-122">User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c444-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="6c444-123">**group** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="6c444-123">For **group** resource:</span></span><br /><span data-ttu-id="6c444-124">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c444-124">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="6c444-125">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="6c444-125">For **contact** resource:</span></span><br /><span data-ttu-id="6c444-126">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c444-126">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="6c444-127">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c444-127">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="6c444-128">**注:** メタデータ操作はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c444-128">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="6c444-129">**user** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="6c444-129">For **user** resource:</span></span><br/><span data-ttu-id="6c444-130">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c444-130">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="6c444-131">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="6c444-131">For **contact** resource:</span></span><br /><span data-ttu-id="6c444-132">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c444-132">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="6c444-133">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c444-133">Application</span></span>                        | <span data-ttu-id="6c444-134">**user** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="6c444-134">For **user** resource:</span></span><br/><span data-ttu-id="6c444-135">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c444-135">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="6c444-136">**group** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="6c444-136">For **group** resource:</span></span><br /><span data-ttu-id="6c444-137">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c444-137">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="6c444-138">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="6c444-138">For **contact** resource:</span></span><br /><span data-ttu-id="6c444-139">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c444-139">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c444-140">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c444-140">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="6c444-141">写真を取得する</span><span class="sxs-lookup"><span data-stu-id="6c444-141">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="6c444-142">写真のメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="6c444-142">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="6c444-143">特定の写真サイズのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="6c444-143">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="6c444-144">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="6c444-144">Path parameters</span></span>

|<span data-ttu-id="6c444-145">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="6c444-145">**Parameter**</span></span>|<span data-ttu-id="6c444-146">**型**</span><span class="sxs-lookup"><span data-stu-id="6c444-146">**Type**</span></span>|<span data-ttu-id="6c444-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c444-147">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6c444-148">size</span><span class="sxs-lookup"><span data-stu-id="6c444-148">size</span></span>  |<span data-ttu-id="6c444-149">String</span><span class="sxs-lookup"><span data-stu-id="6c444-149">String</span></span>  | <span data-ttu-id="6c444-150">写真のサイズ。</span><span class="sxs-lookup"><span data-stu-id="6c444-150">A photo size.</span></span> <span data-ttu-id="6c444-151">Office 365 上でサポートされている HD Photo のサイズは次のとおりです: 48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504、648x648。</span><span class="sxs-lookup"><span data-stu-id="6c444-151">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="6c444-152">写真が Azure Active Directory に格納されている場合は、サイズに関する制限はありません。</span><span class="sxs-lookup"><span data-stu-id="6c444-152">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="6c444-153">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6c444-153">Optional query parameters</span></span>
<span data-ttu-id="6c444-154">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6c444-154">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c444-155">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c444-155">Request headers</span></span>
| <span data-ttu-id="6c444-156">名前</span><span class="sxs-lookup"><span data-stu-id="6c444-156">Name</span></span>       | <span data-ttu-id="6c444-157">型</span><span class="sxs-lookup"><span data-stu-id="6c444-157">Type</span></span> | <span data-ttu-id="6c444-158">説明</span><span class="sxs-lookup"><span data-stu-id="6c444-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6c444-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c444-159">Authorization</span></span>  | <span data-ttu-id="6c444-160">string</span><span class="sxs-lookup"><span data-stu-id="6c444-160">string</span></span>  | <span data-ttu-id="6c444-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6c444-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c444-163">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c444-163">Request body</span></span>
<span data-ttu-id="6c444-164">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6c444-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c444-165">応答</span><span class="sxs-lookup"><span data-stu-id="6c444-165">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="6c444-166">写真の取得に対する応答</span><span class="sxs-lookup"><span data-stu-id="6c444-166">Response for getting the photo</span></span>
<span data-ttu-id="6c444-p108">成功した場合、このメソッドは `200 OK` 応答コードと、要求した写真のバイナリ データを応答本文で返します。写真が存在しない場合、この操作により `404 Not Found` が返されます。</span><span class="sxs-lookup"><span data-stu-id="6c444-p108">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="6c444-169">写真のメタデータの取得に対する応答</span><span class="sxs-lookup"><span data-stu-id="6c444-169">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="6c444-170">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [profilePhoto](../resources/profilephoto.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6c444-170">If successful, this method returns a `200 OK` response code and a [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c444-171">例</span><span class="sxs-lookup"><span data-stu-id="6c444-171">Examples</span></span>

### <a name="example-1-get-the-photo-of-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="6c444-172">例 1: サインインしているユーザーの写真を利用可能な最大のサイズで取得します。</span><span class="sxs-lookup"><span data-stu-id="6c444-172">Example 1: Get the photo of the signed-in user in the largest available size</span></span>

##### <a name="request"></a><span data-ttu-id="6c444-173">要求</span><span class="sxs-lookup"><span data-stu-id="6c444-173">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="6c444-174">応答</span><span class="sxs-lookup"><span data-stu-id="6c444-174">Response</span></span>
<span data-ttu-id="6c444-175">要求した写真のバイナリ データが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c444-175">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="6c444-176">HTTP 応答コードは 200 です。</span><span class="sxs-lookup"><span data-stu-id="6c444-176">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-user"></a><span data-ttu-id="6c444-177">例 2: サインインしているユーザーの 48x48 の写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="6c444-177">Example 2: Get the 48x48 photo for the signed-in user</span></span>

##### <a name="request"></a><span data-ttu-id="6c444-178">要求</span><span class="sxs-lookup"><span data-stu-id="6c444-178">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="6c444-179">応答</span><span class="sxs-lookup"><span data-stu-id="6c444-179">Response</span></span>
<span data-ttu-id="6c444-180">要求した 48x48 の写真のバイナリ データが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c444-180">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="6c444-181">HTTP 応答コードは 200 です。</span><span class="sxs-lookup"><span data-stu-id="6c444-181">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="6c444-182">例 3: サインインしているユーザーのユーザー写真のメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="6c444-182">Example 3: Get the metadata of the user photo of the signed-in user</span></span>

##### <a name="request"></a><span data-ttu-id="6c444-183">要求</span><span class="sxs-lookup"><span data-stu-id="6c444-183">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response"></a><span data-ttu-id="6c444-184">応答</span><span class="sxs-lookup"><span data-stu-id="6c444-184">Response</span></span>
<span data-ttu-id="6c444-185">次の応答データは、写真のメタデータを示しています。</span><span class="sxs-lookup"><span data-stu-id="6c444-185">The following response data shows the photo metadata.</span></span> 

><span data-ttu-id="6c444-186">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6c444-186">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="6c444-187">次の応答データは、そのユーザーの写真がまだアップロードされていないときの応答の内容を示しています。</span><span class="sxs-lookup"><span data-stu-id="6c444-187">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span> 

><span data-ttu-id="6c444-188">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6c444-188">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="6c444-189">要求した写真のバイナリ データを使用する</span><span class="sxs-lookup"><span data-stu-id="6c444-189">Using the binary data of the requested photo</span></span>

<span data-ttu-id="6c444-190">`/photo/$value` エンドポイントを使用してプロフィール写真のバイナリ データを取得するときに、そのデータを電子メールの添付ファイルとして追加するには、ベース 64 の文字列に変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c444-190">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="6c444-191">次の JavaScript の例は、[Outlook メッセージ](user-post-messages.md)の `Attachments` パラメーターの値として渡すことができる配列を作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6c444-191">The following JavaScript example shows how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="6c444-192">この例の実装については、「[Node.js 用の Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c444-192">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="6c444-193">Web ページにイメージを表示する場合は、イメージからメモリ内オブジェクトを作成し、そのオブジェクトをイメージ要素のソースにします。</span><span class="sxs-lookup"><span data-stu-id="6c444-193">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="6c444-194">この操作の JavaScript の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6c444-194">Here is an example in JavaScript of this operation.</span></span>

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
