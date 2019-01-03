---
title: TableRow を取得する　
description: tablerow オブジェクトのプロパティと関係を取得します。
author: lumine2008
ms.openlocfilehash: 472906f105a4f43de938e903c43b73adf6cb8045
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329366"
---
# <a name="get-tablerow"></a><span data-ttu-id="f067c-103">TableRow を取得する　</span><span class="sxs-lookup"><span data-stu-id="f067c-103">Get TableRow</span></span>

> <span data-ttu-id="f067c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f067c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f067c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f067c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f067c-106">tablerow オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="f067c-106">Retrieve the properties and relationships of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f067c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f067c-107">Permissions</span></span>
<span data-ttu-id="f067c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f067c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f067c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f067c-110">Permission type</span></span>      | <span data-ttu-id="f067c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f067c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f067c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f067c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f067c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f067c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f067c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f067c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f067c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f067c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f067c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f067c-116">Application</span></span> | <span data-ttu-id="f067c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f067c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f067c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f067c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows(<index>)
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f067c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f067c-119">Optional query parameters</span></span>
<span data-ttu-id="f067c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f067c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f067c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f067c-121">Request headers</span></span>
| <span data-ttu-id="f067c-122">名前</span><span class="sxs-lookup"><span data-stu-id="f067c-122">Name</span></span>      |<span data-ttu-id="f067c-123">説明</span><span class="sxs-lookup"><span data-stu-id="f067c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f067c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f067c-124">Authorization</span></span>  | <span data-ttu-id="f067c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f067c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f067c-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f067c-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="f067c-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f067c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f067c-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="f067c-130">Request body</span></span>
<span data-ttu-id="f067c-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f067c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f067c-132">応答</span><span class="sxs-lookup"><span data-stu-id="f067c-132">Response</span></span>

<span data-ttu-id="f067c-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableRow](../resources/tablerow.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f067c-133">If successful, this method returns a `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f067c-134">例</span><span class="sxs-lookup"><span data-stu-id="f067c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f067c-135">要求</span><span class="sxs-lookup"><span data-stu-id="f067c-135">Request</span></span>
<span data-ttu-id="f067c-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f067c-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablerow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
```
##### <a name="response"></a><span data-ttu-id="f067c-137">応答</span><span class="sxs-lookup"><span data-stu-id="f067c-137">Response</span></span>
<span data-ttu-id="f067c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f067c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->