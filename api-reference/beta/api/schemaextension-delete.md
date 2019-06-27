---
title: schemaExtension を削除する
description: スキーマ拡張機能の定義を削除します。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: b8811282c8bf05d845c75fb2709bdfcb00064f3e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264877"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="8ff9f-103">schemaExtension を削除する</span><span class="sxs-lookup"><span data-stu-id="8ff9f-103">Delete schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff9f-104">[スキーマ拡張機能](../resources/schemaextension.md)の定義を削除します。</span><span class="sxs-lookup"><span data-stu-id="8ff9f-104">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="8ff9f-p101">スキーマ拡張機能を作成したアプリ (所有者アプリ) だけが、そのスキーマ拡張機能が **InDevelopment** 状態の場合に限り、スキーマ拡張機能の定義を削除できます。スキーマ拡張機能の定義を削除しても、その定義に基づいてリソース インスタンスに追加されたカスタム データへのアクセスには影響しません。</span><span class="sxs-lookup"><span data-stu-id="8ff9f-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="8ff9f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8ff9f-107">Permissions</span></span>
<span data-ttu-id="8ff9f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ff9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8ff9f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ff9f-110">Permission type</span></span>      | <span data-ttu-id="8ff9f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ff9f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ff9f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ff9f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8ff9f-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ff9f-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ff9f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ff9f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff9f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ff9f-115">Not supported.</span></span>    |
|<span data-ttu-id="8ff9f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ff9f-116">Application</span></span> | <span data-ttu-id="8ff9f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ff9f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ff9f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ff9f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ff9f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ff9f-119">Request headers</span></span>
| <span data-ttu-id="8ff9f-120">名前</span><span class="sxs-lookup"><span data-stu-id="8ff9f-120">Name</span></span>      |<span data-ttu-id="8ff9f-121">説明</span><span class="sxs-lookup"><span data-stu-id="8ff9f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8ff9f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ff9f-122">Authorization</span></span>  | <span data-ttu-id="8ff9f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8ff9f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ff9f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ff9f-125">Request body</span></span>
<span data-ttu-id="8ff9f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8ff9f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ff9f-127">応答</span><span class="sxs-lookup"><span data-stu-id="8ff9f-127">Response</span></span>

<span data-ttu-id="8ff9f-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8ff9f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ff9f-130">例</span><span class="sxs-lookup"><span data-stu-id="8ff9f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ff9f-131">要求</span><span class="sxs-lookup"><span data-stu-id="8ff9f-131">Request</span></span>
<span data-ttu-id="8ff9f-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8ff9f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="8ff9f-133">応答</span><span class="sxs-lookup"><span data-stu-id="8ff9f-133">Response</span></span>
<span data-ttu-id="8ff9f-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8ff9f-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8ff9f-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="8ff9f-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8ff9f-136">C#</span><span class="sxs-lookup"><span data-stu-id="8ff9f-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_schemaextension-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ff9f-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="8ff9f-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_schemaextension-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8ff9f-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="8ff9f-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_schemaextension-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="8ff9f-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="8ff9f-139">See also</span></span>

- [<span data-ttu-id="8ff9f-140">拡張機能を使用したリソースへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="8ff9f-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="8ff9f-141">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="8ff9f-141">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/schemaextension-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schemaextension-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
