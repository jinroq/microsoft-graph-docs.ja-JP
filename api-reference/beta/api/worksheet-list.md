---
title: WorksheetCollection を一覧表示する
description: ワークシート オブジェクトの一覧を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0ef8c80d0924a04dfc968b87c0049e85578bcebb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970920"
---
# <a name="list-worksheetcollection"></a><span data-ttu-id="ed5f5-103">WorksheetCollection を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ed5f5-103">List WorksheetCollection</span></span>

> <span data-ttu-id="ed5f5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed5f5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed5f5-106">ワークシート オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-106">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ed5f5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed5f5-107">Permissions</span></span>
<span data-ttu-id="ed5f5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed5f5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed5f5-110">Permission type</span></span>      | <span data-ttu-id="ed5f5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed5f5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed5f5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed5f5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ed5f5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed5f5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ed5f5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed5f5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed5f5-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed5f5-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ed5f5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed5f5-116">Application</span></span> | <span data-ttu-id="ed5f5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed5f5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed5f5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ed5f5-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ed5f5-119">Optional query parameters</span></span>
<span data-ttu-id="ed5f5-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed5f5-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed5f5-121">Request headers</span></span>
| <span data-ttu-id="ed5f5-122">名前</span><span class="sxs-lookup"><span data-stu-id="ed5f5-122">Name</span></span>      |<span data-ttu-id="ed5f5-123">説明</span><span class="sxs-lookup"><span data-stu-id="ed5f5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ed5f5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed5f5-124">Authorization</span></span>  | <span data-ttu-id="ed5f5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed5f5-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ed5f5-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="ed5f5-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed5f5-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed5f5-130">Request body</span></span>
<span data-ttu-id="ed5f5-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed5f5-132">応答</span><span class="sxs-lookup"><span data-stu-id="ed5f5-132">Response</span></span>

<span data-ttu-id="ed5f5-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Worksheet](../resources/worksheet.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-133">If successful, this method returns a `200 OK` response code and collection of [Worksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed5f5-134">例</span><span class="sxs-lookup"><span data-stu-id="ed5f5-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed5f5-135">要求</span><span class="sxs-lookup"><span data-stu-id="ed5f5-135">Request</span></span>
<span data-ttu-id="ed5f5-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheetcollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="ed5f5-137">応答</span><span class="sxs-lookup"><span data-stu-id="ed5f5-137">Response</span></span>
<span data-ttu-id="ed5f5-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed5f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet",
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
  "description": "List WorksheetCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
