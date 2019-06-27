---
title: inferenceClassificationOverride を削除する
description: その ID で指定された上書きを削除します。
localization_priority: Normal
ms.openlocfilehash: ae4043f0f118519de860c12431f0c6a80289a08f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277113"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="74a29-103">inferenceClassificationOverride を削除する</span><span class="sxs-lookup"><span data-stu-id="74a29-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="74a29-104">その ID で指定された上書きを削除します。</span><span class="sxs-lookup"><span data-stu-id="74a29-104">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="74a29-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74a29-105">Permissions</span></span>
<span data-ttu-id="74a29-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74a29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74a29-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74a29-108">Permission type</span></span>      | <span data-ttu-id="74a29-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74a29-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74a29-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74a29-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74a29-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74a29-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="74a29-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74a29-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74a29-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74a29-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="74a29-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74a29-114">Application</span></span> | <span data-ttu-id="74a29-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74a29-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="74a29-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74a29-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="74a29-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74a29-117">Request headers</span></span>
| <span data-ttu-id="74a29-118">名前</span><span class="sxs-lookup"><span data-stu-id="74a29-118">Name</span></span>       | <span data-ttu-id="74a29-119">型</span><span class="sxs-lookup"><span data-stu-id="74a29-119">Type</span></span> | <span data-ttu-id="74a29-120">説明</span><span class="sxs-lookup"><span data-stu-id="74a29-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="74a29-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="74a29-121">Authorization</span></span>  | <span data-ttu-id="74a29-122">string</span><span class="sxs-lookup"><span data-stu-id="74a29-122">string</span></span>  | <span data-ttu-id="74a29-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="74a29-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74a29-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="74a29-125">Request body</span></span>
<span data-ttu-id="74a29-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="74a29-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74a29-127">応答</span><span class="sxs-lookup"><span data-stu-id="74a29-127">Response</span></span>

<span data-ttu-id="74a29-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="74a29-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74a29-130">例</span><span class="sxs-lookup"><span data-stu-id="74a29-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74a29-131">要求</span><span class="sxs-lookup"><span data-stu-id="74a29-131">Request</span></span>
<span data-ttu-id="74a29-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74a29-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="74a29-133">応答</span><span class="sxs-lookup"><span data-stu-id="74a29-133">Response</span></span>
<span data-ttu-id="74a29-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74a29-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="74a29-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="74a29-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74a29-138">C#</span><span class="sxs-lookup"><span data-stu-id="74a29-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74a29-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="74a29-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="74a29-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="74a29-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
