---
title: ワークシートを更新する
description: ワークシート オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e2139e1e350ab4c0f416e48181398011666274b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942032"
---
# <a name="update-worksheet"></a><span data-ttu-id="0ea5b-103">ワークシートを更新する</span><span class="sxs-lookup"><span data-stu-id="0ea5b-103">Update worksheet</span></span>

> <span data-ttu-id="0ea5b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ea5b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ea5b-106">ワークシート オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-106">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ea5b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0ea5b-107">Permissions</span></span>
<span data-ttu-id="0ea5b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea5b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ea5b-110">Permission type</span></span>      | <span data-ttu-id="0ea5b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ea5b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ea5b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ea5b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0ea5b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ea5b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ea5b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ea5b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ea5b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ea5b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ea5b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ea5b-116">Application</span></span> | <span data-ttu-id="0ea5b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ea5b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ea5b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0ea5b-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ea5b-119">Optional request headers</span></span>
| <span data-ttu-id="0ea5b-120">名前</span><span class="sxs-lookup"><span data-stu-id="0ea5b-120">Name</span></span>       | <span data-ttu-id="0ea5b-121">説明</span><span class="sxs-lookup"><span data-stu-id="0ea5b-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0ea5b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea5b-122">Authorization</span></span>  | <span data-ttu-id="0ea5b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ea5b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0ea5b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ea5b-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ea5b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ea5b-128">Request body</span></span>
<span data-ttu-id="0ea5b-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0ea5b-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ea5b-132">Property</span></span>     | <span data-ttu-id="0ea5b-133">種類</span><span class="sxs-lookup"><span data-stu-id="0ea5b-133">Type</span></span>   |<span data-ttu-id="0ea5b-134">説明</span><span class="sxs-lookup"><span data-stu-id="0ea5b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ea5b-135">name</span><span class="sxs-lookup"><span data-stu-id="0ea5b-135">name</span></span>|<span data-ttu-id="0ea5b-136">文字列</span><span class="sxs-lookup"><span data-stu-id="0ea5b-136">string</span></span>|<span data-ttu-id="0ea5b-137">ワークシートの表示名。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-137">The display name of the worksheet.</span></span>|
|<span data-ttu-id="0ea5b-138">position</span><span class="sxs-lookup"><span data-stu-id="0ea5b-138">position</span></span>|<span data-ttu-id="0ea5b-139">int</span><span class="sxs-lookup"><span data-stu-id="0ea5b-139">int</span></span>|<span data-ttu-id="0ea5b-140">0 を起点とした、ブック内のワークシートの位置。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-140">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="0ea5b-141">visibility</span><span class="sxs-lookup"><span data-stu-id="0ea5b-141">visibility</span></span>|<span data-ttu-id="0ea5b-142">文字列</span><span class="sxs-lookup"><span data-stu-id="0ea5b-142">string</span></span>|<span data-ttu-id="0ea5b-p106">ワークシートの可視性。可能な値は、`Visible`、`Hidden`、`VeryHidden` です。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-p106">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="0ea5b-145">応答</span><span class="sxs-lookup"><span data-stu-id="0ea5b-145">Response</span></span>

<span data-ttu-id="0ea5b-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[ワークシート](../resources/worksheet.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-146">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ea5b-147">例</span><span class="sxs-lookup"><span data-stu-id="0ea5b-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ea5b-148">要求</span><span class="sxs-lookup"><span data-stu-id="0ea5b-148">Request</span></span>
<span data-ttu-id="0ea5b-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="0ea5b-150">応答</span><span class="sxs-lookup"><span data-stu-id="0ea5b-150">Response</span></span>
<span data-ttu-id="0ea5b-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ea5b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
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
