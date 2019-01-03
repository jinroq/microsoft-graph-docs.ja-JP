---
title: 'WorksheetCollection: add'
description: 上に .activate()。
author: lumine2008
ms.openlocfilehash: 560a66c4beb589fbb736f0aa27784827740c0440
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363579"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="5ebcc-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="5ebcc-103">WorksheetCollection: add</span></span>

> <span data-ttu-id="5ebcc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ebcc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ebcc-p102">新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。新しく追加したワークシートをアクティブにする場合は、そのワークシートに対して ".activate() を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-p102">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ebcc-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ebcc-109">Permissions</span></span>
<span data-ttu-id="5ebcc-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ebcc-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ebcc-112">Permission type</span></span>      | <span data-ttu-id="5ebcc-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ebcc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ebcc-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ebcc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5ebcc-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ebcc-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ebcc-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ebcc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ebcc-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ebcc-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ebcc-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ebcc-118">Application</span></span> | <span data-ttu-id="5ebcc-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ebcc-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ebcc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="5ebcc-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ebcc-121">Request headers</span></span>
| <span data-ttu-id="5ebcc-122">名前</span><span class="sxs-lookup"><span data-stu-id="5ebcc-122">Name</span></span>       | <span data-ttu-id="5ebcc-123">説明</span><span class="sxs-lookup"><span data-stu-id="5ebcc-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5ebcc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ebcc-124">Authorization</span></span>  | <span data-ttu-id="5ebcc-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ebcc-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5ebcc-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="5ebcc-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ebcc-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ebcc-130">Request body</span></span>
<span data-ttu-id="5ebcc-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5ebcc-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ebcc-132">Parameter</span></span>    | <span data-ttu-id="5ebcc-133">種類</span><span class="sxs-lookup"><span data-stu-id="5ebcc-133">Type</span></span>   |<span data-ttu-id="5ebcc-134">説明</span><span class="sxs-lookup"><span data-stu-id="5ebcc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ebcc-135">name</span><span class="sxs-lookup"><span data-stu-id="5ebcc-135">name</span></span>|<span data-ttu-id="5ebcc-136">文字列</span><span class="sxs-lookup"><span data-stu-id="5ebcc-136">string</span></span>|<span data-ttu-id="5ebcc-p106">省略可能。追加するワークシートの名前。指定する場合、名前は一意である必要があります。指定されていない場合は、Excel が新しいワークシートの名前を決定します。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-p106">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="5ebcc-141">応答</span><span class="sxs-lookup"><span data-stu-id="5ebcc-141">Response</span></span>

<span data-ttu-id="5ebcc-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ワークシート](../resources/worksheet.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-142">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ebcc-143">例</span><span class="sxs-lookup"><span data-stu-id="5ebcc-143">Example</span></span>
<span data-ttu-id="5ebcc-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5ebcc-145">要求</span><span class="sxs-lookup"><span data-stu-id="5ebcc-145">Request</span></span>
<span data-ttu-id="5ebcc-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="5ebcc-147">応答</span><span class="sxs-lookup"><span data-stu-id="5ebcc-147">Response</span></span>
<span data-ttu-id="5ebcc-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5ebcc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->