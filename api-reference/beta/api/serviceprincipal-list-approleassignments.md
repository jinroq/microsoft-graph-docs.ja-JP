---
title: 'servicePrincipal: appRoleAssignments のリスト'
description: Approleassignment オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: 4ecbd1cfe757900429abf77cd05b8f3f3f563d83
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263806"
---
# <a name="serviceprincipal-list-approleassignments"></a><span data-ttu-id="835df-103">servicePrincipal: appRoleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="835df-103">servicePrincipal: List appRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="835df-104">Approleassignment オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="835df-104">Retrieve a list of approleassignment objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="835df-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="835df-105">Permissions</span></span>
<span data-ttu-id="835df-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="835df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="835df-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="835df-108">Permission type</span></span>      | <span data-ttu-id="835df-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="835df-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="835df-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="835df-110">Delegated (work or school account)</span></span> | <span data-ttu-id="835df-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="835df-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="835df-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="835df-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="835df-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="835df-113">Not supported.</span></span>    |
|<span data-ttu-id="835df-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="835df-114">Application</span></span> | <span data-ttu-id="835df-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="835df-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="835df-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="835df-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="835df-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="835df-117">Optional query parameters</span></span>
<span data-ttu-id="835df-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="835df-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="835df-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="835df-119">Request headers</span></span>
| <span data-ttu-id="835df-120">名前</span><span class="sxs-lookup"><span data-stu-id="835df-120">Name</span></span>       | <span data-ttu-id="835df-121">型</span><span class="sxs-lookup"><span data-stu-id="835df-121">Type</span></span> | <span data-ttu-id="835df-122">説明</span><span class="sxs-lookup"><span data-stu-id="835df-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="835df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="835df-123">Authorization</span></span>  | <span data-ttu-id="835df-124">string</span><span class="sxs-lookup"><span data-stu-id="835df-124">string</span></span>  | <span data-ttu-id="835df-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="835df-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="835df-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="835df-127">Request body</span></span>
<span data-ttu-id="835df-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="835df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="835df-129">応答</span><span class="sxs-lookup"><span data-stu-id="835df-129">Response</span></span>

<span data-ttu-id="835df-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[approleassignment](../resources/approleassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="835df-130">If successful, this method returns a `200 OK` response code and collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="835df-131">例</span><span class="sxs-lookup"><span data-stu-id="835df-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="835df-132">要求</span><span class="sxs-lookup"><span data-stu-id="835df-132">Request</span></span>
<span data-ttu-id="835df-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="835df-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="835df-134">応答</span><span class="sxs-lookup"><span data-stu-id="835df-134">Response</span></span>
<span data-ttu-id="835df-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="835df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="835df-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="835df-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="835df-139">C#</span><span class="sxs-lookup"><span data-stu-id="835df-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_approleassignments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="835df-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="835df-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_approleassignments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="835df-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="835df-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_approleassignments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-approleassignments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/serviceprincipal-list-approleassignments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list-approleassignments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
