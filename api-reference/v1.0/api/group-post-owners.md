---
title: グループ所有者の追加
description: グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。
ms.openlocfilehash: 8c879430c78cb1d06150bade842addcb4ba0af38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022110"
---
# <a name="add-group-owner"></a><span data-ttu-id="74273-104">グループ所有者の追加</span><span class="sxs-lookup"><span data-stu-id="74273-104">Add group owner</span></span>
<span data-ttu-id="74273-p102">グループ所有者にユーザーを追加します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="74273-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="74273-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74273-107">Permissions</span></span>
<span data-ttu-id="74273-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74273-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74273-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74273-110">Permission type</span></span>      | <span data-ttu-id="74273-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74273-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74273-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74273-112">Delegated (work or school account)</span></span> | <span data-ttu-id="74273-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74273-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="74273-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74273-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74273-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74273-115">Not supported.</span></span>    |
|<span data-ttu-id="74273-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74273-116">Application</span></span> | <span data-ttu-id="74273-117">Group.ReadWrite.All と User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74273-117">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74273-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74273-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="74273-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74273-119">Request headers</span></span>
| <span data-ttu-id="74273-120">名前</span><span class="sxs-lookup"><span data-stu-id="74273-120">Name</span></span>       | <span data-ttu-id="74273-121">型</span><span class="sxs-lookup"><span data-stu-id="74273-121">Type</span></span> | <span data-ttu-id="74273-122">説明</span><span class="sxs-lookup"><span data-stu-id="74273-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="74273-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74273-123">Authorization</span></span>  | <span data-ttu-id="74273-124">string</span><span class="sxs-lookup"><span data-stu-id="74273-124">string</span></span>  | <span data-ttu-id="74273-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="74273-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74273-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="74273-127">Request body</span></span>
<span data-ttu-id="74273-128">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="74273-128">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="74273-129">応答</span><span class="sxs-lookup"><span data-stu-id="74273-129">Response</span></span>
<span data-ttu-id="74273-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="74273-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74273-132">例</span><span class="sxs-lookup"><span data-stu-id="74273-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="74273-133">要求</span><span class="sxs-lookup"><span data-stu-id="74273-133">Request</span></span>
<span data-ttu-id="74273-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74273-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="74273-135">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="74273-135">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="74273-136">応答</span><span class="sxs-lookup"><span data-stu-id="74273-136">Response</span></span>
<span data-ttu-id="74273-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74273-137">The following is an example of the response.</span></span>
><span data-ttu-id="74273-138">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="74273-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="74273-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="74273-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
