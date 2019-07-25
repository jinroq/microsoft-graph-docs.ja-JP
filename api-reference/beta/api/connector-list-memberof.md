---
title: memberOf を一覧表示する
description: コネクタがメンバーであるコネクタグループを取得します。
localization_priority: Normal
ms.openlocfilehash: 28051e687d65beaea3962e2f4befce9f9c9d8f25
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863408"
---
# <a name="list-memberof"></a><span data-ttu-id="1acf4-103">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1acf4-103">List memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1acf4-104">コネクタがメンバーであるコネクタグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="1acf4-104">Retrieve the connectorgroup the connector is a member of.</span></span>
## <a name="permissions"></a><span data-ttu-id="1acf4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1acf4-105">Permissions</span></span>
<span data-ttu-id="1acf4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1acf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1acf4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1acf4-108">Permission type</span></span>      | <span data-ttu-id="1acf4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1acf4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1acf4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1acf4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1acf4-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1acf4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1acf4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1acf4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1acf4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1acf4-113">Not supported.</span></span>    |
|<span data-ttu-id="1acf4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1acf4-114">Application</span></span> | <span data-ttu-id="1acf4-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1acf4-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1acf4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1acf4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1acf4-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1acf4-117">Optional query parameters</span></span>
<span data-ttu-id="1acf4-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1acf4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1acf4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1acf4-119">Request headers</span></span>
| <span data-ttu-id="1acf4-120">名前</span><span class="sxs-lookup"><span data-stu-id="1acf4-120">Name</span></span>      |<span data-ttu-id="1acf4-121">説明</span><span class="sxs-lookup"><span data-stu-id="1acf4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1acf4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1acf4-122">Authorization</span></span>  | <span data-ttu-id="1acf4-123">ベアラー.</span><span class="sxs-lookup"><span data-stu-id="1acf4-123">Bearer.</span></span> <span data-ttu-id="1acf4-124">必須</span><span class="sxs-lookup"><span data-stu-id="1acf4-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="1acf4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1acf4-125">Request body</span></span>
<span data-ttu-id="1acf4-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1acf4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1acf4-127">応答</span><span class="sxs-lookup"><span data-stu-id="1acf4-127">Response</span></span>

<span data-ttu-id="1acf4-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[コネクタグループ](../resources/connectorgroup.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1acf4-128">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1acf4-129">例</span><span class="sxs-lookup"><span data-stu-id="1acf4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1acf4-130">要求</span><span class="sxs-lookup"><span data-stu-id="1acf4-130">Request</span></span>
<span data-ttu-id="1acf4-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1acf4-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "connector_get_memberof"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="1acf4-132">応答</span><span class="sxs-lookup"><span data-stu-id="1acf4-132">Response</span></span>
<span data-ttu-id="1acf4-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1acf4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
