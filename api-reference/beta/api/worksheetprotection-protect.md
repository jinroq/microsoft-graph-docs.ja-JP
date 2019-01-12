---
title: 'WorksheetProtection: protect'
description: ワークシートを保護します。ワークシートが保護されている場合はスローします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d72d81b181c6e2fb82df991baaca7c12bb72c721
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930573"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="b88e6-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="b88e6-104">WorksheetProtection: protect</span></span>

> <span data-ttu-id="b88e6-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b88e6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b88e6-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b88e6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b88e6-p103">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="b88e6-p103">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="b88e6-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b88e6-109">Permissions</span></span>
<span data-ttu-id="b88e6-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b88e6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b88e6-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b88e6-112">Permission type</span></span>      | <span data-ttu-id="b88e6-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b88e6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b88e6-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b88e6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b88e6-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b88e6-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b88e6-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b88e6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b88e6-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b88e6-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b88e6-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b88e6-118">Application</span></span> | <span data-ttu-id="b88e6-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b88e6-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b88e6-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b88e6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="b88e6-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b88e6-121">Request headers</span></span>
| <span data-ttu-id="b88e6-122">名前</span><span class="sxs-lookup"><span data-stu-id="b88e6-122">Name</span></span>       | <span data-ttu-id="b88e6-123">説明</span><span class="sxs-lookup"><span data-stu-id="b88e6-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b88e6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b88e6-124">Authorization</span></span>  | <span data-ttu-id="b88e6-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b88e6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b88e6-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b88e6-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="b88e6-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b88e6-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b88e6-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="b88e6-130">Request body</span></span>
<span data-ttu-id="b88e6-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b88e6-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b88e6-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b88e6-132">Parameter</span></span>    | <span data-ttu-id="b88e6-133">Type</span><span class="sxs-lookup"><span data-stu-id="b88e6-133">Type</span></span>   |<span data-ttu-id="b88e6-134">説明</span><span class="sxs-lookup"><span data-stu-id="b88e6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b88e6-135">options</span><span class="sxs-lookup"><span data-stu-id="b88e6-135">options</span></span>|<span data-ttu-id="b88e6-136">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="b88e6-136">WorksheetProtectionOptions</span></span>|<span data-ttu-id="b88e6-p107">省略可能。シートの保護のオプション。</span><span class="sxs-lookup"><span data-stu-id="b88e6-p107">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="b88e6-139">応答</span><span class="sxs-lookup"><span data-stu-id="b88e6-139">Response</span></span>

<span data-ttu-id="b88e6-p108">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b88e6-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b88e6-142">例</span><span class="sxs-lookup"><span data-stu-id="b88e6-142">Example</span></span>
<span data-ttu-id="b88e6-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b88e6-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b88e6-144">要求</span><span class="sxs-lookup"><span data-stu-id="b88e6-144">Request</span></span>
<span data-ttu-id="b88e6-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b88e6-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="b88e6-146">応答</span><span class="sxs-lookup"><span data-stu-id="b88e6-146">Response</span></span>
<span data-ttu-id="b88e6-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b88e6-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
