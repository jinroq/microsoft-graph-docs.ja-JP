---
title: RiskyUser の履歴項目を取得する
description: RiskyUser オブジェクトの履歴アイテムを取得します。
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cc5f365a1ee5503b9ee756955ea37037c14e8c5e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630448"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="99b44-103">RiskyUserHistoryItem を取得する</span><span class="sxs-lookup"><span data-stu-id="99b44-103">Get riskyUserHistoryItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99b44-104">[RiskyUser](../resources/riskyuser.md)の[RiskyUserHistoryItem](../resources/riskyuserhistoryitem.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="99b44-104">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="99b44-105">**注:** RiskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="99b44-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="99b44-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="99b44-106">Permissions</span></span>
<span data-ttu-id="99b44-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99b44-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="99b44-109">Permission type</span></span>      | <span data-ttu-id="99b44-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="99b44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99b44-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="99b44-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99b44-112">IdentityRiskyUser、IdentityRiskUser のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="99b44-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="99b44-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="99b44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99b44-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99b44-114">Not supported.</span></span>    |
|<span data-ttu-id="99b44-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="99b44-115">Application</span></span> | <span data-ttu-id="99b44-116">IdentityRiskyUser、IdentityRiskUser のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="99b44-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99b44-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="99b44-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="99b44-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99b44-118">Request headers</span></span>
| <span data-ttu-id="99b44-119">名前</span><span class="sxs-lookup"><span data-stu-id="99b44-119">Name</span></span>      |<span data-ttu-id="99b44-120">説明</span><span class="sxs-lookup"><span data-stu-id="99b44-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99b44-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="99b44-121">Authorization</span></span>  | <span data-ttu-id="99b44-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="99b44-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99b44-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="99b44-124">Request body</span></span>
<span data-ttu-id="99b44-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="99b44-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99b44-126">応答</span><span class="sxs-lookup"><span data-stu-id="99b44-126">Response</span></span>

<span data-ttu-id="99b44-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="99b44-127">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99b44-128">例</span><span class="sxs-lookup"><span data-stu-id="99b44-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99b44-129">要求</span><span class="sxs-lookup"><span data-stu-id="99b44-129">Request</span></span>
<span data-ttu-id="99b44-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="99b44-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
##### <a name="response"></a><span data-ttu-id="99b44-131">応答</span><span class="sxs-lookup"><span data-stu-id="99b44-131">Response</span></span>
<span data-ttu-id="99b44-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="99b44-132">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->

