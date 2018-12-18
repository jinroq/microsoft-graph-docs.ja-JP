---
title: TableColumn を作成する
description: この API を使用して、新しい TableColumn を作成します。
author: lumine2008
ms.openlocfilehash: 8dd2ce889fcd5d6677ca3aeef2f8c544325bdbac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305370"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="75fc9-103">TableColumn を作成する</span><span class="sxs-lookup"><span data-stu-id="75fc9-103">Create TableColumn</span></span>

> <span data-ttu-id="75fc9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="75fc9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75fc9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75fc9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75fc9-106">この API を使用して、新しい TableColumn を作成します。</span><span class="sxs-lookup"><span data-stu-id="75fc9-106">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="75fc9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="75fc9-107">Permissions</span></span>
<span data-ttu-id="75fc9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75fc9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75fc9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75fc9-110">Permission type</span></span>      | <span data-ttu-id="75fc9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="75fc9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75fc9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75fc9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75fc9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75fc9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75fc9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75fc9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75fc9-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75fc9-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75fc9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75fc9-116">Application</span></span> | <span data-ttu-id="75fc9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75fc9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75fc9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75fc9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="75fc9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75fc9-119">Request headers</span></span>
| <span data-ttu-id="75fc9-120">名前</span><span class="sxs-lookup"><span data-stu-id="75fc9-120">Name</span></span>       | <span data-ttu-id="75fc9-121">説明</span><span class="sxs-lookup"><span data-stu-id="75fc9-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75fc9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75fc9-122">Authorization</span></span>  | <span data-ttu-id="75fc9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="75fc9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75fc9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="75fc9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="75fc9-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="75fc9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75fc9-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="75fc9-128">Request body</span></span>
<span data-ttu-id="75fc9-129">要求本文で、[TableColumn](../resources/tablecolumn.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="75fc9-129">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="75fc9-130">応答</span><span class="sxs-lookup"><span data-stu-id="75fc9-130">Response</span></span>

<span data-ttu-id="75fc9-131">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [TableColumn](../resources/tablecolumn.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="75fc9-131">If successful, this method returns `201 Created` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75fc9-132">例</span><span class="sxs-lookup"><span data-stu-id="75fc9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75fc9-133">要求</span><span class="sxs-lookup"><span data-stu-id="75fc9-133">Request</span></span>
<span data-ttu-id="75fc9-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="75fc9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="75fc9-135">要求本文で、[TableColumn](../resources/tablecolumn.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="75fc9-135">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="75fc9-136">応答</span><span class="sxs-lookup"><span data-stu-id="75fc9-136">Response</span></span>
<span data-ttu-id="75fc9-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="75fc9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
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