---
title: RiskyUser の履歴を一覧表示する
description: リスク履歴を取得する
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87f19d4e573221baa0253707a97bbe73f496aed5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630455"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="76af1-103">RiskyUser の履歴を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="76af1-103">List history of riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76af1-104">[RiskyUser](../resources/riskyuser.md)リソースのリスク履歴を取得します。</span><span class="sxs-lookup"><span data-stu-id="76af1-104">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="76af1-105">**注:** RiskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="76af1-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="76af1-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="76af1-106">Permissions</span></span>
<span data-ttu-id="76af1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76af1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76af1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76af1-109">Permission type</span></span>      | <span data-ttu-id="76af1-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="76af1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76af1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76af1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="76af1-112">IdentityRiskyUser、IdentityRiskUser のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="76af1-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="76af1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76af1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76af1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76af1-114">Not supported.</span></span>    |
|<span data-ttu-id="76af1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76af1-115">Application</span></span> | <span data-ttu-id="76af1-116">IdentityRiskyUser、IdentityRiskUser のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="76af1-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76af1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76af1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
```


## <a name="request-headers"></a><span data-ttu-id="76af1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76af1-118">Request headers</span></span>
| <span data-ttu-id="76af1-119">名前</span><span class="sxs-lookup"><span data-stu-id="76af1-119">Name</span></span>      |<span data-ttu-id="76af1-120">説明</span><span class="sxs-lookup"><span data-stu-id="76af1-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76af1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="76af1-121">Authorization</span></span>  | <span data-ttu-id="76af1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="76af1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76af1-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="76af1-124">Request body</span></span>
<span data-ttu-id="76af1-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="76af1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76af1-126">応答</span><span class="sxs-lookup"><span data-stu-id="76af1-126">Response</span></span>

<span data-ttu-id="76af1-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="76af1-127">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76af1-128">例</span><span class="sxs-lookup"><span data-stu-id="76af1-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76af1-129">要求</span><span class="sxs-lookup"><span data-stu-id="76af1-129">Request</span></span>
<span data-ttu-id="76af1-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="76af1-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
##### <a name="response"></a><span data-ttu-id="76af1-131">応答</span><span class="sxs-lookup"><span data-stu-id="76af1-131">Response</span></span>
<span data-ttu-id="76af1-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="76af1-132">Here is an example of the response.</span></span>
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user risk history",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

