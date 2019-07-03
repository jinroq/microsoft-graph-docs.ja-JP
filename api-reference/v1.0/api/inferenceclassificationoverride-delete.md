---
title: inferenceClassificationOverride を削除する
description: その ID で指定された上書きを削除します。
localization_priority: Normal
ms.openlocfilehash: 3f1b98e38a431cf98a85c960e439f225c20e348c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444625"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="668d4-103">inferenceClassificationOverride を削除する</span><span class="sxs-lookup"><span data-stu-id="668d4-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="668d4-104">その ID で指定された上書きを削除します。</span><span class="sxs-lookup"><span data-stu-id="668d4-104">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="668d4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="668d4-105">Permissions</span></span>
<span data-ttu-id="668d4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="668d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="668d4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="668d4-108">Permission type</span></span>      | <span data-ttu-id="668d4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="668d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="668d4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="668d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="668d4-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="668d4-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="668d4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="668d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="668d4-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="668d4-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="668d4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="668d4-114">Application</span></span> | <span data-ttu-id="668d4-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="668d4-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="668d4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="668d4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="668d4-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="668d4-117">Request headers</span></span>
| <span data-ttu-id="668d4-118">名前</span><span class="sxs-lookup"><span data-stu-id="668d4-118">Name</span></span>       | <span data-ttu-id="668d4-119">型</span><span class="sxs-lookup"><span data-stu-id="668d4-119">Type</span></span> | <span data-ttu-id="668d4-120">説明</span><span class="sxs-lookup"><span data-stu-id="668d4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="668d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="668d4-121">Authorization</span></span>  | <span data-ttu-id="668d4-122">string</span><span class="sxs-lookup"><span data-stu-id="668d4-122">string</span></span>  | <span data-ttu-id="668d4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="668d4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="668d4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="668d4-125">Request body</span></span>
<span data-ttu-id="668d4-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="668d4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="668d4-127">応答</span><span class="sxs-lookup"><span data-stu-id="668d4-127">Response</span></span>

<span data-ttu-id="668d4-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="668d4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="668d4-130">例</span><span class="sxs-lookup"><span data-stu-id="668d4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="668d4-131">要求</span><span class="sxs-lookup"><span data-stu-id="668d4-131">Request</span></span>
<span data-ttu-id="668d4-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="668d4-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="668d4-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="668d4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="668d4-134">C#</span><span class="sxs-lookup"><span data-stu-id="668d4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="668d4-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="668d4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="668d4-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="668d4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="668d4-137">応答</span><span class="sxs-lookup"><span data-stu-id="668d4-137">Response</span></span>
<span data-ttu-id="668d4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="668d4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
