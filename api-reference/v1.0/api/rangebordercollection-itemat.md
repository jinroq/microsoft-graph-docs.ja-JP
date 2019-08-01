---
title: 'RangeBorderCollection: ItemAt'
description: オブジェクトのインデックスを使用して、境界線オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 480ecdf8f9f22df0b5a29ac4736479900b35c53e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022132"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="20e21-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="20e21-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="20e21-104">オブジェクトのインデックスを使用して、境界線オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="20e21-104">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="20e21-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="20e21-105">Permissions</span></span>
<span data-ttu-id="20e21-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20e21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20e21-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20e21-108">Permission type</span></span>      | <span data-ttu-id="20e21-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="20e21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20e21-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20e21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="20e21-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20e21-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20e21-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20e21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20e21-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20e21-113">Not supported.</span></span>    |
|<span data-ttu-id="20e21-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20e21-114">Application</span></span> | <span data-ttu-id="20e21-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20e21-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20e21-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20e21-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20e21-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="20e21-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders/itemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/itemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="20e21-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20e21-118">Request headers</span></span>
| <span data-ttu-id="20e21-119">名前</span><span class="sxs-lookup"><span data-stu-id="20e21-119">Name</span></span>       | <span data-ttu-id="20e21-120">説明</span><span class="sxs-lookup"><span data-stu-id="20e21-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20e21-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="20e21-121">Authorization</span></span>  | <span data-ttu-id="20e21-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="20e21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20e21-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="20e21-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="20e21-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="20e21-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20e21-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="20e21-127">Request body</span></span>
<span data-ttu-id="20e21-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="20e21-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20e21-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="20e21-129">Parameter</span></span>    | <span data-ttu-id="20e21-130">型</span><span class="sxs-lookup"><span data-stu-id="20e21-130">Type</span></span>   |<span data-ttu-id="20e21-131">説明</span><span class="sxs-lookup"><span data-stu-id="20e21-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20e21-132">index</span><span class="sxs-lookup"><span data-stu-id="20e21-132">index</span></span>|<span data-ttu-id="20e21-133">Int32</span><span class="sxs-lookup"><span data-stu-id="20e21-133">Int32</span></span>|<span data-ttu-id="20e21-p104">取得するオブジェクトのインデックス値。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="20e21-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="20e21-136">応答</span><span class="sxs-lookup"><span data-stu-id="20e21-136">Response</span></span>

<span data-ttu-id="20e21-137">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[WorkbookRangeBorder](../resources/rangeborder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="20e21-137">If successful, this method returns `200 OK` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20e21-138">例</span><span class="sxs-lookup"><span data-stu-id="20e21-138">Example</span></span>
<span data-ttu-id="20e21-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="20e21-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="20e21-140">要求</span><span class="sxs-lookup"><span data-stu-id="20e21-140">Request</span></span>
<span data-ttu-id="20e21-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="20e21-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "rangebordercollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 1
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20e21-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="20e21-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangebordercollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20e21-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="20e21-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangebordercollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="20e21-144">応答</span><span class="sxs-lookup"><span data-stu-id="20e21-144">Response</span></span>
<span data-ttu-id="20e21-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="20e21-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
