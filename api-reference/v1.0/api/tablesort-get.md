---
title: TableSort を取得する　
description: tablesort オブジェクトのプロパティと関係を取得します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 01cb4f6eaca0463d2fdc96c3dcefffdb9d6a0842
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861427"
---
# <a name="get-tablesort"></a><span data-ttu-id="90d23-103">TableSort を取得する　</span><span class="sxs-lookup"><span data-stu-id="90d23-103">Get TableSort</span></span>

<span data-ttu-id="90d23-104">tablesort オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="90d23-104">Retrieve the properties and relationships of tablesort object.</span></span>
## <a name="permissions"></a><span data-ttu-id="90d23-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="90d23-105">Permissions</span></span>
<span data-ttu-id="90d23-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90d23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90d23-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90d23-108">Permission type</span></span>      | <span data-ttu-id="90d23-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="90d23-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90d23-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90d23-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90d23-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90d23-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90d23-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90d23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90d23-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90d23-113">Not supported.</span></span>    |
|<span data-ttu-id="90d23-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90d23-114">Application</span></span> | <span data-ttu-id="90d23-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90d23-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90d23-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90d23-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort
```
## <a name="optional-query-parameters"></a><span data-ttu-id="90d23-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="90d23-117">Optional query parameters</span></span>
<span data-ttu-id="90d23-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="90d23-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90d23-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90d23-119">Request headers</span></span>
| <span data-ttu-id="90d23-120">名前</span><span class="sxs-lookup"><span data-stu-id="90d23-120">Name</span></span>      |<span data-ttu-id="90d23-121">説明</span><span class="sxs-lookup"><span data-stu-id="90d23-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90d23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90d23-122">Authorization</span></span>  | <span data-ttu-id="90d23-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="90d23-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90d23-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="90d23-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="90d23-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="90d23-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90d23-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="90d23-128">Request body</span></span>
<span data-ttu-id="90d23-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="90d23-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90d23-130">応答</span><span class="sxs-lookup"><span data-stu-id="90d23-130">Response</span></span>

<span data-ttu-id="90d23-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[WorkbookTableSort](../resources/tablesort.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="90d23-131">If successful, this method returns a `200 OK` response code and [WorkbookTableSort](../resources/tablesort.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="90d23-132">例</span><span class="sxs-lookup"><span data-stu-id="90d23-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90d23-133">要求</span><span class="sxs-lookup"><span data-stu-id="90d23-133">Request</span></span>
<span data-ttu-id="90d23-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="90d23-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablesort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort
```
##### <a name="response"></a><span data-ttu-id="90d23-135">応答</span><span class="sxs-lookup"><span data-stu-id="90d23-135">Response</span></span>
<span data-ttu-id="90d23-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="90d23-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableSort"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "matchCase": true,
  "method": "method-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TableSort",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
