---
title: RiskyUser が侵害されたことを確認する
description: RiskyUser オブジェクトが侵害されていることを確認します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: ca2cbaacdc84f7c7aee3f1894beef562dd094ba9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871042"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="70780-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="70780-103">riskyUser: confirmCompromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="70780-104">**注:** RiskyUsers API には、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="70780-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="70780-105">1つまたは複数の[riskyUser](../resources/riskyuser.md)オブジェクトが侵害されたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="70780-105">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="70780-106">このアクションは、対象ユーザーのリスクレベルを [高」に設定します。</span><span class="sxs-lookup"><span data-stu-id="70780-106">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="70780-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="70780-107">Permissions</span></span>
<span data-ttu-id="70780-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70780-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70780-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="70780-110">Permission type</span></span>      | <span data-ttu-id="70780-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="70780-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70780-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="70780-112">Delegated (work or school account)</span></span> | <span data-ttu-id="70780-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="70780-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="70780-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="70780-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70780-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70780-115">Not supported.</span></span>    |
|<span data-ttu-id="70780-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="70780-116">Application</span></span> | <span data-ttu-id="70780-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="70780-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70780-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70780-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="70780-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70780-119">Request headers</span></span>
| <span data-ttu-id="70780-120">名前</span><span class="sxs-lookup"><span data-stu-id="70780-120">Name</span></span>      |<span data-ttu-id="70780-121">説明</span><span class="sxs-lookup"><span data-stu-id="70780-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70780-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70780-122">Authorization</span></span>  | <span data-ttu-id="70780-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="70780-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70780-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="70780-125">Request body</span></span>
<span data-ttu-id="70780-126">要求本文で無視する危険なユーザー Id を指定します。</span><span class="sxs-lookup"><span data-stu-id="70780-126">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="70780-127">応答</span><span class="sxs-lookup"><span data-stu-id="70780-127">Response</span></span>

<span data-ttu-id="70780-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="70780-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70780-130">例</span><span class="sxs-lookup"><span data-stu-id="70780-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70780-131">要求</span><span class="sxs-lookup"><span data-stu-id="70780-131">Request</span></span>
<span data-ttu-id="70780-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="70780-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="70780-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="70780-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70780-134">C#</span><span class="sxs-lookup"><span data-stu-id="70780-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70780-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="70780-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70780-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="70780-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="70780-137">Java</span><span class="sxs-lookup"><span data-stu-id="70780-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="70780-138">応答</span><span class="sxs-lookup"><span data-stu-id="70780-138">Response</span></span>
<span data-ttu-id="70780-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="70780-139">Here is an example of the response.</span></span>
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
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
