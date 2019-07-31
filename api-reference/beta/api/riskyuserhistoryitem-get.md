---
title: RiskyUser の履歴項目を取得する
description: RiskyUser オブジェクトの履歴アイテムを取得します。
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74114055c62ffcbdf7a226e9ba08712587b08f09
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978113"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="cbd85-103">RiskyUserHistoryItem を取得する</span><span class="sxs-lookup"><span data-stu-id="cbd85-103">Get riskyUserHistoryItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbd85-104">[RiskyUser](../resources/riskyuser.md)の[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbd85-104">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="cbd85-105">**注:** RiskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="cbd85-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbd85-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cbd85-106">Permissions</span></span>
<span data-ttu-id="cbd85-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbd85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbd85-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cbd85-109">Permission type</span></span>      | <span data-ttu-id="cbd85-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cbd85-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbd85-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cbd85-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cbd85-112">IdentityRiskyUser、IdentityRiskUser のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbd85-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="cbd85-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cbd85-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbd85-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbd85-114">Not supported.</span></span>    |
|<span data-ttu-id="cbd85-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cbd85-115">Application</span></span> | <span data-ttu-id="cbd85-116">IdentityRiskyUser、IdentityRiskUser のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbd85-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbd85-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cbd85-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="cbd85-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbd85-118">Request headers</span></span>
| <span data-ttu-id="cbd85-119">名前</span><span class="sxs-lookup"><span data-stu-id="cbd85-119">Name</span></span>      |<span data-ttu-id="cbd85-120">説明</span><span class="sxs-lookup"><span data-stu-id="cbd85-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cbd85-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbd85-121">Authorization</span></span>  | <span data-ttu-id="cbd85-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cbd85-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbd85-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="cbd85-124">Request body</span></span>
<span data-ttu-id="cbd85-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cbd85-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbd85-126">応答</span><span class="sxs-lookup"><span data-stu-id="cbd85-126">Response</span></span>

<span data-ttu-id="cbd85-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cbd85-127">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cbd85-128">例</span><span class="sxs-lookup"><span data-stu-id="cbd85-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbd85-129">要求</span><span class="sxs-lookup"><span data-stu-id="cbd85-129">Request</span></span>
<span data-ttu-id="cbd85-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cbd85-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cbd85-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cbd85-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cbd85-132">C#</span><span class="sxs-lookup"><span data-stu-id="cbd85-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbd85-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="cbd85-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cbd85-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="cbd85-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cbd85-135">Java</span><span class="sxs-lookup"><span data-stu-id="cbd85-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-historyitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cbd85-136">応答</span><span class="sxs-lookup"><span data-stu-id="cbd85-136">Response</span></span>
<span data-ttu-id="cbd85-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cbd85-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "isDeleted": false,
    "isGuest": false,
    "isProcessing": false,
    "riskLevel": "none",
    "riskState": "remediated",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "riskLastUpdatedDateTime": "2019-05-03T03:50:34.9565578Z",
    "userDisplayName": "Allan Deyoung",
    "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
    "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
    "activity": {
        "eventTypes": [],
        "detail": "userPerformedSecuredPasswordReset"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUserHistoryItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

