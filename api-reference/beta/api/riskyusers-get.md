---
title: RiskyUsers を取得します。
description: プロパティと、 **riskyUsers**オブジェクトの関係を取得します。
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 586e76cd57e720741c6a63bc00374cd0973a1cf3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642346"
---
# <a name="get-riskyusers"></a><span data-ttu-id="f8408-103">RiskyUsers を取得します。</span><span class="sxs-lookup"><span data-stu-id="f8408-103">Get riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8408-104">プロパティと、 **riskyUsers**オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="f8408-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="f8408-105">**注:** この API には、Azure AD プレミアム P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="f8408-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8408-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f8408-106">Permissions</span></span>
<span data-ttu-id="f8408-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8408-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8408-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8408-109">Permission type</span></span>      | <span data-ttu-id="f8408-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8408-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8408-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8408-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8408-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8408-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="f8408-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8408-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8408-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8408-114">Not supported.</span></span>    |
|<span data-ttu-id="f8408-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8408-115">Application</span></span> | <span data-ttu-id="f8408-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8408-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8408-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8408-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="f8408-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8408-118">Request headers</span></span>
| <span data-ttu-id="f8408-119">名前</span><span class="sxs-lookup"><span data-stu-id="f8408-119">Name</span></span>      |<span data-ttu-id="f8408-120">説明</span><span class="sxs-lookup"><span data-stu-id="f8408-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f8408-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8408-121">Authorization</span></span>  | <span data-ttu-id="f8408-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f8408-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f8408-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f8408-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f8408-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f8408-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8408-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8408-127">Request body</span></span>
<span data-ttu-id="f8408-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f8408-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8408-129">応答</span><span class="sxs-lookup"><span data-stu-id="f8408-129">Response</span></span>

<span data-ttu-id="f8408-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[riskyUser](../resources/riskyuser.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f8408-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8408-131">例</span><span class="sxs-lookup"><span data-stu-id="f8408-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8408-132">要求</span><span class="sxs-lookup"><span data-stu-id="f8408-132">Request</span></span>
<span data-ttu-id="f8408-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f8408-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="f8408-134">応答</span><span class="sxs-lookup"><span data-stu-id="f8408-134">Response</span></span>
<span data-ttu-id="f8408-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f8408-135">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
