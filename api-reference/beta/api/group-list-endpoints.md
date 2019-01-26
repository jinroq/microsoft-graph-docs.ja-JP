---
title: エンドポイントを一覧表示する
description: エンドポイント オブジェクトの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4f6d5d1fc8578f390dce0fece668a851c47032a7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575857"
---
# <a name="list-endpoints"></a><span data-ttu-id="26685-103">エンドポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="26685-103">List endpoints</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26685-104">[エンドポイント](../resources/endpoint.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="26685-104">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="26685-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="26685-105">Permissions</span></span>
<span data-ttu-id="26685-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26685-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26685-108">Permission type</span></span>      | <span data-ttu-id="26685-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="26685-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26685-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26685-110">Delegated (work or school account)</span></span> | <span data-ttu-id="26685-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26685-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="26685-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26685-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26685-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26685-113">Not supported.</span></span>    |
|<span data-ttu-id="26685-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26685-114">Application</span></span> | <span data-ttu-id="26685-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26685-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26685-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26685-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="26685-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="26685-117">Optional query parameters</span></span>
<span data-ttu-id="26685-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="26685-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26685-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26685-119">Request headers</span></span>
| <span data-ttu-id="26685-120">名前</span><span class="sxs-lookup"><span data-stu-id="26685-120">Name</span></span>      |<span data-ttu-id="26685-121">説明</span><span class="sxs-lookup"><span data-stu-id="26685-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="26685-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26685-122">Authorization</span></span>  | <span data-ttu-id="26685-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="26685-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="26685-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26685-125">Content-Type</span></span>   | <span data-ttu-id="26685-126">アプリケーションまたは Json</span><span class="sxs-lookup"><span data-stu-id="26685-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="26685-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="26685-127">Request body</span></span>
<span data-ttu-id="26685-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="26685-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26685-129">応答</span><span class="sxs-lookup"><span data-stu-id="26685-129">Response</span></span>

<span data-ttu-id="26685-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[エンドポイント](../resources/endpoint.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="26685-130">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26685-131">例</span><span class="sxs-lookup"><span data-stu-id="26685-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26685-132">要求</span><span class="sxs-lookup"><span data-stu-id="26685-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
##### <a name="response"></a><span data-ttu-id="26685-133">応答</span><span class="sxs-lookup"><span data-stu-id="26685-133">Response</span></span>
<span data-ttu-id="26685-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26685-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 261

{
  "value": [
    {
      "capability": "Conversations",
      "providerId": "{Yammer GUID}",
      "providerName": "Yammer",
      "uri": "uri-value",
      "providerResourceId": "Yammer.FeedURL",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-endpoints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
