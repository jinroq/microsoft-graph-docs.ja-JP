---
title: RiskyUser の履歴を一覧表示する
description: リスク履歴を取得する
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e33303b64cf9ff8b83e86a080e0c39ccf7c5f83c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267068"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="2017a-103">RiskyUser の履歴を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2017a-103">List history of riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2017a-104">[RiskyUser](../resources/riskyuser.md)リソースのリスク履歴を取得します。</span><span class="sxs-lookup"><span data-stu-id="2017a-104">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="2017a-105">**注:** RiskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="2017a-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="2017a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2017a-106">Permissions</span></span>
<span data-ttu-id="2017a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2017a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2017a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2017a-109">Permission type</span></span>      | <span data-ttu-id="2017a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2017a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2017a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2017a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2017a-112">IdentityRiskyUser、IdentityRiskUser のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="2017a-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="2017a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2017a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2017a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2017a-114">Not supported.</span></span>    |
|<span data-ttu-id="2017a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2017a-115">Application</span></span> | <span data-ttu-id="2017a-116">IdentityRiskyUser、IdentityRiskUser のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="2017a-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2017a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2017a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
```


## <a name="request-headers"></a><span data-ttu-id="2017a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2017a-118">Request headers</span></span>
| <span data-ttu-id="2017a-119">名前</span><span class="sxs-lookup"><span data-stu-id="2017a-119">Name</span></span>      |<span data-ttu-id="2017a-120">説明</span><span class="sxs-lookup"><span data-stu-id="2017a-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2017a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2017a-121">Authorization</span></span>  | <span data-ttu-id="2017a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2017a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2017a-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="2017a-124">Request body</span></span>
<span data-ttu-id="2017a-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2017a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2017a-126">応答</span><span class="sxs-lookup"><span data-stu-id="2017a-126">Response</span></span>

<span data-ttu-id="2017a-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2017a-127">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2017a-128">例</span><span class="sxs-lookup"><span data-stu-id="2017a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2017a-129">要求</span><span class="sxs-lookup"><span data-stu-id="2017a-129">Request</span></span>
<span data-ttu-id="2017a-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2017a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
##### <a name="response"></a><span data-ttu-id="2017a-131">応答</span><span class="sxs-lookup"><span data-stu-id="2017a-131">Response</span></span>
<span data-ttu-id="2017a-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2017a-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers('41a31b00-3b3b-42d9-8f1c-6d4f14e74c69')/history",
    "value": [
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
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901009342322587",
            "isDeleted": false,
            "isGuest": false,
            "isProcessing": false,
            "riskLevel": "high",
            "riskState": "atRisk",
            "riskDetail": "none",
            "riskLastUpdatedDateTime": "2019-04-05T22:31:27Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": null,
            "activity": {
                "eventTypes": [
                    "anonymizedIPAddress"
                ],
                "detail": null
            }
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901020140973557",
            "isDeleted": false,
            "isGuest": false,
            "isProcessing": false,
            "riskLevel": "none",
            "riskState": "remediated",
            "riskDetail": "userPerformedSecuredPasswordReset",
            "riskLastUpdatedDateTime": "2019-04-05T23:00:14.0973557Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
            "activity": {
                "eventTypes": [],
                "detail": "userPerformedSecuredPasswordReset"
            }
        }
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2017a-133">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="2017a-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2017a-134">C#</span><span class="sxs-lookup"><span data-stu-id="2017a-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_userriskhitsory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2017a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="2017a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_userriskhitsory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2017a-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="2017a-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_userriskhitsory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user risk history",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyuser-list-history.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyuser-list-history.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyuser-list-history.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

