---
title: schemaExtension を取得する
description: 指定された schemaExtension 定義のプロパティを取得します。
localization_priority: Normal
ms.openlocfilehash: 694dd29bb9ed997512cf389888f4b69fa9ad290c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810739"
---
# <a name="get-schemaextension"></a><span data-ttu-id="fa51f-103">schemaExtension を取得する</span><span class="sxs-lookup"><span data-stu-id="fa51f-103">Get schemaExtension</span></span>
<span data-ttu-id="fa51f-104">指定された [schemaExtension](../resources/schemaextension.md) 定義のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="fa51f-104">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa51f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fa51f-105">Permissions</span></span>
<span data-ttu-id="fa51f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa51f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fa51f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa51f-108">Permission type</span></span>      | <span data-ttu-id="fa51f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa51f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa51f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa51f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa51f-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa51f-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa51f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa51f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa51f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa51f-113">Not supported.</span></span>    |
|<span data-ttu-id="fa51f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa51f-114">Application</span></span> | <span data-ttu-id="fa51f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa51f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa51f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa51f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa51f-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fa51f-117">Optional query parameters</span></span>
<span data-ttu-id="fa51f-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fa51f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa51f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa51f-119">Request headers</span></span>
| <span data-ttu-id="fa51f-120">名前</span><span class="sxs-lookup"><span data-stu-id="fa51f-120">Name</span></span>      |<span data-ttu-id="fa51f-121">説明</span><span class="sxs-lookup"><span data-stu-id="fa51f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa51f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa51f-122">Authorization</span></span>  | <span data-ttu-id="fa51f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fa51f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa51f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa51f-125">Content-Type</span></span>   | <span data-ttu-id="fa51f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa51f-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa51f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa51f-127">Request body</span></span>
<span data-ttu-id="fa51f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fa51f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa51f-129">応答</span><span class="sxs-lookup"><span data-stu-id="fa51f-129">Response</span></span>

<span data-ttu-id="fa51f-130">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [schemaExtension](../resources/schemaextension.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fa51f-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa51f-131">例</span><span class="sxs-lookup"><span data-stu-id="fa51f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa51f-132">要求</span><span class="sxs-lookup"><span data-stu-id="fa51f-132">Request</span></span>
<span data-ttu-id="fa51f-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa51f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="fa51f-134">応答</span><span class="sxs-lookup"><span data-stu-id="fa51f-134">Response</span></span>
<span data-ttu-id="fa51f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa51f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
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

## <a name="see-also"></a><span data-ttu-id="fa51f-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="fa51f-138">See also</span></span>

- [<span data-ttu-id="fa51f-139">拡張機能を使用したリソースへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="fa51f-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fa51f-140">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="fa51f-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
