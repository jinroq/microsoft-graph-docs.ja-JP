---
title: リスト agreementAcceptances
description: ユーザーの agreementAcceptance オブジェクトのリストを取得します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 22babc13c3b1db4cf143a35ab2119e97c43c822b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517870"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="07c0c-103">リスト agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="07c0c-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07c0c-104">ユーザーの[agreementAcceptance](../resources/agreementacceptance.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="07c0c-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="07c0c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="07c0c-105">Permissions</span></span>
<span data-ttu-id="07c0c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07c0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07c0c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07c0c-108">Permission type</span></span>                        | <span data-ttu-id="07c0c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="07c0c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="07c0c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07c0c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="07c0c-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="07c0c-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="07c0c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07c0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07c0c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07c0c-113">Not supported.</span></span> |
|<span data-ttu-id="07c0c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07c0c-114">Application</span></span>                            | <span data-ttu-id="07c0c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07c0c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07c0c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07c0c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="07c0c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07c0c-117">Request headers</span></span>
| <span data-ttu-id="07c0c-118">名前</span><span class="sxs-lookup"><span data-stu-id="07c0c-118">Name</span></span>      |<span data-ttu-id="07c0c-119">説明</span><span class="sxs-lookup"><span data-stu-id="07c0c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07c0c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="07c0c-120">Authorization</span></span> | <span data-ttu-id="07c0c-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="07c0c-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="07c0c-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="07c0c-122">Request body</span></span>
<span data-ttu-id="07c0c-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="07c0c-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="07c0c-124">応答</span><span class="sxs-lookup"><span data-stu-id="07c0c-124">Response</span></span>
<span data-ttu-id="07c0c-125">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[agreementAcceptance](../resources/agreementacceptance.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="07c0c-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07c0c-126">例</span><span class="sxs-lookup"><span data-stu-id="07c0c-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07c0c-127">要求</span><span class="sxs-lookup"><span data-stu-id="07c0c-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="07c0c-128">応答</span><span class="sxs-lookup"><span data-stu-id="07c0c-128">Response</span></span>
><span data-ttu-id="07c0c-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="07c0c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
