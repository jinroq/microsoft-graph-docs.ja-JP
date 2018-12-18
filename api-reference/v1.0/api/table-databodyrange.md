---
title: Table:DataBodyRange
description: テーブルのデータ本体に関連付けられた範囲オブジェクトを取得します。
author: lumine2008
ms.openlocfilehash: f36ec6ca005e529ac06e410bbbeb425db3096261
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326748"
---
# <a name="table-databodyrange"></a><span data-ttu-id="277c9-103">Table:DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="277c9-103">Table: DataBodyRange</span></span>

<span data-ttu-id="277c9-104">テーブルのデータ本体に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="277c9-104">Gets the range object associated with the data body of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="277c9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="277c9-105">Permissions</span></span>
<span data-ttu-id="277c9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="277c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="277c9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="277c9-108">Permission type</span></span>      | <span data-ttu-id="277c9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="277c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="277c9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="277c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="277c9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="277c9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="277c9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="277c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="277c9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="277c9-113">Not supported.</span></span>    |
|<span data-ttu-id="277c9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="277c9-114">Application</span></span> | <span data-ttu-id="277c9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="277c9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="277c9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="277c9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/dataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="277c9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="277c9-117">Request headers</span></span>
| <span data-ttu-id="277c9-118">名前</span><span class="sxs-lookup"><span data-stu-id="277c9-118">Name</span></span>       | <span data-ttu-id="277c9-119">説明</span><span class="sxs-lookup"><span data-stu-id="277c9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="277c9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="277c9-120">Authorization</span></span>  | <span data-ttu-id="277c9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="277c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="277c9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="277c9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="277c9-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="277c9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="277c9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="277c9-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="277c9-127">応答</span><span class="sxs-lookup"><span data-stu-id="277c9-127">Response</span></span>

<span data-ttu-id="277c9-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="277c9-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="277c9-129">例</span><span class="sxs-lookup"><span data-stu-id="277c9-129">Example</span></span>
<span data-ttu-id="277c9-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="277c9-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="277c9-131">要求</span><span class="sxs-lookup"><span data-stu-id="277c9-131">Request</span></span>
<span data-ttu-id="277c9-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="277c9-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_databodyrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/dataBodyRange
```

##### <a name="response"></a><span data-ttu-id="277c9-133">応答</span><span class="sxs-lookup"><span data-stu-id="277c9-133">Response</span></span>
<span data-ttu-id="277c9-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="277c9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->