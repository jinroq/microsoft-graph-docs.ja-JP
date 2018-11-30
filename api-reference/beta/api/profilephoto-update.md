---
title: ProfilePhoto を更新する
description: 署名を含むテナント内のユーザーの写真を更新するユーザー、または指定したグループ、または取引先担当者です。 そこから
ms.openlocfilehash: 801ccd58e57cb02c1805f927dc22c9fd593cbae5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071200"
---
# <a name="update-profilephoto"></a><span data-ttu-id="b490d-104">ProfilePhoto を更新する</span><span class="sxs-lookup"><span data-stu-id="b490d-104">Update profilephoto</span></span>

> <span data-ttu-id="b490d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b490d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b490d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b490d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b490d-p103">サインイン ユーザー、または指定されたグループあるいは連絡先を含むテナント内の任意のユーザーの写真を更新します。現在各 REST 要求の合計サイズは 4 MB に制限されているため、追加する写真のサイズは 4 MB 未満に制限されます。</span><span class="sxs-lookup"><span data-stu-id="b490d-p103">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="b490d-109">ベータ版では、この操作に PUT のみを使用します。</span><span class="sxs-lookup"><span data-stu-id="b490d-109">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="b490d-110">**注** ベータ版の写真更新操作では、ユーザーの職場用または学校用メールボックスのみがサポートされ、個人用メールボックスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b490d-110">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="b490d-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b490d-111">Permissions</span></span>
<span data-ttu-id="b490d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b490d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b490d-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b490d-114">Permission type</span></span>      | <span data-ttu-id="b490d-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b490d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b490d-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b490d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b490d-117">サインインしている**ユーザー**のプロフィールの写真。</span><span class="sxs-lookup"><span data-stu-id="b490d-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="b490d-118">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b490d-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="b490d-119">**group** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="b490d-119">For **group** resource:</span></span><br /><span data-ttu-id="b490d-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b490d-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="b490d-121">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="b490d-121">For **contact** resource:</span></span><br /><span data-ttu-id="b490d-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b490d-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="b490d-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b490d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b490d-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b490d-124">Not supported.</span></span> |
|<span data-ttu-id="b490d-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b490d-125">Application</span></span>                            | <span data-ttu-id="b490d-126">**user** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="b490d-126">For **user** resource:</span></span><br/><span data-ttu-id="b490d-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b490d-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="b490d-128">**group** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="b490d-128">For **group** resource:</span></span><br /><span data-ttu-id="b490d-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b490d-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="b490d-130">**contact** リソースの場合:</span><span class="sxs-lookup"><span data-stu-id="b490d-130">For **contact** resource:</span></span><br /><span data-ttu-id="b490d-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b490d-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="b490d-p105">**注** 組織内のユーザーの写真を更新するには、アプリにはアプリケーションのアクセス許可 User.ReadWrite.All が必要で、ユーザーの代わりではなく、それ自身の ID でこの API を呼び出す必要があります。詳細については、「[ユーザーなしでアクセスを取得する](/graph/auth-v2-service)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b490d-p105">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="b490d-134">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b490d-134">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="b490d-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b490d-135">Request headers</span></span>
| <span data-ttu-id="b490d-136">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b490d-136">Header</span></span>       | <span data-ttu-id="b490d-137">値</span><span class="sxs-lookup"><span data-stu-id="b490d-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b490d-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="b490d-138">Authorization</span></span>  | <span data-ttu-id="b490d-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b490d-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b490d-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b490d-141">Content-Type</span></span>  | <span data-ttu-id="b490d-p107">image/jpeg。必須。</span><span class="sxs-lookup"><span data-stu-id="b490d-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b490d-144">要求本文</span><span class="sxs-lookup"><span data-stu-id="b490d-144">Request body</span></span>
<span data-ttu-id="b490d-145">要求本文に、写真のバイナリ データを含めます。</span><span class="sxs-lookup"><span data-stu-id="b490d-145">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="b490d-146">応答</span><span class="sxs-lookup"><span data-stu-id="b490d-146">Response</span></span>

<span data-ttu-id="b490d-147">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b490d-147">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="b490d-148">例</span><span class="sxs-lookup"><span data-stu-id="b490d-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b490d-149">要求</span><span class="sxs-lookup"><span data-stu-id="b490d-149">Request</span></span>
<span data-ttu-id="b490d-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b490d-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="b490d-151">応答</span><span class="sxs-lookup"><span data-stu-id="b490d-151">Response</span></span>
<span data-ttu-id="b490d-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b490d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
