---
title: TableCollection の一覧表示
description: テーブル オブジェクトの一覧を取得します。
ms.openlocfilehash: 56864105d199b461b14e66543f683e1815b28021
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020849"
---
# <a name="list-tablecollection"></a><span data-ttu-id="fd70a-103">TableCollection の一覧表示</span><span class="sxs-lookup"><span data-stu-id="fd70a-103">List TableCollection</span></span>

<span data-ttu-id="fd70a-104">テーブル オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="fd70a-104">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="fd70a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd70a-105">Permissions</span></span>
<span data-ttu-id="fd70a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd70a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd70a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd70a-108">Permission type</span></span>      | <span data-ttu-id="fd70a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd70a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd70a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd70a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd70a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd70a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fd70a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd70a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd70a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd70a-113">Not supported.</span></span>    |
|<span data-ttu-id="fd70a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd70a-114">Application</span></span> | <span data-ttu-id="fd70a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd70a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd70a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd70a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables
GET /workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fd70a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fd70a-117">Optional query parameters</span></span>
<span data-ttu-id="fd70a-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fd70a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd70a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd70a-119">Request headers</span></span>
| <span data-ttu-id="fd70a-120">名前</span><span class="sxs-lookup"><span data-stu-id="fd70a-120">Name</span></span>      |<span data-ttu-id="fd70a-121">説明</span><span class="sxs-lookup"><span data-stu-id="fd70a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fd70a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd70a-122">Authorization</span></span>  | <span data-ttu-id="fd70a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fd70a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd70a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fd70a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="fd70a-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="fd70a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd70a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd70a-128">Request body</span></span>
<span data-ttu-id="fd70a-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fd70a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd70a-130">応答</span><span class="sxs-lookup"><span data-stu-id="fd70a-130">Response</span></span>

<span data-ttu-id="fd70a-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[WorkbookTable](../resources/table.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="fd70a-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTable](../resources/table.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd70a-132">例</span><span class="sxs-lookup"><span data-stu-id="fd70a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd70a-133">要求</span><span class="sxs-lookup"><span data-stu-id="fd70a-133">Request</span></span>
<span data-ttu-id="fd70a-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fd70a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables
```
##### <a name="response"></a><span data-ttu-id="fd70a-135">応答</span><span class="sxs-lookup"><span data-stu-id="fd70a-135">Response</span></span>
<span data-ttu-id="fd70a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fd70a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "showHeaders": true,
      "showTotals": true,
      "style": "style-value"
    }
  ]
}
```
> <span data-ttu-id="fd70a-139">**注:** [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターを使用して、多数のテーブルをページングします。</span><span class="sxs-lookup"><span data-stu-id="fd70a-139">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) query parameters to page through large numbers of tables.</span></span>

<span data-ttu-id="fd70a-140">例:</span><span class="sxs-lookup"><span data-stu-id="fd70a-140">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
