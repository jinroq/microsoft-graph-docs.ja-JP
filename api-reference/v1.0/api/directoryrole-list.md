---
title: directoryRoles を一覧表示する
description: テナントでアクティブになっているディレクトリ ロールを一覧表示します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1d40f7bc48eb98ef42b002da74f9848571e33ff0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272339"
---
# <a name="list-directoryroles"></a><span data-ttu-id="efb3e-103">directoryRoles を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="efb3e-103">List directoryRoles</span></span>

<span data-ttu-id="efb3e-104">テナントでアクティブになっているディレクトリ ロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="efb3e-104">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="efb3e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="efb3e-105">Permissions</span></span>
<span data-ttu-id="efb3e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efb3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efb3e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="efb3e-108">Permission type</span></span>      | <span data-ttu-id="efb3e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="efb3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efb3e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="efb3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="efb3e-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="efb3e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="efb3e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="efb3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efb3e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efb3e-113">Not supported.</span></span>    |
|<span data-ttu-id="efb3e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="efb3e-114">Application</span></span> | <span data-ttu-id="efb3e-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb3e-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efb3e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="efb3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="efb3e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="efb3e-117">Optional query parameters</span></span>
<span data-ttu-id="efb3e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="efb3e-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="efb3e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="efb3e-119">Request headers</span></span>
| <span data-ttu-id="efb3e-120">名前</span><span class="sxs-lookup"><span data-stu-id="efb3e-120">Name</span></span>       | <span data-ttu-id="efb3e-121">型</span><span class="sxs-lookup"><span data-stu-id="efb3e-121">Type</span></span> | <span data-ttu-id="efb3e-122">説明</span><span class="sxs-lookup"><span data-stu-id="efb3e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="efb3e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="efb3e-123">Authorization</span></span>  | <span data-ttu-id="efb3e-124">string</span><span class="sxs-lookup"><span data-stu-id="efb3e-124">string</span></span>  | <span data-ttu-id="efb3e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="efb3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efb3e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="efb3e-127">Request body</span></span>
<span data-ttu-id="efb3e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="efb3e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efb3e-129">応答</span><span class="sxs-lookup"><span data-stu-id="efb3e-129">Response</span></span>

<span data-ttu-id="efb3e-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="efb3e-130">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="efb3e-131">例</span><span class="sxs-lookup"><span data-stu-id="efb3e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="efb3e-132">要求</span><span class="sxs-lookup"><span data-stu-id="efb3e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="efb3e-133">応答</span><span class="sxs-lookup"><span data-stu-id="efb3e-133">Response</span></span>
<span data-ttu-id="efb3e-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="efb3e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="efb3e-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="efb3e-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="efb3e-137">C#</span><span class="sxs-lookup"><span data-stu-id="efb3e-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryroles-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="efb3e-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="efb3e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryroles-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="efb3e-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="efb3e-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directoryroles-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryrole-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryrole-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryrole-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
