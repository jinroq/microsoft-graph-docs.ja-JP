---
title: directoryRoleTemplates を一覧表示する
description: Directoryroletemplate オブジェクトのリストを取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ed83b629715f54ab5d9ff679fee3fc53ad955b0b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260600"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="1a8a4-103">directoryRoleTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1a8a4-103">List directoryRoleTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a8a4-104">Directoryroletemplate オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1a8a4-104">Retrieve a list of directoryroletemplate objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a8a4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1a8a4-105">Permissions</span></span>
<span data-ttu-id="1a8a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a8a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a8a4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a8a4-108">Permission type</span></span>      | <span data-ttu-id="1a8a4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a8a4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a8a4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a8a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a8a4-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a8a4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1a8a4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a8a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a8a4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a8a4-113">Not supported.</span></span>    |
|<span data-ttu-id="1a8a4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a8a4-114">Application</span></span> | <span data-ttu-id="1a8a4-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a8a4-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a8a4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a8a4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a8a4-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1a8a4-117">Optional query parameters</span></span>
<span data-ttu-id="1a8a4-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="1a8a4-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a8a4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a8a4-119">Request headers</span></span>
| <span data-ttu-id="1a8a4-120">名前</span><span class="sxs-lookup"><span data-stu-id="1a8a4-120">Name</span></span>       | <span data-ttu-id="1a8a4-121">型</span><span class="sxs-lookup"><span data-stu-id="1a8a4-121">Type</span></span> | <span data-ttu-id="1a8a4-122">説明</span><span class="sxs-lookup"><span data-stu-id="1a8a4-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a8a4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a8a4-123">Authorization</span></span>  | <span data-ttu-id="1a8a4-124">string</span><span class="sxs-lookup"><span data-stu-id="1a8a4-124">string</span></span>  | <span data-ttu-id="1a8a4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1a8a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a8a4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a8a4-127">Request body</span></span>
<span data-ttu-id="1a8a4-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1a8a4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a8a4-129">応答</span><span class="sxs-lookup"><span data-stu-id="1a8a4-129">Response</span></span>

<span data-ttu-id="1a8a4-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRoleTemplate](../resources/directoryroletemplate.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1a8a4-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a8a4-131">例</span><span class="sxs-lookup"><span data-stu-id="1a8a4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a8a4-132">要求</span><span class="sxs-lookup"><span data-stu-id="1a8a4-132">Request</span></span>
<span data-ttu-id="1a8a4-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a8a4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="1a8a4-134">応答</span><span class="sxs-lookup"><span data-stu-id="1a8a4-134">Response</span></span>
<span data-ttu-id="1a8a4-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a8a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 139

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1a8a4-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1a8a4-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1a8a4-139">C#</span><span class="sxs-lookup"><span data-stu-id="1a8a4-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryroletemplates-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a8a4-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a8a4-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryroletemplates-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1a8a4-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="1a8a4-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directoryroletemplates-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryroletemplate-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryroletemplate-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryroletemplate-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
