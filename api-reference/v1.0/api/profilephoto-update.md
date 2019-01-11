---
title: ProfilePhoto を更新する
description: サインインしている**ユーザー**、指定された**グループ**または**連絡先**の写真を更新します。 そこから
localization_priority: Priority
ms.openlocfilehash: 39c5a0405a05d46cbd77f161cd45fb19c40d8b7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871821"
---
# <a name="update-profilephoto"></a><span data-ttu-id="af802-104">ProfilePhoto を更新する</span><span class="sxs-lookup"><span data-stu-id="af802-104">Update profilephoto</span></span>

<span data-ttu-id="af802-p102">サインイン **ユーザー**、または指定された**グループ**または**連絡先**の写真を更新します。現在各 REST 要求の合計サイズは 4 MB に制限されているため、追加する写真のサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="af802-p102">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="af802-107">バージョン 1.0 では、この操作に PATCH と PUT のいずれかを使用できます。</span><span class="sxs-lookup"><span data-stu-id="af802-107">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="af802-108">**注** バージョン 1.0 のこの操作では、ユーザーの職場用または学校用メールボックスのみがサポートされ、個人用メールボックスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af802-108">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="af802-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="af802-109">Permissions</span></span>
<span data-ttu-id="af802-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af802-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

- <span data-ttu-id="af802-112">サインインしている**ユーザー**のプロファイル写真 - User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af802-112">Profile photo of the signed-in **user** - User.ReadWrite, User.ReadWrite.All</span></span>
- <span data-ttu-id="af802-113">**グループ**のプロファイル写真 - Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af802-113">Profile photo of a **group** - Group.ReadWrite.All</span></span>
- <span data-ttu-id="af802-114">**連絡先**の写真 - Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af802-114">Photo of a **contact** - Contacts.ReadWrite</span></span>

> <span data-ttu-id="af802-p104">**注** 組織内のユーザーの写真を更新するには、アプリにはアプリケーションのアクセス許可 User.ReadWrite.All が必要で、ユーザーの代わりではなく、それ自身の ID でこの API を呼び出す必要があります。詳細については、「[ユーザーなしでアクセスを取得する](/graph/auth-v2-service)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af802-p104">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="af802-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af802-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a><span data-ttu-id="af802-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af802-118">Request headers</span></span>
| <span data-ttu-id="af802-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af802-119">Header</span></span>       | <span data-ttu-id="af802-120">値</span><span class="sxs-lookup"><span data-stu-id="af802-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="af802-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="af802-121">Authorization</span></span>  | <span data-ttu-id="af802-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="af802-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="af802-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af802-124">Content-Type</span></span>  | <span data-ttu-id="af802-p106">image/jpeg。必須。</span><span class="sxs-lookup"><span data-stu-id="af802-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af802-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="af802-127">Request body</span></span>
<span data-ttu-id="af802-128">要求本文に、写真のバイナリ データを含めます。</span><span class="sxs-lookup"><span data-stu-id="af802-128">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="af802-129">応答</span><span class="sxs-lookup"><span data-stu-id="af802-129">Response</span></span>

<span data-ttu-id="af802-130">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="af802-130">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="af802-131">例</span><span class="sxs-lookup"><span data-stu-id="af802-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af802-132">要求</span><span class="sxs-lookup"><span data-stu-id="af802-132">Request</span></span>
<span data-ttu-id="af802-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af802-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="af802-134">応答</span><span class="sxs-lookup"><span data-stu-id="af802-134">Response</span></span>
<span data-ttu-id="af802-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="af802-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
