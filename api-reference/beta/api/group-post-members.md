---
title: メンバーを追加する
description: この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループにメンバーを追加できます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7bb6e5980ca76d96b544fe07880983de6171e014
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262924"
---
# <a name="add-member"></a><span data-ttu-id="1bad2-103">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="1bad2-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bad2-104">この API を使用して、**members** ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループにメンバーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="1bad2-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="1bad2-105">ユーザーや他のグループを追加できます。</span><span class="sxs-lookup"><span data-stu-id="1bad2-105">You can add users or other groups.</span></span> <span data-ttu-id="1bad2-106">重要: Office 365 のグループには、ユーザーのみを追加できます。</span><span class="sxs-lookup"><span data-stu-id="1bad2-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bad2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1bad2-107">Permissions</span></span>
<span data-ttu-id="1bad2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1bad2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bad2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1bad2-110">Permission type</span></span>      | <span data-ttu-id="1bad2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1bad2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bad2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1bad2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1bad2-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1bad2-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1bad2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1bad2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bad2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1bad2-115">Not supported.</span></span>    |
|<span data-ttu-id="1bad2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1bad2-116">Application</span></span> | <span data-ttu-id="1bad2-117">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bad2-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bad2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1bad2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1bad2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1bad2-119">Request headers</span></span>
| <span data-ttu-id="1bad2-120">名前</span><span class="sxs-lookup"><span data-stu-id="1bad2-120">Name</span></span>       | <span data-ttu-id="1bad2-121">型</span><span class="sxs-lookup"><span data-stu-id="1bad2-121">Type</span></span> | <span data-ttu-id="1bad2-122">説明</span><span class="sxs-lookup"><span data-stu-id="1bad2-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1bad2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bad2-123">Authorization</span></span>  | <span data-ttu-id="1bad2-124">string</span><span class="sxs-lookup"><span data-stu-id="1bad2-124">string</span></span>  | <span data-ttu-id="1bad2-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1bad2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bad2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1bad2-127">Request body</span></span>
<span data-ttu-id="1bad2-128">要求本文で、追加する [directoryObject](../resources/directoryobject.md)、[ユーザー](../resources/user.md) または [グループ](../resources/group.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1bad2-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="1bad2-129">応答</span><span class="sxs-lookup"><span data-stu-id="1bad2-129">Response</span></span>
<span data-ttu-id="1bad2-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1bad2-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bad2-132">例</span><span class="sxs-lookup"><span data-stu-id="1bad2-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1bad2-133">要求</span><span class="sxs-lookup"><span data-stu-id="1bad2-133">Request</span></span>
<span data-ttu-id="1bad2-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1bad2-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
<span data-ttu-id="1bad2-135">要求本文で、追加する[Directoryobject](../resources/directoryobject.md)、 [user](../resources/user.md)、 `id`または[group](../resources/group.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1bad2-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="1bad2-136">応答</span><span class="sxs-lookup"><span data-stu-id="1bad2-136">Response</span></span>
<span data-ttu-id="1bad2-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1bad2-137">The following is an example of the response.</span></span>
><span data-ttu-id="1bad2-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="1bad2-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1bad2-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1bad2-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1bad2-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1bad2-140">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bad2-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="1bad2-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/add_group_member-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1bad2-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="1bad2-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/add_group_member-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
