---
title: 'TableColumnCollection: ItemAt'
description: コレクション内の位置に基づいて列を取得します。
ms.openlocfilehash: 2fc8950b08c378a8f1610699b1819fb4bc1bc7fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069343"
---
# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="f9b48-103">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="f9b48-103">TableColumnCollection: ItemAt</span></span>

> <span data-ttu-id="f9b48-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f9b48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9b48-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9b48-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9b48-106">コレクション内の位置に基づいて列を取得します。</span><span class="sxs-lookup"><span data-stu-id="f9b48-106">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9b48-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f9b48-107">Permissions</span></span>
<span data-ttu-id="f9b48-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9b48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9b48-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9b48-110">Permission type</span></span>      | <span data-ttu-id="f9b48-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9b48-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9b48-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9b48-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9b48-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9b48-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9b48-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9b48-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9b48-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9b48-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9b48-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9b48-116">Application</span></span> | <span data-ttu-id="f9b48-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9b48-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9b48-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9b48-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="f9b48-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9b48-119">Request headers</span></span>
| <span data-ttu-id="f9b48-120">名前</span><span class="sxs-lookup"><span data-stu-id="f9b48-120">Name</span></span>       | <span data-ttu-id="f9b48-121">説明</span><span class="sxs-lookup"><span data-stu-id="f9b48-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f9b48-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9b48-122">Authorization</span></span>  | <span data-ttu-id="f9b48-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f9b48-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9b48-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f9b48-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f9b48-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f9b48-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9b48-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9b48-128">Request body</span></span>
<span data-ttu-id="f9b48-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f9b48-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f9b48-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f9b48-130">Parameter</span></span>    | <span data-ttu-id="f9b48-131">型</span><span class="sxs-lookup"><span data-stu-id="f9b48-131">Type</span></span>   |<span data-ttu-id="f9b48-132">説明</span><span class="sxs-lookup"><span data-stu-id="f9b48-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9b48-133">index</span><span class="sxs-lookup"><span data-stu-id="f9b48-133">index</span></span>|<span data-ttu-id="f9b48-134">数値</span><span class="sxs-lookup"><span data-stu-id="f9b48-134">number</span></span>|<span data-ttu-id="f9b48-p105">取得するオブジェクトのインデックス値。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="f9b48-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="f9b48-137">応答</span><span class="sxs-lookup"><span data-stu-id="f9b48-137">Response</span></span>

<span data-ttu-id="f9b48-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableColumn](../resources/tablecolumn.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f9b48-138">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9b48-139">例</span><span class="sxs-lookup"><span data-stu-id="f9b48-139">Example</span></span>
<span data-ttu-id="f9b48-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f9b48-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f9b48-141">要求</span><span class="sxs-lookup"><span data-stu-id="f9b48-141">Request</span></span>
<span data-ttu-id="f9b48-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f9b48-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="f9b48-143">応答</span><span class="sxs-lookup"><span data-stu-id="f9b48-143">Response</span></span>
<span data-ttu-id="f9b48-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f9b48-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->