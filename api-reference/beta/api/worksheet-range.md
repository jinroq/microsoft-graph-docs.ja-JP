---
title: ワークシート:Range
description: アドレスまたは名前で指定された範囲オブジェクトを取得します。
ms.openlocfilehash: defe05f953d5fe7cd5fafda6ae16f04bb9f91e86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071076"
---
# <a name="worksheet-range"></a><span data-ttu-id="82b8b-103">ワークシート:Range</span><span class="sxs-lookup"><span data-stu-id="82b8b-103">Worksheet: Range</span></span>

> <span data-ttu-id="82b8b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="82b8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82b8b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82b8b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82b8b-106">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="82b8b-106">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="82b8b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="82b8b-107">Permissions</span></span>
<span data-ttu-id="82b8b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82b8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82b8b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82b8b-110">Permission type</span></span>      | <span data-ttu-id="82b8b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="82b8b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82b8b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82b8b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="82b8b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82b8b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="82b8b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82b8b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82b8b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82b8b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="82b8b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82b8b-116">Application</span></span> | <span data-ttu-id="82b8b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82b8b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82b8b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82b8b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="82b8b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82b8b-119">Request headers</span></span>
| <span data-ttu-id="82b8b-120">名前</span><span class="sxs-lookup"><span data-stu-id="82b8b-120">Name</span></span>       | <span data-ttu-id="82b8b-121">説明</span><span class="sxs-lookup"><span data-stu-id="82b8b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="82b8b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82b8b-122">Authorization</span></span>  | <span data-ttu-id="82b8b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="82b8b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82b8b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="82b8b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="82b8b-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="82b8b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82b8b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="82b8b-128">Request body</span></span>
<span data-ttu-id="82b8b-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="82b8b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="82b8b-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="82b8b-130">Parameter</span></span>    | <span data-ttu-id="82b8b-131">型</span><span class="sxs-lookup"><span data-stu-id="82b8b-131">Type</span></span>   |<span data-ttu-id="82b8b-132">説明</span><span class="sxs-lookup"><span data-stu-id="82b8b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82b8b-133">address</span><span class="sxs-lookup"><span data-stu-id="82b8b-133">address</span></span>|<span data-ttu-id="82b8b-134">文字列</span><span class="sxs-lookup"><span data-stu-id="82b8b-134">string</span></span>|<span data-ttu-id="82b8b-p105">省略可能。範囲のアドレスまたは名前。指定されていない場合は、ワークシート全体の範囲が返されます。</span><span class="sxs-lookup"><span data-stu-id="82b8b-p105">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="82b8b-138">応答</span><span class="sxs-lookup"><span data-stu-id="82b8b-138">Response</span></span>

<span data-ttu-id="82b8b-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="82b8b-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82b8b-140">例</span><span class="sxs-lookup"><span data-stu-id="82b8b-140">Example</span></span>
<span data-ttu-id="82b8b-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="82b8b-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="82b8b-142">要求</span><span class="sxs-lookup"><span data-stu-id="82b8b-142">Request</span></span>
<span data-ttu-id="82b8b-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82b8b-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="82b8b-144">応答</span><span class="sxs-lookup"><span data-stu-id="82b8b-144">Response</span></span>
<span data-ttu-id="82b8b-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82b8b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->