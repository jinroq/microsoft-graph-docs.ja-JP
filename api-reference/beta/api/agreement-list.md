---
title: リスト契約
description: 契約オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: 82674e81b6b059ffafedf3b9c15c19e90438dc28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525977"
---
# <a name="list-agreements"></a><span data-ttu-id="044bc-103">リスト契約</span><span class="sxs-lookup"><span data-stu-id="044bc-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="044bc-104">[契約](../resources/agreement.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="044bc-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="044bc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="044bc-105">Permissions</span></span>
<span data-ttu-id="044bc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="044bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="044bc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="044bc-108">Permission type</span></span>                        | <span data-ttu-id="044bc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="044bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="044bc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="044bc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="044bc-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="044bc-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="044bc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="044bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="044bc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="044bc-113">Not supported.</span></span> |
|<span data-ttu-id="044bc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="044bc-114">Application</span></span>                            | <span data-ttu-id="044bc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="044bc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="044bc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="044bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="044bc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="044bc-117">Request headers</span></span>
| <span data-ttu-id="044bc-118">名前</span><span class="sxs-lookup"><span data-stu-id="044bc-118">Name</span></span>         | <span data-ttu-id="044bc-119">型</span><span class="sxs-lookup"><span data-stu-id="044bc-119">Type</span></span>        | <span data-ttu-id="044bc-120">説明</span><span class="sxs-lookup"><span data-stu-id="044bc-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="044bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="044bc-121">Authorization</span></span> | <span data-ttu-id="044bc-122">string</span><span class="sxs-lookup"><span data-stu-id="044bc-122">string</span></span> | <span data-ttu-id="044bc-123">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="044bc-123">Bearer \{token\}.</span></span> <span data-ttu-id="044bc-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="044bc-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="044bc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="044bc-125">Request body</span></span>
<span data-ttu-id="044bc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="044bc-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="044bc-127">応答</span><span class="sxs-lookup"><span data-stu-id="044bc-127">Response</span></span>
<span data-ttu-id="044bc-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[許可書](../resources/agreement.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="044bc-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="044bc-129">例</span><span class="sxs-lookup"><span data-stu-id="044bc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="044bc-130">要求</span><span class="sxs-lookup"><span data-stu-id="044bc-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="044bc-131">応答</span><span class="sxs-lookup"><span data-stu-id="044bc-131">Response</span></span>
><span data-ttu-id="044bc-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="044bc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
