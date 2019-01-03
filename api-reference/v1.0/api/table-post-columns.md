---
title: TableColumn を作成する
description: この API を使用して、新しい TableColumn を作成します。
author: lumine2008
ms.openlocfilehash: 00cef446f6f7c75961bb081975af8f908bacc674
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339971"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="ea646-103">TableColumn を作成する</span><span class="sxs-lookup"><span data-stu-id="ea646-103">Create TableColumn</span></span>

<span data-ttu-id="ea646-104">この API を使用して、新しい TableColumn を作成します。</span><span class="sxs-lookup"><span data-stu-id="ea646-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea646-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ea646-105">Permissions</span></span>
<span data-ttu-id="ea646-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea646-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea646-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ea646-108">Permission type</span></span>      | <span data-ttu-id="ea646-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ea646-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea646-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ea646-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea646-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea646-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea646-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ea646-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea646-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea646-113">Not supported.</span></span>    |
|<span data-ttu-id="ea646-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ea646-114">Application</span></span> | <span data-ttu-id="ea646-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea646-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea646-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ea646-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="ea646-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ea646-117">Request headers</span></span>
| <span data-ttu-id="ea646-118">名前</span><span class="sxs-lookup"><span data-stu-id="ea646-118">Name</span></span>       | <span data-ttu-id="ea646-119">説明</span><span class="sxs-lookup"><span data-stu-id="ea646-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ea646-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea646-120">Authorization</span></span>  | <span data-ttu-id="ea646-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ea646-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea646-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ea646-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ea646-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ea646-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea646-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ea646-126">Request body</span></span>
<span data-ttu-id="ea646-127">要求の本文には、 [WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea646-127">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ea646-128">応答</span><span class="sxs-lookup"><span data-stu-id="ea646-128">Response</span></span>

<span data-ttu-id="ea646-129">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ea646-129">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea646-130">例</span><span class="sxs-lookup"><span data-stu-id="ea646-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea646-131">要求</span><span class="sxs-lookup"><span data-stu-id="ea646-131">Request</span></span>
<span data-ttu-id="ea646-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ea646-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="ea646-133">要求の本文には、 [WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea646-133">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ea646-134">応答</span><span class="sxs-lookup"><span data-stu-id="ea646-134">Response</span></span>
<span data-ttu-id="ea646-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ea646-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->