---
title: エンドポイントを取得する
description: 特定のエンドポイントオブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 7c5b7bd28b06e20dbc92b09ff961214828749999
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457469"
---
# <a name="get-endpoint"></a><span data-ttu-id="b5933-103">エンドポイントを取得する</span><span class="sxs-lookup"><span data-stu-id="b5933-103">Get endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5933-104">特定の[エンドポイント](../resources/endpoint.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="b5933-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5933-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b5933-105">Permissions</span></span>
<span data-ttu-id="b5933-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5933-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b5933-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b5933-108">Permission type</span></span>      | <span data-ttu-id="b5933-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b5933-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5933-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b5933-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5933-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5933-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5933-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5933-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5933-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5933-113">Not supported.</span></span>    |
|<span data-ttu-id="b5933-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b5933-114">Application</span></span> | <span data-ttu-id="b5933-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5933-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5933-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b5933-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5933-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b5933-117">Optional query parameters</span></span>
<span data-ttu-id="b5933-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b5933-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5933-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5933-119">Request headers</span></span>
| <span data-ttu-id="b5933-120">名前</span><span class="sxs-lookup"><span data-stu-id="b5933-120">Name</span></span>      |<span data-ttu-id="b5933-121">説明</span><span class="sxs-lookup"><span data-stu-id="b5933-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5933-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5933-122">Authorization</span></span>  | <span data-ttu-id="b5933-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b5933-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b5933-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5933-125">Content-Type</span></span>   | <span data-ttu-id="b5933-126">Application/Json</span><span class="sxs-lookup"><span data-stu-id="b5933-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5933-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b5933-127">Request body</span></span>
<span data-ttu-id="b5933-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b5933-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5933-129">応答</span><span class="sxs-lookup"><span data-stu-id="b5933-129">Response</span></span>

<span data-ttu-id="b5933-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[エンドポイント](../resources/endpoint.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b5933-130">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5933-131">例</span><span class="sxs-lookup"><span data-stu-id="b5933-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5933-132">要求</span><span class="sxs-lookup"><span data-stu-id="b5933-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
##### <a name="response"></a><span data-ttu-id="b5933-133">応答</span><span class="sxs-lookup"><span data-stu-id="b5933-133">Response</span></span>
<span data-ttu-id="b5933-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b5933-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/endpoint-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
