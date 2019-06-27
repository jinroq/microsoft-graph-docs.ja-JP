---
title: privilegedRoleSummary を取得する
description: PrivilegedRoleSummary オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 91e62e204f007bb4cfddfba5409e94d263047615
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268090"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="3ee03-103">privilegedRoleSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="3ee03-103">Get privilegedRoleSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ee03-104">[PrivilegedRoleSummary](../resources/privilegedrolesummary.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="3ee03-104">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ee03-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3ee03-105">Permissions</span></span>
<span data-ttu-id="3ee03-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ee03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3ee03-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ee03-108">Permission type</span></span>      | <span data-ttu-id="3ee03-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ee03-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ee03-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ee03-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ee03-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ee03-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ee03-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ee03-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ee03-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ee03-113">Not supported.</span></span>    |
|<span data-ttu-id="3ee03-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ee03-114">Application</span></span> | <span data-ttu-id="3ee03-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ee03-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ee03-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ee03-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3ee03-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3ee03-117">Optional query parameters</span></span>
<span data-ttu-id="3ee03-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3ee03-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ee03-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ee03-119">Request headers</span></span>
| <span data-ttu-id="3ee03-120">名前</span><span class="sxs-lookup"><span data-stu-id="3ee03-120">Name</span></span>      |<span data-ttu-id="3ee03-121">説明</span><span class="sxs-lookup"><span data-stu-id="3ee03-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3ee03-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ee03-122">Authorization</span></span>  | <span data-ttu-id="3ee03-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3ee03-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ee03-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ee03-125">Request body</span></span>
<span data-ttu-id="3ee03-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3ee03-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ee03-127">応答</span><span class="sxs-lookup"><span data-stu-id="3ee03-127">Response</span></span>

<span data-ttu-id="3ee03-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleSummary](../resources/privilegedrolesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3ee03-128">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="3ee03-129">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3ee03-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="3ee03-130">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="3ee03-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="3ee03-131">例</span><span class="sxs-lookup"><span data-stu-id="3ee03-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ee03-132">要求</span><span class="sxs-lookup"><span data-stu-id="3ee03-132">Request</span></span>
<span data-ttu-id="3ee03-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3ee03-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="3ee03-134">応答</span><span class="sxs-lookup"><span data-stu-id="3ee03-134">Response</span></span>
<span data-ttu-id="3ee03-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3ee03-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3ee03-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="3ee03-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3ee03-139">C#</span><span class="sxs-lookup"><span data-stu-id="3ee03-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedrolesummary-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ee03-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="3ee03-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedrolesummary-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3ee03-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="3ee03-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_privilegedrolesummary-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesummary-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedrolesummary-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrolesummary-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
