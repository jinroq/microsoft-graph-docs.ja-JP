---
title: directoryObject を取得する
description: directoryObject オブジェクトのプロパティとリレーションシップを取得します。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ee35563a3b2e89c2d43cf683745afff202f69d1
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657001"
---
# <a name="get-directoryobject"></a><span data-ttu-id="fe8d8-103">directoryObject を取得する</span><span class="sxs-lookup"><span data-stu-id="fe8d8-103">Get directoryObject</span></span>

<span data-ttu-id="fe8d8-104">directoryObject オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-104">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe8d8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe8d8-105">Permissions</span></span>
<span data-ttu-id="fe8d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe8d8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe8d8-108">Permission type</span></span>      | <span data-ttu-id="fe8d8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe8d8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe8d8-111">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fe8d8-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fe8d8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe8d8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-113">Not supported.</span></span>    |
|<span data-ttu-id="fe8d8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe8d8-114">Application</span></span> | <span data-ttu-id="fe8d8-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe8d8-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe8d8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe8d8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe8d8-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fe8d8-117">Optional query parameters</span></span>
<span data-ttu-id="fe8d8-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fe8d8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe8d8-119">Request headers</span></span>
| <span data-ttu-id="fe8d8-120">名前</span><span class="sxs-lookup"><span data-stu-id="fe8d8-120">Name</span></span>       | <span data-ttu-id="fe8d8-121">型</span><span class="sxs-lookup"><span data-stu-id="fe8d8-121">Type</span></span> | <span data-ttu-id="fe8d8-122">説明</span><span class="sxs-lookup"><span data-stu-id="fe8d8-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fe8d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe8d8-123">Authorization</span></span>  | <span data-ttu-id="fe8d8-124">string</span><span class="sxs-lookup"><span data-stu-id="fe8d8-124">string</span></span>  | <span data-ttu-id="fe8d8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe8d8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe8d8-127">Request body</span></span>
<span data-ttu-id="fe8d8-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe8d8-129">応答</span><span class="sxs-lookup"><span data-stu-id="fe8d8-129">Response</span></span>

<span data-ttu-id="fe8d8-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe8d8-131">例</span><span class="sxs-lookup"><span data-stu-id="fe8d8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe8d8-132">要求</span><span class="sxs-lookup"><span data-stu-id="fe8d8-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="fe8d8-133">応答</span><span class="sxs-lookup"><span data-stu-id="fe8d8-133">Response</span></span>
<span data-ttu-id="fe8d8-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fe8d8-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="fe8d8-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fe8d8-137">C#</span><span class="sxs-lookup"><span data-stu-id="fe8d8-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryobject-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe8d8-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="fe8d8-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryobject-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
