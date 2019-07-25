---
title: リストのオーバーライド
description: ユーザーが設定したオーバーライドを取得して、特定の送信者からのメッセージを常に一定の方法で分類します。
localization_priority: Normal
ms.openlocfilehash: 8bbe0eb84f03e4a6c11114c9eca78640e4f0036f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880872"
---
# <a name="list-overrides"></a><span data-ttu-id="8c087-103">リストのオーバーライド</span><span class="sxs-lookup"><span data-stu-id="8c087-103">List overrides</span></span>

<span data-ttu-id="8c087-104">ユーザーが設定したオーバーライドを取得して、特定の送信者からのメッセージを常に一定の方法で分類します。</span><span class="sxs-lookup"><span data-stu-id="8c087-104">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="8c087-p101">それぞれのオーバーライドは、送信者の SMTP アドレスに対応します。 最初は、ユーザーにはオーバーライドはありません。</span><span class="sxs-lookup"><span data-stu-id="8c087-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c087-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c087-107">Permissions</span></span>
<span data-ttu-id="8c087-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c087-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c087-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c087-110">Permission type</span></span>      | <span data-ttu-id="8c087-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c087-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c087-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c087-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c087-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8c087-113">Mail.Read</span></span>    |
|<span data-ttu-id="8c087-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c087-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c087-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8c087-115">Mail.Read</span></span>    |
|<span data-ttu-id="8c087-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c087-116">Application</span></span> | <span data-ttu-id="8c087-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8c087-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c087-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c087-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="8c087-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c087-119">Request headers</span></span>
| <span data-ttu-id="8c087-120">名前</span><span class="sxs-lookup"><span data-stu-id="8c087-120">Name</span></span>       | <span data-ttu-id="8c087-121">型</span><span class="sxs-lookup"><span data-stu-id="8c087-121">Type</span></span> | <span data-ttu-id="8c087-122">説明</span><span class="sxs-lookup"><span data-stu-id="8c087-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c087-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c087-123">Authorization</span></span>  | <span data-ttu-id="8c087-124">string</span><span class="sxs-lookup"><span data-stu-id="8c087-124">string</span></span>  | <span data-ttu-id="8c087-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c087-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c087-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c087-127">Request body</span></span>
<span data-ttu-id="8c087-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8c087-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c087-129">応答</span><span class="sxs-lookup"><span data-stu-id="8c087-129">Response</span></span>

<span data-ttu-id="8c087-p104">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) オブジェクトのコレクションを返します。ユーザーがオーバーライドを設定していない場合は、空のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="8c087-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="8c087-132">例</span><span class="sxs-lookup"><span data-stu-id="8c087-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c087-133">要求</span><span class="sxs-lookup"><span data-stu-id="8c087-133">Request</span></span>
<span data-ttu-id="8c087-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c087-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8c087-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8c087-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c087-136">C#</span><span class="sxs-lookup"><span data-stu-id="8c087-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-overrides-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c087-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="8c087-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-overrides-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c087-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="8c087-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-overrides-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8c087-139">Java</span><span class="sxs-lookup"><span data-stu-id="8c087-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-overrides-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8c087-140">応答</span><span class="sxs-lookup"><span data-stu-id="8c087-140">Response</span></span>
<span data-ttu-id="8c087-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c087-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
