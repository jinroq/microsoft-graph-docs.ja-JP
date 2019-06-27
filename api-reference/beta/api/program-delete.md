---
title: プログラムの削除
description: Azure AD access レビュー機能で、プログラムオブジェクトを削除します。
localization_priority: Normal
ms.openlocfilehash: 6ae6757c46efd137fe7f433d690e9f7444531eac
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268076"
---
# <a name="delete-program"></a><span data-ttu-id="65778-103">プログラムの削除</span><span class="sxs-lookup"><span data-stu-id="65778-103">Delete program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65778-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、[プログラム](../resources/program.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="65778-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="65778-105">まだ`programControl`リンクされているプログラムを削除しないでください。これらのアクセスレビューは、最初にプログラムから削除するか、別のプログラムにリンクする必要があります。</span><span class="sxs-lookup"><span data-stu-id="65778-105">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="65778-106">また、組み込みの既定のプログラムは削除できないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="65778-106">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="65778-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65778-107">Permissions</span></span>
<span data-ttu-id="65778-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65778-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65778-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65778-110">Permission type</span></span>                        | <span data-ttu-id="65778-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65778-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="65778-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65778-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="65778-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65778-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="65778-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65778-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65778-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65778-115">Not supported.</span></span> |
|<span data-ttu-id="65778-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65778-116">Application</span></span>                            | <span data-ttu-id="65778-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65778-117">Not supported.</span></span> |

<span data-ttu-id="65778-118">サインインしているユーザーは、プログラムを作成することを許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="65778-118">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="65778-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65778-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="65778-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65778-120">Request headers</span></span>
| <span data-ttu-id="65778-121">名前</span><span class="sxs-lookup"><span data-stu-id="65778-121">Name</span></span>         | <span data-ttu-id="65778-122">型</span><span class="sxs-lookup"><span data-stu-id="65778-122">Type</span></span>        | <span data-ttu-id="65778-123">説明</span><span class="sxs-lookup"><span data-stu-id="65778-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="65778-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="65778-124">Authorization</span></span> | <span data-ttu-id="65778-125">string</span><span class="sxs-lookup"><span data-stu-id="65778-125">string</span></span> | <span data-ttu-id="65778-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="65778-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65778-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="65778-128">Request body</span></span>
<span data-ttu-id="65778-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="65778-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="65778-130">応答</span><span class="sxs-lookup"><span data-stu-id="65778-130">Response</span></span>
<span data-ttu-id="65778-p104">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="65778-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65778-133">例</span><span class="sxs-lookup"><span data-stu-id="65778-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65778-134">要求</span><span class="sxs-lookup"><span data-stu-id="65778-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
##### <a name="response"></a><span data-ttu-id="65778-135">応答</span><span class="sxs-lookup"><span data-stu-id="65778-135">Response</span></span>
><span data-ttu-id="65778-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="65778-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="65778-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="65778-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="65778-139">C#</span><span class="sxs-lookup"><span data-stu-id="65778-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65778-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="65778-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_program-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="65778-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="65778-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_program-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/program-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
