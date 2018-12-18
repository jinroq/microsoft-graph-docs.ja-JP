---
title: TableSort を取得する　
description: tablesort オブジェクトのプロパティと関係を取得します。
author: lumine2008
ms.openlocfilehash: 2968a0c5639acb84245db6c4816ce17cb8f0616f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325075"
---
# <a name="get-tablesort"></a><span data-ttu-id="94d81-103">TableSort を取得する　</span><span class="sxs-lookup"><span data-stu-id="94d81-103">Get TableSort</span></span>

> <span data-ttu-id="94d81-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="94d81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94d81-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94d81-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94d81-106">tablesort オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="94d81-106">Retrieve the properties and relationships of tablesort object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94d81-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94d81-107">Permissions</span></span>
<span data-ttu-id="94d81-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94d81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94d81-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94d81-110">Permission type</span></span>      | <span data-ttu-id="94d81-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94d81-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94d81-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94d81-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94d81-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94d81-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94d81-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94d81-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94d81-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94d81-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="94d81-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94d81-116">Application</span></span> | <span data-ttu-id="94d81-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94d81-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94d81-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94d81-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort
```
## <a name="optional-query-parameters"></a><span data-ttu-id="94d81-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="94d81-119">Optional query parameters</span></span>
<span data-ttu-id="94d81-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="94d81-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94d81-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94d81-121">Request headers</span></span>
| <span data-ttu-id="94d81-122">名前</span><span class="sxs-lookup"><span data-stu-id="94d81-122">Name</span></span>      |<span data-ttu-id="94d81-123">説明</span><span class="sxs-lookup"><span data-stu-id="94d81-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94d81-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="94d81-124">Authorization</span></span>  | <span data-ttu-id="94d81-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="94d81-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94d81-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="94d81-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="94d81-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="94d81-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94d81-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="94d81-130">Request body</span></span>
<span data-ttu-id="94d81-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="94d81-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94d81-132">応答</span><span class="sxs-lookup"><span data-stu-id="94d81-132">Response</span></span>

<span data-ttu-id="94d81-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableSort](../resources/tablesort.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="94d81-133">If successful, this method returns a `200 OK` response code and [TableSort](../resources/tablesort.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94d81-134">例</span><span class="sxs-lookup"><span data-stu-id="94d81-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94d81-135">要求</span><span class="sxs-lookup"><span data-stu-id="94d81-135">Request</span></span>
<span data-ttu-id="94d81-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94d81-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablesort"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort
```
##### <a name="response"></a><span data-ttu-id="94d81-137">応答</span><span class="sxs-lookup"><span data-stu-id="94d81-137">Response</span></span>
<span data-ttu-id="94d81-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94d81-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableSort"
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