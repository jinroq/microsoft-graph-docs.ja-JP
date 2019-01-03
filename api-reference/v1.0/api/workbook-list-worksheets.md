---
title: ワークシートを一覧表示する
description: ワークシート オブジェクトの一覧を取得します。
author: lumine2008
ms.openlocfilehash: 9aee30c0cebae535b6a588ac24344e1fb6e17e7d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340391"
---
# <a name="list-worksheets"></a><span data-ttu-id="09694-103">ワークシートを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="09694-103">List worksheets</span></span>

<span data-ttu-id="09694-104">ワークシート オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="09694-104">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="09694-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="09694-105">Permissions</span></span>
<span data-ttu-id="09694-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09694-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09694-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09694-108">Permission type</span></span>      | <span data-ttu-id="09694-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="09694-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09694-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09694-110">Delegated (work or school account)</span></span> | <span data-ttu-id="09694-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09694-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="09694-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09694-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09694-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09694-113">Not supported.</span></span>    |
|<span data-ttu-id="09694-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09694-114">Application</span></span> | <span data-ttu-id="09694-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09694-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09694-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09694-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="09694-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="09694-117">Optional query parameters</span></span>
<span data-ttu-id="09694-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="09694-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09694-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09694-119">Request headers</span></span>
| <span data-ttu-id="09694-120">名前</span><span class="sxs-lookup"><span data-stu-id="09694-120">Name</span></span>      |<span data-ttu-id="09694-121">説明</span><span class="sxs-lookup"><span data-stu-id="09694-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09694-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09694-122">Authorization</span></span>  | <span data-ttu-id="09694-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="09694-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09694-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="09694-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="09694-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="09694-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09694-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="09694-128">Request body</span></span>
<span data-ttu-id="09694-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="09694-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09694-130">応答</span><span class="sxs-lookup"><span data-stu-id="09694-130">Response</span></span>

<span data-ttu-id="09694-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[WorkbookWorksheet](../resources/worksheet.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="09694-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09694-132">例</span><span class="sxs-lookup"><span data-stu-id="09694-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09694-133">要求</span><span class="sxs-lookup"><span data-stu-id="09694-133">Request</span></span>
<span data-ttu-id="09694-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09694-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheets"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="09694-135">応答</span><span class="sxs-lookup"><span data-stu-id="09694-135">Response</span></span>
<span data-ttu-id="09694-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="09694-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List worksheets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->