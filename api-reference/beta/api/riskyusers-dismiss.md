---
title: RiskyUser を閉じる
description: RiskyUser オブジェクトのリスクを無視します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 7812235ceecc1304711c715e2aaa6640e684277e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358210"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="fe648-103">riskyUser: 閉じる</span><span class="sxs-lookup"><span data-stu-id="fe648-103">riskyUser: dismiss</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="fe648-104">**注:** RiskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="fe648-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="fe648-105">1つまたは複数の[riskyUser](../resources/riskyuser.md)オブジェクトのリスクを無視します。</span><span class="sxs-lookup"><span data-stu-id="fe648-105">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="fe648-106">このアクションは、対象ユーザーのリスクレベルを [なし] に設定します。</span><span class="sxs-lookup"><span data-stu-id="fe648-106">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe648-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe648-107">Permissions</span></span>
<span data-ttu-id="fe648-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe648-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe648-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe648-110">Permission type</span></span>      | <span data-ttu-id="fe648-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe648-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe648-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe648-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe648-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="fe648-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe648-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe648-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe648-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe648-115">Not supported.</span></span>    |
|<span data-ttu-id="fe648-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe648-116">Application</span></span> | <span data-ttu-id="fe648-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="fe648-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe648-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe648-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="fe648-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe648-119">Request headers</span></span>
| <span data-ttu-id="fe648-120">名前</span><span class="sxs-lookup"><span data-stu-id="fe648-120">Name</span></span>      |<span data-ttu-id="fe648-121">説明</span><span class="sxs-lookup"><span data-stu-id="fe648-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fe648-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe648-122">Authorization</span></span>  | <span data-ttu-id="fe648-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe648-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe648-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe648-125">Request body</span></span>
<span data-ttu-id="fe648-126">要求本文で無視する userIds を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe648-126">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="fe648-127">応答</span><span class="sxs-lookup"><span data-stu-id="fe648-127">Response</span></span>

<span data-ttu-id="fe648-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fe648-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe648-130">例</span><span class="sxs-lookup"><span data-stu-id="fe648-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe648-131">要求</span><span class="sxs-lookup"><span data-stu-id="fe648-131">Request</span></span>
<span data-ttu-id="fe648-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe648-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fe648-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fe648-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe648-134">C#</span><span class="sxs-lookup"><span data-stu-id="fe648-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe648-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe648-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe648-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="fe648-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fe648-137">Java</span><span class="sxs-lookup"><span data-stu-id="fe648-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fe648-138">応答</span><span class="sxs-lookup"><span data-stu-id="fe648-138">Response</span></span>
<span data-ttu-id="fe648-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fe648-139">Here is an example of the response.</span></span>
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
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
