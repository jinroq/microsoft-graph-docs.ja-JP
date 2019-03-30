---
title: riskyUsers を取得する
description: '**riskyUsers**オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b65135fcd1ad77304b98f18fa595154aee984910
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003714"
---
# <a name="get-riskyusers"></a><span data-ttu-id="244e3-103">riskyUsers を取得する</span><span class="sxs-lookup"><span data-stu-id="244e3-103">Get riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="244e3-104">**riskyUsers**オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="244e3-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

><span data-ttu-id="244e3-105">**注:** riskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="244e3-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="244e3-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="244e3-106">Permissions</span></span>
<span data-ttu-id="244e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="244e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="244e3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="244e3-109">Permission type</span></span>      | <span data-ttu-id="244e3-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="244e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="244e3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="244e3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="244e3-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="244e3-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="244e3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="244e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="244e3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="244e3-114">Not supported.</span></span>    |
|<span data-ttu-id="244e3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="244e3-115">Application</span></span> | <span data-ttu-id="244e3-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="244e3-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="244e3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="244e3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="244e3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="244e3-118">Request headers</span></span>
| <span data-ttu-id="244e3-119">名前</span><span class="sxs-lookup"><span data-stu-id="244e3-119">Name</span></span>      |<span data-ttu-id="244e3-120">説明</span><span class="sxs-lookup"><span data-stu-id="244e3-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="244e3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="244e3-121">Authorization</span></span>  | <span data-ttu-id="244e3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="244e3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="244e3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="244e3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="244e3-125">変更を保存するかどうかを決定するブックセッション ID。</span><span class="sxs-lookup"><span data-stu-id="244e3-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="244e3-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="244e3-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="244e3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="244e3-127">Request body</span></span>
<span data-ttu-id="244e3-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="244e3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="244e3-129">応答</span><span class="sxs-lookup"><span data-stu-id="244e3-129">Response</span></span>

<span data-ttu-id="244e3-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[riskyUser](../resources/riskyUser.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="244e3-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyUser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="244e3-131">例</span><span class="sxs-lookup"><span data-stu-id="244e3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="244e3-132">要求</span><span class="sxs-lookup"><span data-stu-id="244e3-132">Request</span></span>
<span data-ttu-id="244e3-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="244e3-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="244e3-134">応答</span><span class="sxs-lookup"><span data-stu-id="244e3-134">Response</span></span>
<span data-ttu-id="244e3-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="244e3-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": "true",
  "isProcessing": true,
  "isDeleted": "true",
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk"
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

