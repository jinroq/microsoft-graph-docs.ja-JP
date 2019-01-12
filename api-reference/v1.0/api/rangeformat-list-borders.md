---
title: 境界線を一覧表示する
description: rangeborder オブジェクトのリストを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bfe977a90a43749e2a7b9faefea46c8b998eb65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986027"
---
# <a name="list-borders"></a><span data-ttu-id="6102a-103">境界線を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6102a-103">List borders</span></span>

<span data-ttu-id="6102a-104">rangeborder オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="6102a-104">Retrieve a list of rangeborder objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6102a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6102a-105">Permissions</span></span>
<span data-ttu-id="6102a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6102a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6102a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6102a-108">Permission type</span></span>      | <span data-ttu-id="6102a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6102a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6102a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6102a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6102a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6102a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6102a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6102a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6102a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6102a-113">Not supported.</span></span>    |
|<span data-ttu-id="6102a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6102a-114">Application</span></span> | <span data-ttu-id="6102a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6102a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6102a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6102a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6102a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6102a-117">Optional query parameters</span></span>
<span data-ttu-id="6102a-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6102a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6102a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6102a-119">Request headers</span></span>
| <span data-ttu-id="6102a-120">名前</span><span class="sxs-lookup"><span data-stu-id="6102a-120">Name</span></span>      |<span data-ttu-id="6102a-121">説明</span><span class="sxs-lookup"><span data-stu-id="6102a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6102a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6102a-122">Authorization</span></span>  | <span data-ttu-id="6102a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6102a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6102a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6102a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6102a-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="6102a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6102a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6102a-128">Request body</span></span>
<span data-ttu-id="6102a-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6102a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6102a-130">応答</span><span class="sxs-lookup"><span data-stu-id="6102a-130">Response</span></span>

<span data-ttu-id="6102a-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[WorkbookRangeBorder](../resources/rangeborder.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6102a-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookRangeBorder](../resources/rangeborder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6102a-132">例</span><span class="sxs-lookup"><span data-stu-id="6102a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6102a-133">要求</span><span class="sxs-lookup"><span data-stu-id="6102a-133">Request</span></span>
<span data-ttu-id="6102a-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6102a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_borders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
```
##### <a name="response"></a><span data-ttu-id="6102a-135">応答</span><span class="sxs-lookup"><span data-stu-id="6102a-135">Response</span></span>
<span data-ttu-id="6102a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6102a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 185

{
  "value": [
    {
      "id": "id-value",
      "color": "color-value",
      "style": "style-value",
      "sideIndex": "sideIndex-value",
      "weight": "weight-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List borders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
