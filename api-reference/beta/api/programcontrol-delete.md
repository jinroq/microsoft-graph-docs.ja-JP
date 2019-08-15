---
title: ProgramControl の削除
description: Azure AD access レビュー機能で、programControl オブジェクトを削除します。  これにより、プログラムからのアクセスレビューがリンク解除します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: ba76bad184ef4fb4514b529dac4a1c779d29f01b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412468"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="8bdeb-104">ProgramControl の削除</span><span class="sxs-lookup"><span data-stu-id="8bdeb-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bdeb-105">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [programcontrol](../resources/programcontrol.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="8bdeb-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="8bdeb-106">これにより、プログラムからのアクセスレビューがリンク解除します。</span><span class="sxs-lookup"><span data-stu-id="8bdeb-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="8bdeb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8bdeb-107">Permissions</span></span>
<span data-ttu-id="8bdeb-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bdeb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bdeb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8bdeb-110">Permission type</span></span>                        | <span data-ttu-id="8bdeb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8bdeb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bdeb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8bdeb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bdeb-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bdeb-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="8bdeb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8bdeb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bdeb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bdeb-115">Not supported.</span></span> |
|<span data-ttu-id="8bdeb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8bdeb-116">Application</span></span>                            | <span data-ttu-id="8bdeb-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bdeb-117">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="8bdeb-118">サインインしているユーザーは、を`programControl`削除することを許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="8bdeb-118">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="8bdeb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8bdeb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('{id}')
```
## <a name="request-headers"></a><span data-ttu-id="8bdeb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bdeb-120">Request headers</span></span>
| <span data-ttu-id="8bdeb-121">名前</span><span class="sxs-lookup"><span data-stu-id="8bdeb-121">Name</span></span>         | <span data-ttu-id="8bdeb-122">型</span><span class="sxs-lookup"><span data-stu-id="8bdeb-122">Type</span></span>        | <span data-ttu-id="8bdeb-123">説明</span><span class="sxs-lookup"><span data-stu-id="8bdeb-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8bdeb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bdeb-124">Authorization</span></span> | <span data-ttu-id="8bdeb-125">string</span><span class="sxs-lookup"><span data-stu-id="8bdeb-125">string</span></span> | <span data-ttu-id="8bdeb-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="8bdeb-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bdeb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8bdeb-128">Request body</span></span>
<span data-ttu-id="8bdeb-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8bdeb-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8bdeb-130">応答</span><span class="sxs-lookup"><span data-stu-id="8bdeb-130">Response</span></span>
<span data-ttu-id="8bdeb-p105">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8bdeb-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bdeb-133">例</span><span class="sxs-lookup"><span data-stu-id="8bdeb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bdeb-134">要求</span><span class="sxs-lookup"><span data-stu-id="8bdeb-134">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8bdeb-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8bdeb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8bdeb-136">C#</span><span class="sxs-lookup"><span data-stu-id="8bdeb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bdeb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bdeb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8bdeb-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="8bdeb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8bdeb-139">応答</span><span class="sxs-lookup"><span data-stu-id="8bdeb-139">Response</span></span>
><span data-ttu-id="8bdeb-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8bdeb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
