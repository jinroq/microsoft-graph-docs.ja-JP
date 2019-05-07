---
title: RiskyUser が侵害されたことを確認する
description: RiskyUser オブジェクトが侵害されていることを確認します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: f0ce7b0a29b90f12104a697bdc38f3297e52676e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639034"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="dbad6-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="dbad6-103">riskyUser: confirmCompromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="dbad6-104">**注:** RiskyUsers API には、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="dbad6-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="dbad6-105">1つまたは複数の[riskyUser](../resources/riskyuser.md)オブジェクトが侵害されたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="dbad6-105">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="dbad6-106">このアクションは、対象ユーザーのリスクレベルを [高」に設定します。</span><span class="sxs-lookup"><span data-stu-id="dbad6-106">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbad6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dbad6-107">Permissions</span></span>
<span data-ttu-id="dbad6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dbad6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbad6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dbad6-110">Permission type</span></span>      | <span data-ttu-id="dbad6-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dbad6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbad6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dbad6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dbad6-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="dbad6-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbad6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dbad6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbad6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dbad6-115">Not supported.</span></span>    |
|<span data-ttu-id="dbad6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dbad6-116">Application</span></span> | <span data-ttu-id="dbad6-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="dbad6-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbad6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dbad6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="dbad6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dbad6-119">Request headers</span></span>
| <span data-ttu-id="dbad6-120">名前</span><span class="sxs-lookup"><span data-stu-id="dbad6-120">Name</span></span>      |<span data-ttu-id="dbad6-121">説明</span><span class="sxs-lookup"><span data-stu-id="dbad6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dbad6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbad6-122">Authorization</span></span>  | <span data-ttu-id="dbad6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dbad6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbad6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="dbad6-125">Request body</span></span>
<span data-ttu-id="dbad6-126">要求本文で無視する危険なユーザー Id を指定します。</span><span class="sxs-lookup"><span data-stu-id="dbad6-126">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="dbad6-127">応答</span><span class="sxs-lookup"><span data-stu-id="dbad6-127">Response</span></span>

<span data-ttu-id="dbad6-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="dbad6-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dbad6-130">例</span><span class="sxs-lookup"><span data-stu-id="dbad6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbad6-131">要求</span><span class="sxs-lookup"><span data-stu-id="dbad6-131">Request</span></span>
<span data-ttu-id="dbad6-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dbad6-132">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="dbad6-133">応答</span><span class="sxs-lookup"><span data-stu-id="dbad6-133">Response</span></span>
<span data-ttu-id="dbad6-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dbad6-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dbad6-135">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="dbad6-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dbad6-136">Visual</span><span class="sxs-lookup"><span data-stu-id="dbad6-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/confirm_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbad6-137">Java</span><span class="sxs-lookup"><span data-stu-id="dbad6-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/confirm_riskyuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
