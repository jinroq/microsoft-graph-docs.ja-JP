---
title: ワークシートを更新する
description: ワークシート オブジェクトのプロパティを更新します。
author: lumine2008
ms.openlocfilehash: 249fb16fea3c7086411bfa9f11a2ea23926b4b5b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344080"
---
# <a name="update-worksheet"></a><span data-ttu-id="73bb7-103">ワークシートを更新する</span><span class="sxs-lookup"><span data-stu-id="73bb7-103">Update worksheet</span></span>

<span data-ttu-id="73bb7-104">ワークシート オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="73bb7-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="73bb7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73bb7-105">Permissions</span></span>
<span data-ttu-id="73bb7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73bb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73bb7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73bb7-108">Permission type</span></span>      | <span data-ttu-id="73bb7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="73bb7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73bb7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73bb7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73bb7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73bb7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="73bb7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73bb7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73bb7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73bb7-113">Not supported.</span></span>    |
|<span data-ttu-id="73bb7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73bb7-114">Application</span></span> | <span data-ttu-id="73bb7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73bb7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73bb7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73bb7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="73bb7-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73bb7-117">Optional request headers</span></span>
| <span data-ttu-id="73bb7-118">名前</span><span class="sxs-lookup"><span data-stu-id="73bb7-118">Name</span></span>       | <span data-ttu-id="73bb7-119">説明</span><span class="sxs-lookup"><span data-stu-id="73bb7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="73bb7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="73bb7-120">Authorization</span></span>  | <span data-ttu-id="73bb7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="73bb7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73bb7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="73bb7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="73bb7-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="73bb7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73bb7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="73bb7-126">Request body</span></span>
<span data-ttu-id="73bb7-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="73bb7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="73bb7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73bb7-130">Property</span></span>     | <span data-ttu-id="73bb7-131">種類</span><span class="sxs-lookup"><span data-stu-id="73bb7-131">Type</span></span>   |<span data-ttu-id="73bb7-132">説明</span><span class="sxs-lookup"><span data-stu-id="73bb7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73bb7-133">name</span><span class="sxs-lookup"><span data-stu-id="73bb7-133">name</span></span>|<span data-ttu-id="73bb7-134">文字列</span><span class="sxs-lookup"><span data-stu-id="73bb7-134">string</span></span>|<span data-ttu-id="73bb7-135">ワークシートの表示名。</span><span class="sxs-lookup"><span data-stu-id="73bb7-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="73bb7-136">position</span><span class="sxs-lookup"><span data-stu-id="73bb7-136">position</span></span>|<span data-ttu-id="73bb7-137">int</span><span class="sxs-lookup"><span data-stu-id="73bb7-137">int</span></span>|<span data-ttu-id="73bb7-138">0 を起点とした、ブック内のワークシートの位置。</span><span class="sxs-lookup"><span data-stu-id="73bb7-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="73bb7-139">visibility</span><span class="sxs-lookup"><span data-stu-id="73bb7-139">visibility</span></span>|<span data-ttu-id="73bb7-140">文字列</span><span class="sxs-lookup"><span data-stu-id="73bb7-140">string</span></span>|<span data-ttu-id="73bb7-141">ワークシートの可視性。</span><span class="sxs-lookup"><span data-stu-id="73bb7-141">The Visibility of the worksheet.</span></span> <span data-ttu-id="73bb7-142">可能な値: `Visible`、 `Hidden`、 `VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="73bb7-142">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="73bb7-143">応答</span><span class="sxs-lookup"><span data-stu-id="73bb7-143">Response</span></span>

<span data-ttu-id="73bb7-144">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[WorkbookWorksheet](../resources/worksheet.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="73bb7-144">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73bb7-145">例</span><span class="sxs-lookup"><span data-stu-id="73bb7-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73bb7-146">要求</span><span class="sxs-lookup"><span data-stu-id="73bb7-146">Request</span></span>
<span data-ttu-id="73bb7-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73bb7-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="73bb7-148">応答</span><span class="sxs-lookup"><span data-stu-id="73bb7-148">Response</span></span>
<span data-ttu-id="73bb7-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73bb7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->