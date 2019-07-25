---
title: 契約を削除する
description: アグリーメントオブジェクトを削除します。
localization_priority: Normal
ms.openlocfilehash: 2b0bf56bf63a62cacd757035f10f0cbb48a30604
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855523"
---
# <a name="delete-agreement"></a><span data-ttu-id="2a536-103">契約を削除する</span><span class="sxs-lookup"><span data-stu-id="2a536-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a536-104">[アグリーメント](../resources/agreement.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2a536-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2a536-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a536-105">Permissions</span></span>
<span data-ttu-id="2a536-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a536-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a536-108">Permission type</span></span>                        | <span data-ttu-id="2a536-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a536-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a536-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a536-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a536-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a536-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="2a536-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a536-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a536-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a536-113">Not supported.</span></span> |
|<span data-ttu-id="2a536-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a536-114">Application</span></span>                            | <span data-ttu-id="2a536-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a536-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a536-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a536-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="2a536-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a536-117">Request headers</span></span>
| <span data-ttu-id="2a536-118">名前</span><span class="sxs-lookup"><span data-stu-id="2a536-118">Name</span></span>         | <span data-ttu-id="2a536-119">型</span><span class="sxs-lookup"><span data-stu-id="2a536-119">Type</span></span>        | <span data-ttu-id="2a536-120">説明</span><span class="sxs-lookup"><span data-stu-id="2a536-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2a536-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a536-121">Authorization</span></span> | <span data-ttu-id="2a536-122">string</span><span class="sxs-lookup"><span data-stu-id="2a536-122">string</span></span> | <span data-ttu-id="2a536-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a536-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a536-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a536-125">Request body</span></span>
<span data-ttu-id="2a536-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2a536-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2a536-127">応答</span><span class="sxs-lookup"><span data-stu-id="2a536-127">Response</span></span>
<span data-ttu-id="2a536-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2a536-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a536-130">例</span><span class="sxs-lookup"><span data-stu-id="2a536-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a536-131">要求</span><span class="sxs-lookup"><span data-stu-id="2a536-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2a536-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2a536-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2a536-133">C#</span><span class="sxs-lookup"><span data-stu-id="2a536-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a536-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="2a536-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2a536-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="2a536-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2a536-136">Java</span><span class="sxs-lookup"><span data-stu-id="2a536-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2a536-137">応答</span><span class="sxs-lookup"><span data-stu-id="2a536-137">Response</span></span>
><span data-ttu-id="2a536-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2a536-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
