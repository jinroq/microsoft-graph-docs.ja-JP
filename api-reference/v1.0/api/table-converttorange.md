---
title: 'Table: convertToRange'
description: テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2cda7e4eac082938cafb8328063658071eeb01d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560852"
---
# <a name="table-converttorange"></a><span data-ttu-id="af312-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="af312-104">Table: convertToRange</span></span>

<span data-ttu-id="af312-p102">テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。</span><span class="sxs-lookup"><span data-stu-id="af312-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="af312-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="af312-107">Permissions</span></span>
<span data-ttu-id="af312-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af312-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af312-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af312-110">Permission type</span></span>      | <span data-ttu-id="af312-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="af312-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af312-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af312-112">Delegated (work or school account)</span></span> | <span data-ttu-id="af312-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af312-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="af312-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af312-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af312-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af312-115">Not supported.</span></span>    |
|<span data-ttu-id="af312-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af312-116">Application</span></span> | <span data-ttu-id="af312-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af312-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af312-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af312-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="af312-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af312-119">Request headers</span></span>
| <span data-ttu-id="af312-120">名前</span><span class="sxs-lookup"><span data-stu-id="af312-120">Name</span></span>       | <span data-ttu-id="af312-121">説明</span><span class="sxs-lookup"><span data-stu-id="af312-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="af312-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af312-122">Authorization</span></span>  | <span data-ttu-id="af312-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="af312-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af312-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="af312-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="af312-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="af312-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af312-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="af312-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="af312-129">応答</span><span class="sxs-lookup"><span data-stu-id="af312-129">Response</span></span>

<span data-ttu-id="af312-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="af312-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af312-131">例</span><span class="sxs-lookup"><span data-stu-id="af312-131">Example</span></span>
<span data-ttu-id="af312-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="af312-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="af312-133">要求</span><span class="sxs-lookup"><span data-stu-id="af312-133">Request</span></span>
<span data-ttu-id="af312-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af312-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="af312-135">応答</span><span class="sxs-lookup"><span data-stu-id="af312-135">Response</span></span>
<span data-ttu-id="af312-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="af312-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
