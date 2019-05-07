---
title: 契約を一覧表示する
description: アグリーメントオブジェクトの一覧を取得します。
localization_priority: Normal
ms.openlocfilehash: 3d0594f37a3d88f7ff1ba9ea543e3b2d21ebc63a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636626"
---
# <a name="list-agreements"></a><span data-ttu-id="d1cc3-103">契約を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d1cc3-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1cc3-104">[アグリーメント](../resources/agreement.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d1cc3-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1cc3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d1cc3-105">Permissions</span></span>
<span data-ttu-id="d1cc3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1cc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1cc3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1cc3-108">Permission type</span></span>                        | <span data-ttu-id="d1cc3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1cc3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1cc3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1cc3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1cc3-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1cc3-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="d1cc3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1cc3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1cc3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1cc3-113">Not supported.</span></span> |
|<span data-ttu-id="d1cc3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1cc3-114">Application</span></span>                            | <span data-ttu-id="d1cc3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1cc3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1cc3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1cc3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="d1cc3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1cc3-117">Request headers</span></span>
| <span data-ttu-id="d1cc3-118">名前</span><span class="sxs-lookup"><span data-stu-id="d1cc3-118">Name</span></span>         | <span data-ttu-id="d1cc3-119">型</span><span class="sxs-lookup"><span data-stu-id="d1cc3-119">Type</span></span>        | <span data-ttu-id="d1cc3-120">説明</span><span class="sxs-lookup"><span data-stu-id="d1cc3-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d1cc3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1cc3-121">Authorization</span></span> | <span data-ttu-id="d1cc3-122">string</span><span class="sxs-lookup"><span data-stu-id="d1cc3-122">string</span></span> | <span data-ttu-id="d1cc3-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="d1cc3-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1cc3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1cc3-125">Request body</span></span>
<span data-ttu-id="d1cc3-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d1cc3-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d1cc3-127">応答</span><span class="sxs-lookup"><span data-stu-id="d1cc3-127">Response</span></span>
<span data-ttu-id="d1cc3-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[アグリーメント](../resources/agreement.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d1cc3-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1cc3-129">例</span><span class="sxs-lookup"><span data-stu-id="d1cc3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1cc3-130">要求</span><span class="sxs-lookup"><span data-stu-id="d1cc3-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="d1cc3-131">応答</span><span class="sxs-lookup"><span data-stu-id="d1cc3-131">Response</span></span>
><span data-ttu-id="d1cc3-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d1cc3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d1cc3-134">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="d1cc3-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d1cc3-135">Visual</span><span class="sxs-lookup"><span data-stu-id="d1cc3-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_agreements-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1cc3-136">Java</span><span class="sxs-lookup"><span data-stu-id="d1cc3-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_agreements-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/agreement-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
