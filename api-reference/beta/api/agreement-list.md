---
title: 契約を一覧表示する
description: アグリーメントオブジェクトの一覧を取得します。
localization_priority: Normal
ms.openlocfilehash: 82674e81b6b059ffafedf3b9c15c19e90438dc28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459203"
---
# <a name="list-agreements"></a><span data-ttu-id="f557b-103">契約を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f557b-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f557b-104">[アグリーメント](../resources/agreement.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f557b-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f557b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f557b-105">Permissions</span></span>
<span data-ttu-id="f557b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f557b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f557b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f557b-108">Permission type</span></span>                        | <span data-ttu-id="f557b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f557b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f557b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f557b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f557b-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="f557b-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="f557b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f557b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f557b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f557b-113">Not supported.</span></span> |
|<span data-ttu-id="f557b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f557b-114">Application</span></span>                            | <span data-ttu-id="f557b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f557b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f557b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f557b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="f557b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f557b-117">Request headers</span></span>
| <span data-ttu-id="f557b-118">名前</span><span class="sxs-lookup"><span data-stu-id="f557b-118">Name</span></span>         | <span data-ttu-id="f557b-119">型</span><span class="sxs-lookup"><span data-stu-id="f557b-119">Type</span></span>        | <span data-ttu-id="f557b-120">説明</span><span class="sxs-lookup"><span data-stu-id="f557b-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f557b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f557b-121">Authorization</span></span> | <span data-ttu-id="f557b-122">string</span><span class="sxs-lookup"><span data-stu-id="f557b-122">string</span></span> | <span data-ttu-id="f557b-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="f557b-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f557b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f557b-125">Request body</span></span>
<span data-ttu-id="f557b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f557b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f557b-127">応答</span><span class="sxs-lookup"><span data-stu-id="f557b-127">Response</span></span>
<span data-ttu-id="f557b-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[アグリーメント](../resources/agreement.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f557b-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f557b-129">例</span><span class="sxs-lookup"><span data-stu-id="f557b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f557b-130">要求</span><span class="sxs-lookup"><span data-stu-id="f557b-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="f557b-131">応答</span><span class="sxs-lookup"><span data-stu-id="f557b-131">Response</span></span>
><span data-ttu-id="f557b-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f557b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
