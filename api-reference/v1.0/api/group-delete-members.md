---
title: メンバーを削除する
description: この API を使用して、**メンバー** ナビゲーション プロパティ経由でグループからメンバーを削除します。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 688e93da20d247aee2250f1c21c329703f668522
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448111"
---
# <a name="remove-member"></a><span data-ttu-id="a3c2b-103">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="a3c2b-103">Remove member</span></span>
<span data-ttu-id="a3c2b-104">この API を使用して、**メンバー** ナビゲーション プロパティ経由でグループからメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-104">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3c2b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3c2b-105">Permissions</span></span>
<span data-ttu-id="a3c2b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3c2b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3c2b-108">Permission type</span></span>      | <span data-ttu-id="a3c2b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3c2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3c2b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3c2b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3c2b-111">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3c2b-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a3c2b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3c2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3c2b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-113">Not supported.</span></span> |
|<span data-ttu-id="a3c2b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3c2b-114">Application</span></span> | <span data-ttu-id="a3c2b-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c2b-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3c2b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3c2b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a3c2b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3c2b-117">Request headers</span></span>
| <span data-ttu-id="a3c2b-118">名前</span><span class="sxs-lookup"><span data-stu-id="a3c2b-118">Name</span></span>       | <span data-ttu-id="a3c2b-119">型</span><span class="sxs-lookup"><span data-stu-id="a3c2b-119">Type</span></span> | <span data-ttu-id="a3c2b-120">説明</span><span class="sxs-lookup"><span data-stu-id="a3c2b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3c2b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3c2b-121">Authorization</span></span>  | <span data-ttu-id="a3c2b-122">string</span><span class="sxs-lookup"><span data-stu-id="a3c2b-122">string</span></span>  | <span data-ttu-id="a3c2b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3c2b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3c2b-125">Request body</span></span>
<span data-ttu-id="a3c2b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3c2b-127">応答</span><span class="sxs-lookup"><span data-stu-id="a3c2b-127">Response</span></span>
<span data-ttu-id="a3c2b-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3c2b-130">例</span><span class="sxs-lookup"><span data-stu-id="a3c2b-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a3c2b-131">要求</span><span class="sxs-lookup"><span data-stu-id="a3c2b-131">Request</span></span>
<span data-ttu-id="a3c2b-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a3c2b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3c2b-133">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3c2b-134">C#</span><span class="sxs-lookup"><span data-stu-id="a3c2b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3c2b-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3c2b-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3c2b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3c2b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a3c2b-137">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-137">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="a3c2b-138">応答</span><span class="sxs-lookup"><span data-stu-id="a3c2b-138">Response</span></span>
<span data-ttu-id="a3c2b-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-139">The following is an example of the response.</span></span>
><span data-ttu-id="a3c2b-140">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a3c2b-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a3c2b-141">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
