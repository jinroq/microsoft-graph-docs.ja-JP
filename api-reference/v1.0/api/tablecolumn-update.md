---
title: tablecolumn を更新する
description: tablecolumn オブジェクトのプロパティを更新します。
author: lumine2008
ms.openlocfilehash: b33c25deea629fceb18a5c5b00fa91e932ce98cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353733"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="675ba-103">tablecolumn を更新する</span><span class="sxs-lookup"><span data-stu-id="675ba-103">Update tablecolumn</span></span>

<span data-ttu-id="675ba-104">tablecolumn オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="675ba-104">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="675ba-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="675ba-105">Permissions</span></span>
<span data-ttu-id="675ba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="675ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="675ba-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="675ba-108">Permission type</span></span>      | <span data-ttu-id="675ba-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="675ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="675ba-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="675ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="675ba-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="675ba-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="675ba-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="675ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="675ba-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="675ba-113">Not supported.</span></span>    |
|<span data-ttu-id="675ba-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="675ba-114">Application</span></span> | <span data-ttu-id="675ba-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="675ba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="675ba-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="675ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="675ba-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="675ba-117">Optional request headers</span></span>
| <span data-ttu-id="675ba-118">名前</span><span class="sxs-lookup"><span data-stu-id="675ba-118">Name</span></span>       | <span data-ttu-id="675ba-119">説明</span><span class="sxs-lookup"><span data-stu-id="675ba-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="675ba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="675ba-120">Authorization</span></span>  | <span data-ttu-id="675ba-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="675ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="675ba-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="675ba-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="675ba-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="675ba-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="675ba-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="675ba-126">Request body</span></span>
<span data-ttu-id="675ba-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="675ba-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="675ba-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="675ba-130">Property</span></span>     | <span data-ttu-id="675ba-131">種類</span><span class="sxs-lookup"><span data-stu-id="675ba-131">Type</span></span>   |<span data-ttu-id="675ba-132">説明</span><span class="sxs-lookup"><span data-stu-id="675ba-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="675ba-133">values</span><span class="sxs-lookup"><span data-stu-id="675ba-133">values</span></span>|<span data-ttu-id="675ba-134">Json</span><span class="sxs-lookup"><span data-stu-id="675ba-134">Json</span></span>|<span data-ttu-id="675ba-p105">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="675ba-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="675ba-138">応答</span><span class="sxs-lookup"><span data-stu-id="675ba-138">Response</span></span>

<span data-ttu-id="675ba-139">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="675ba-139">If successful, this method returns a `200 OK` response code and updated [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="675ba-140">例</span><span class="sxs-lookup"><span data-stu-id="675ba-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="675ba-141">要求</span><span class="sxs-lookup"><span data-stu-id="675ba-141">Request</span></span>
<span data-ttu-id="675ba-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="675ba-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="675ba-143">応答</span><span class="sxs-lookup"><span data-stu-id="675ba-143">Response</span></span>
<span data-ttu-id="675ba-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="675ba-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
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
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->