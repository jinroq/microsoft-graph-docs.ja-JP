---
title: テーブルを更新する
description: table オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: df975d13ddc97c0c6b592d02d61a978c5a0db732
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520488"
---
# <a name="update-table"></a><span data-ttu-id="179be-103">テーブルを更新する</span><span class="sxs-lookup"><span data-stu-id="179be-103">Update table</span></span>

<span data-ttu-id="179be-104">table オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="179be-104">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="179be-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="179be-105">Permissions</span></span>
<span data-ttu-id="179be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="179be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="179be-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="179be-108">Permission type</span></span>      | <span data-ttu-id="179be-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="179be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="179be-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="179be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="179be-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="179be-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="179be-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="179be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="179be-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="179be-113">Not supported.</span></span>    |
|<span data-ttu-id="179be-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="179be-114">Application</span></span> | <span data-ttu-id="179be-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="179be-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="179be-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="179be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="179be-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="179be-117">Optional request headers</span></span>
| <span data-ttu-id="179be-118">名前</span><span class="sxs-lookup"><span data-stu-id="179be-118">Name</span></span>       | <span data-ttu-id="179be-119">説明</span><span class="sxs-lookup"><span data-stu-id="179be-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="179be-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="179be-120">Authorization</span></span>  | <span data-ttu-id="179be-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="179be-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="179be-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="179be-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="179be-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="179be-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="179be-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="179be-126">Request body</span></span>
<span data-ttu-id="179be-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="179be-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="179be-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="179be-130">Property</span></span>     | <span data-ttu-id="179be-131">型</span><span class="sxs-lookup"><span data-stu-id="179be-131">Type</span></span>   |<span data-ttu-id="179be-132">説明</span><span class="sxs-lookup"><span data-stu-id="179be-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="179be-133">name</span><span class="sxs-lookup"><span data-stu-id="179be-133">name</span></span>|<span data-ttu-id="179be-134">string</span><span class="sxs-lookup"><span data-stu-id="179be-134">string</span></span>|<span data-ttu-id="179be-135">テーブルの名前。</span><span class="sxs-lookup"><span data-stu-id="179be-135">Name of the table.</span></span>|
|<span data-ttu-id="179be-136">showHeaders</span><span class="sxs-lookup"><span data-stu-id="179be-136">showHeaders</span></span>|<span data-ttu-id="179be-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="179be-137">boolean</span></span>|<span data-ttu-id="179be-p105">ヘッダー行を表示するかどうかを示します。この値によって、ヘッダー行の表示または削除を設定できます。</span><span class="sxs-lookup"><span data-stu-id="179be-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="179be-140">showTotals</span><span class="sxs-lookup"><span data-stu-id="179be-140">showTotals</span></span>|<span data-ttu-id="179be-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="179be-141">boolean</span></span>|<span data-ttu-id="179be-p106">集計行を表示するかどうかを示します。この値によって、集計行の表示または削除を設定できます。</span><span class="sxs-lookup"><span data-stu-id="179be-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="179be-144">style</span><span class="sxs-lookup"><span data-stu-id="179be-144">style</span></span>|<span data-ttu-id="179be-145">string</span><span class="sxs-lookup"><span data-stu-id="179be-145">string</span></span>|<span data-ttu-id="179be-146">テーブル スタイルを表す定数値。</span><span class="sxs-lookup"><span data-stu-id="179be-146">Constant value that represents the Table style.</span></span> <span data-ttu-id="179be-147">使用可能な値: TableStyleLight1 から TableStyleLight21、TableStyleMedium1 から TableStyleMedium28、TableStyleStyleDark1 から TableStyleStyleDark11。</span><span class="sxs-lookup"><span data-stu-id="179be-147">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="179be-148">ブックに存在するカスタムのユーザー定義スタイルも指定できます。</span><span class="sxs-lookup"><span data-stu-id="179be-148">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="179be-149">応答</span><span class="sxs-lookup"><span data-stu-id="179be-149">Response</span></span>

<span data-ttu-id="179be-150">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[WorkbookTable](../resources/table.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="179be-150">If successful, this method returns a `200 OK` response code and updated [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="179be-151">例</span><span class="sxs-lookup"><span data-stu-id="179be-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="179be-152">要求</span><span class="sxs-lookup"><span data-stu-id="179be-152">Request</span></span>
<span data-ttu-id="179be-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="179be-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="179be-154">応答</span><span class="sxs-lookup"><span data-stu-id="179be-154">Response</span></span>
<span data-ttu-id="179be-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="179be-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
