---
title: RangeBorder を作成する
description: この API を使用して、新しい RangeBorder を作成します。
ms.openlocfilehash: 22a0e85a0e4e2ca6ad0a4fb2bdf503a01c892452
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021078"
---
# <a name="create-rangeborder"></a><span data-ttu-id="4e063-103">RangeBorder を作成する</span><span class="sxs-lookup"><span data-stu-id="4e063-103">Create RangeBorder</span></span>

<span data-ttu-id="4e063-104">この API を使用して、新しい RangeBorder を作成します。</span><span class="sxs-lookup"><span data-stu-id="4e063-104">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4e063-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4e063-105">Permissions</span></span>
<span data-ttu-id="4e063-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e063-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e063-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e063-108">Permission type</span></span>      | <span data-ttu-id="4e063-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e063-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e063-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e063-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4e063-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e063-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4e063-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e063-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e063-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e063-113">Not supported.</span></span>    |
|<span data-ttu-id="4e063-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e063-114">Application</span></span> | <span data-ttu-id="4e063-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e063-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e063-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e063-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="4e063-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e063-117">Request headers</span></span>
| <span data-ttu-id="4e063-118">名前</span><span class="sxs-lookup"><span data-stu-id="4e063-118">Name</span></span>       | <span data-ttu-id="4e063-119">説明</span><span class="sxs-lookup"><span data-stu-id="4e063-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4e063-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e063-120">Authorization</span></span>  | <span data-ttu-id="4e063-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4e063-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e063-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4e063-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4e063-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="4e063-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e063-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4e063-126">Request body</span></span>
<span data-ttu-id="4e063-127">要求の本文には、 [WorkbookRangeBorder](../resources/rangeborder.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e063-127">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4e063-128">応答</span><span class="sxs-lookup"><span data-stu-id="4e063-128">Response</span></span>

<span data-ttu-id="4e063-129">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[WorkbookRangeBorder](../resources/rangeborder.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4e063-129">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e063-130">例</span><span class="sxs-lookup"><span data-stu-id="4e063-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e063-131">要求</span><span class="sxs-lookup"><span data-stu-id="4e063-131">Request</span></span>
<span data-ttu-id="4e063-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4e063-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
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
<span data-ttu-id="4e063-133">要求の本文には、 [WorkbookRangeBorder](../resources/rangeborder.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e063-133">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4e063-134">応答</span><span class="sxs-lookup"><span data-stu-id="4e063-134">Response</span></span>
<span data-ttu-id="4e063-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4e063-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->