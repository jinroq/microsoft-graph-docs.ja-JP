---
title: 列を一覧表示する
description: tablecolumn オブジェクトのリストを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a3b9feeff30844a5ac5e4a30c8fd032c7de1b3d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536753"
---
# <a name="list-columns"></a><span data-ttu-id="d680f-103">列を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d680f-103">List columns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d680f-104">tablecolumn オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d680f-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d680f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d680f-105">Permissions</span></span>
<span data-ttu-id="d680f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d680f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d680f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d680f-108">Permission type</span></span>      | <span data-ttu-id="d680f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d680f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d680f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d680f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d680f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d680f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d680f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d680f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d680f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d680f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d680f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d680f-114">Application</span></span> | <span data-ttu-id="d680f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d680f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d680f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d680f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d680f-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d680f-117">Optional query parameters</span></span>
<span data-ttu-id="d680f-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d680f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="d680f-119">
  [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) クエリ パラメーターを使用して結果をページングすると、信頼性の高い結果を得られます。</span><span class="sxs-lookup"><span data-stu-id="d680f-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="d680f-120">こうして、大きな結果セットに関連するパフォーマンスの問題を回避できます。</span><span class="sxs-lookup"><span data-stu-id="d680f-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d680f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d680f-121">Request headers</span></span>
| <span data-ttu-id="d680f-122">名前</span><span class="sxs-lookup"><span data-stu-id="d680f-122">Name</span></span>      |<span data-ttu-id="d680f-123">説明</span><span class="sxs-lookup"><span data-stu-id="d680f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d680f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d680f-124">Authorization</span></span>  | <span data-ttu-id="d680f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d680f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d680f-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d680f-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="d680f-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="d680f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d680f-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="d680f-130">Request body</span></span>
<span data-ttu-id="d680f-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d680f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d680f-132">応答</span><span class="sxs-lookup"><span data-stu-id="d680f-132">Response</span></span>

<span data-ttu-id="d680f-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableColumn](../resources/tablecolumn.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d680f-133">If successful, this method returns a `200 OK` response code and collection of [TableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d680f-134">例</span><span class="sxs-lookup"><span data-stu-id="d680f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d680f-135">要求</span><span class="sxs-lookup"><span data-stu-id="d680f-135">Request</span></span>
<span data-ttu-id="d680f-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d680f-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="d680f-137">応答</span><span class="sxs-lookup"><span data-stu-id="d680f-137">Response</span></span>
<span data-ttu-id="d680f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d680f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="d680f-141">
  **注:\*\* [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) を使用して、多数の列をページングします。</span><span class="sxs-lookup"><span data-stu-id="d680f-141">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="d680f-142">例: </span><span class="sxs-lookup"><span data-stu-id="d680f-142">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-list-columns.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
