---
title: RiskyUsers を取得します。
description: プロパティと、 **riskyUsers**オブジェクトの関係を取得します。
ms.openlocfilehash: 14a944012a8015ecf3c60f761edba680c2c7a68b
ms.sourcegitcommit: ba6b1d1a12dcb54916b4d3e529c856f6514e01e7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/12/2018
ms.locfileid: "27241028"
---
# <a name="get-riskyusers"></a><span data-ttu-id="1404c-103">RiskyUsers を取得します。</span><span class="sxs-lookup"><span data-stu-id="1404c-103">Get riskyUsers</span></span>

> <span data-ttu-id="1404c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1404c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1404c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1404c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1404c-106">プロパティと、 **riskyUsers**オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="1404c-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="1404c-107">**注:** この API には、Azure AD プレミアム P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="1404c-107">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="1404c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1404c-108">Permissions</span></span>
<span data-ttu-id="1404c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1404c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1404c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1404c-111">Permission type</span></span>      | <span data-ttu-id="1404c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1404c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1404c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1404c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1404c-114">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="1404c-114">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="1404c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1404c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1404c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1404c-116">Not supported.</span></span>    |
|<span data-ttu-id="1404c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1404c-117">Application</span></span> | <span data-ttu-id="1404c-118">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="1404c-118">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1404c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1404c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="1404c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1404c-120">Request headers</span></span>
| <span data-ttu-id="1404c-121">名前</span><span class="sxs-lookup"><span data-stu-id="1404c-121">Name</span></span>      |<span data-ttu-id="1404c-122">説明</span><span class="sxs-lookup"><span data-stu-id="1404c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1404c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1404c-123">Authorization</span></span>  | <span data-ttu-id="1404c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1404c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1404c-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1404c-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="1404c-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1404c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1404c-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="1404c-129">Request body</span></span>
<span data-ttu-id="1404c-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1404c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1404c-131">応答</span><span class="sxs-lookup"><span data-stu-id="1404c-131">Response</span></span>

<span data-ttu-id="1404c-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[riskyUser](../resources/riskyuser.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1404c-132">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1404c-133">例</span><span class="sxs-lookup"><span data-stu-id="1404c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1404c-134">要求</span><span class="sxs-lookup"><span data-stu-id="1404c-134">Request</span></span>
<span data-ttu-id="1404c-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1404c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="1404c-136">応答</span><span class="sxs-lookup"><span data-stu-id="1404c-136">Response</span></span>
<span data-ttu-id="1404c-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1404c-137">Here is an example of the response.</span></span>
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