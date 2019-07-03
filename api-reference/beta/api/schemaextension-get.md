---
title: schemaExtension を取得する
description: 指定された schemaExtension 定義のプロパティを取得します。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: e95590361e4afa94f2d462c3b5f35a71a8010b9d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457514"
---
# <a name="get-schemaextension"></a><span data-ttu-id="b0ac9-103">schemaExtension を取得する</span><span class="sxs-lookup"><span data-stu-id="b0ac9-103">Get schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0ac9-104">指定された[Schemaextension](../resources/schemaextension.md)定義のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="b0ac9-104">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0ac9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0ac9-105">Permissions</span></span>
<span data-ttu-id="b0ac9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0ac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b0ac9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0ac9-108">Permission type</span></span>      | <span data-ttu-id="b0ac9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0ac9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0ac9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0ac9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0ac9-111">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b0ac9-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0ac9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0ac9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0ac9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0ac9-113">Not supported.</span></span>    |
|<span data-ttu-id="b0ac9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0ac9-114">Application</span></span> | <span data-ttu-id="b0ac9-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0ac9-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0ac9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0ac9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0ac9-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b0ac9-117">Optional query parameters</span></span>
<span data-ttu-id="b0ac9-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b0ac9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0ac9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0ac9-119">Request headers</span></span>
| <span data-ttu-id="b0ac9-120">名前</span><span class="sxs-lookup"><span data-stu-id="b0ac9-120">Name</span></span>      |<span data-ttu-id="b0ac9-121">説明</span><span class="sxs-lookup"><span data-stu-id="b0ac9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0ac9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0ac9-122">Authorization</span></span>  | <span data-ttu-id="b0ac9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0ac9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0ac9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0ac9-125">Content-Type</span></span>   | <span data-ttu-id="b0ac9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0ac9-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0ac9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0ac9-127">Request body</span></span>
<span data-ttu-id="b0ac9-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b0ac9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0ac9-129">応答</span><span class="sxs-lookup"><span data-stu-id="b0ac9-129">Response</span></span>

<span data-ttu-id="b0ac9-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[schemaextension](../resources/schemaextension.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b0ac9-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0ac9-131">例</span><span class="sxs-lookup"><span data-stu-id="b0ac9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0ac9-132">要求</span><span class="sxs-lookup"><span data-stu-id="b0ac9-132">Request</span></span>
<span data-ttu-id="b0ac9-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0ac9-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0ac9-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b0ac9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0ac9-135">C#</span><span class="sxs-lookup"><span data-stu-id="b0ac9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0ac9-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0ac9-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0ac9-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="b0ac9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0ac9-138">応答</span><span class="sxs-lookup"><span data-stu-id="b0ac9-138">Response</span></span>
<span data-ttu-id="b0ac9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b0ac9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id":"graphlearn_test",
    "description": "Yet another test schema",
    "targetTypes": [
        "User", "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "testName",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="b0ac9-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0ac9-142">See also</span></span>

- [<span data-ttu-id="b0ac9-143">拡張機能を使用したリソースへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="b0ac9-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b0ac9-144">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="b0ac9-144">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
