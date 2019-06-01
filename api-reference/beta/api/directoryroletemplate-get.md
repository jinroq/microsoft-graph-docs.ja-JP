---
title: directoryRoleTemplate を取得する
description: directoryroletemplate オブジェクトのプロパティと関係を取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: edea45d9bbf2c24fc112d19812773a9b2b6ee5e0
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655888"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="151be-103">directoryRoleTemplate を取得する</span><span class="sxs-lookup"><span data-stu-id="151be-103">Get directoryRoleTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="151be-104">directoryroletemplate オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="151be-104">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="151be-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="151be-105">Permissions</span></span>
<span data-ttu-id="151be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="151be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="151be-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="151be-108">Permission type</span></span>      | <span data-ttu-id="151be-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="151be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="151be-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="151be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="151be-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="151be-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="151be-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="151be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="151be-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="151be-113">Not supported.</span></span>    |
|<span data-ttu-id="151be-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="151be-114">Application</span></span> | <span data-ttu-id="151be-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="151be-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="151be-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="151be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="151be-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="151be-117">Optional query parameters</span></span>
<span data-ttu-id="151be-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="151be-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="151be-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="151be-119">Request headers</span></span>
| <span data-ttu-id="151be-120">名前</span><span class="sxs-lookup"><span data-stu-id="151be-120">Name</span></span>       | <span data-ttu-id="151be-121">型</span><span class="sxs-lookup"><span data-stu-id="151be-121">Type</span></span> | <span data-ttu-id="151be-122">説明</span><span class="sxs-lookup"><span data-stu-id="151be-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="151be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="151be-123">Authorization</span></span>  | <span data-ttu-id="151be-124">string</span><span class="sxs-lookup"><span data-stu-id="151be-124">string</span></span>  | <span data-ttu-id="151be-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="151be-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="151be-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="151be-127">Request body</span></span>
<span data-ttu-id="151be-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="151be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="151be-129">応答</span><span class="sxs-lookup"><span data-stu-id="151be-129">Response</span></span>

<span data-ttu-id="151be-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRoleTemplate](../resources/directoryroletemplate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="151be-130">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="151be-131">例</span><span class="sxs-lookup"><span data-stu-id="151be-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="151be-132">要求</span><span class="sxs-lookup"><span data-stu-id="151be-132">Request</span></span>
<span data-ttu-id="151be-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="151be-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoleTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="151be-134">応答</span><span class="sxs-lookup"><span data-stu-id="151be-134">Response</span></span>
<span data-ttu-id="151be-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="151be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="151be-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="151be-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="151be-139">C#</span><span class="sxs-lookup"><span data-stu-id="151be-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryroletemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="151be-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="151be-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryroletemplate-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryroletemplate-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryroletemplate-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
