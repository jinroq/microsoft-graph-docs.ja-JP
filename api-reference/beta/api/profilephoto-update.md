---
title: ProfilePhoto を更新する
description: サインイン ユーザー、または指定されたグループあるいは連絡先を含むテナント内の任意のユーザーの写真を更新します。 そこから
localization_priority: Normal
ms.openlocfilehash: 8a3c6d2ce042fa068fb0e0d99798fd8fa2be1d07
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621342"
---
# <a name="update-profilephoto"></a><span data-ttu-id="91925-104">profilephoto を更新する</span><span class="sxs-lookup"><span data-stu-id="91925-104">Update profilephoto</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91925-p102">サインイン ユーザー、または指定されたグループあるいは連絡先を含むテナント内の任意のユーザーの写真を更新します。現在各 REST 要求の合計サイズは 4 MB に制限されているため、追加する写真のサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="91925-p102">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="91925-107">ベータ版では、この操作に PUT のみを使用します。</span><span class="sxs-lookup"><span data-stu-id="91925-107">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="91925-108">**注** ベータ版の写真更新操作では、ユーザーの職場用または学校用メールボックスのみがサポートされ、個人用メールボックスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91925-108">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="91925-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91925-109">Permissions</span></span>
<span data-ttu-id="91925-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91925-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91925-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91925-112">Permission type</span></span>      | <span data-ttu-id="91925-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="91925-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91925-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91925-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="91925-115">サインインしている**ユーザー**のプロファイル写真:</span><span class="sxs-lookup"><span data-stu-id="91925-115">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="91925-116">ユーザー読み取り/書き込みユーザー。</span><span class="sxs-lookup"><span data-stu-id="91925-116">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="91925-117">**group** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="91925-117">For **group** resource:</span></span><br /><span data-ttu-id="91925-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91925-118">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="91925-119">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="91925-119">For **contact** resource:</span></span><br /><span data-ttu-id="91925-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91925-120">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="91925-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91925-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91925-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91925-122">Not supported.</span></span> |
|<span data-ttu-id="91925-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91925-123">Application</span></span>                            | <span data-ttu-id="91925-124">**user** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="91925-124">For **user** resource:</span></span><br/><span data-ttu-id="91925-125">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91925-125">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="91925-126">**group** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="91925-126">For **group** resource:</span></span><br /><span data-ttu-id="91925-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91925-127">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="91925-128">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="91925-128">For **contact** resource:</span></span><br /><span data-ttu-id="91925-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91925-129">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="91925-130">**注** 組織内のユーザーの写真を更新するには、アプリにはアプリケーションのアクセス許可 User.ReadWrite.All が必要で、ユーザーの代わりではなく、それ自身の ID でこの API を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="91925-130">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="91925-131">詳細については、「[ユーザーなしでアクセスを取得する](/graph/auth-v2-service)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91925-131">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

> <span data-ttu-id="91925-132">**注:** アプリケーションのアクセス許可を使用してグループ写真にアクセスする際に、[既知の問題](https://docs.microsoft.com/en-us/graph/known-issues#groups)が現在発生しています。</span><span class="sxs-lookup"><span data-stu-id="91925-132">**Note:**  There is currently a [known issue](https://docs.microsoft.com/en-us/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="91925-133">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91925-133">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a><span data-ttu-id="91925-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91925-134">Request headers</span></span>
| <span data-ttu-id="91925-135">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91925-135">Header</span></span>       | <span data-ttu-id="91925-136">値</span><span class="sxs-lookup"><span data-stu-id="91925-136">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91925-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="91925-137">Authorization</span></span>  | <span data-ttu-id="91925-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="91925-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="91925-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91925-140">Content-Type</span></span>  | <span data-ttu-id="91925-p106">image/jpeg。必須。</span><span class="sxs-lookup"><span data-stu-id="91925-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91925-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="91925-143">Request body</span></span>
<span data-ttu-id="91925-144">要求本文に、写真のバイナリ データを含めます。</span><span class="sxs-lookup"><span data-stu-id="91925-144">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="91925-145">応答</span><span class="sxs-lookup"><span data-stu-id="91925-145">Response</span></span>

<span data-ttu-id="91925-146">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="91925-146">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="91925-147">例</span><span class="sxs-lookup"><span data-stu-id="91925-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91925-148">要求</span><span class="sxs-lookup"><span data-stu-id="91925-148">Request</span></span>
<span data-ttu-id="91925-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="91925-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="91925-150">プロトコル</span><span class="sxs-lookup"><span data-stu-id="91925-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="91925-151">C#</span><span class="sxs-lookup"><span data-stu-id="91925-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91925-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="91925-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91925-153">応答</span><span class="sxs-lookup"><span data-stu-id="91925-153">Response</span></span>
<span data-ttu-id="91925-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="91925-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
