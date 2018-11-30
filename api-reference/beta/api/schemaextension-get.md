---
title: schemaExtension を取得する
description: 指定された schemaExtension 定義のプロパティを取得します。
ms.openlocfilehash: 32376d6afd0d6171362db1978b708610d9f4d056
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072277"
---
# <a name="get-schemaextension"></a><span data-ttu-id="2b5e7-103">schemaExtension を取得する</span><span class="sxs-lookup"><span data-stu-id="2b5e7-103">Get schemaExtension</span></span>

> <span data-ttu-id="2b5e7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b5e7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b5e7-106">指定された [schemaExtension](../resources/schemaextension.md) 定義のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-106">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b5e7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b5e7-107">Permissions</span></span>
<span data-ttu-id="2b5e7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2b5e7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b5e7-110">Permission type</span></span>      | <span data-ttu-id="2b5e7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b5e7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b5e7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b5e7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b5e7-113">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2b5e7-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2b5e7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b5e7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b5e7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-115">Not supported.</span></span>    |
|<span data-ttu-id="2b5e7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b5e7-116">Application</span></span> | <span data-ttu-id="2b5e7-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b5e7-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b5e7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b5e7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2b5e7-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2b5e7-119">Optional query parameters</span></span>
<span data-ttu-id="2b5e7-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b5e7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b5e7-121">Request headers</span></span>
| <span data-ttu-id="2b5e7-122">名前</span><span class="sxs-lookup"><span data-stu-id="2b5e7-122">Name</span></span>      |<span data-ttu-id="2b5e7-123">説明</span><span class="sxs-lookup"><span data-stu-id="2b5e7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b5e7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b5e7-124">Authorization</span></span>  | <span data-ttu-id="2b5e7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b5e7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b5e7-127">Content-Type</span></span>   | <span data-ttu-id="2b5e7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2b5e7-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b5e7-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b5e7-129">Request body</span></span>
<span data-ttu-id="2b5e7-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b5e7-131">応答</span><span class="sxs-lookup"><span data-stu-id="2b5e7-131">Response</span></span>

<span data-ttu-id="2b5e7-132">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [schemaExtension](../resources/schemaextension.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-132">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b5e7-133">例</span><span class="sxs-lookup"><span data-stu-id="2b5e7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b5e7-134">要求</span><span class="sxs-lookup"><span data-stu-id="2b5e7-134">Request</span></span>
<span data-ttu-id="2b5e7-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="2b5e7-136">応答</span><span class="sxs-lookup"><span data-stu-id="2b5e7-136">Response</span></span>
<span data-ttu-id="2b5e7-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2b5e7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2b5e7-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="2b5e7-140">See also</span></span>

- [<span data-ttu-id="2b5e7-141">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="2b5e7-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2b5e7-142">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="2b5e7-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->