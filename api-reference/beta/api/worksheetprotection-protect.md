---
title: 'WorksheetProtection: protect'
description: ワークシートを保護します。ワークシートが保護されている場合はスローします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 52c7b9a6d3437417e6b8d527d4625e64a9d91cc8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520131"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="d9322-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="d9322-104">WorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9322-p102">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="d9322-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9322-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d9322-107">Permissions</span></span>
<span data-ttu-id="d9322-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9322-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9322-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9322-110">Permission type</span></span>      | <span data-ttu-id="d9322-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9322-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9322-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9322-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9322-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9322-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9322-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9322-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9322-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9322-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9322-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9322-116">Application</span></span> | <span data-ttu-id="d9322-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9322-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9322-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9322-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="d9322-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9322-119">Request headers</span></span>
| <span data-ttu-id="d9322-120">名前</span><span class="sxs-lookup"><span data-stu-id="d9322-120">Name</span></span>       | <span data-ttu-id="d9322-121">説明</span><span class="sxs-lookup"><span data-stu-id="d9322-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9322-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9322-122">Authorization</span></span>  | <span data-ttu-id="d9322-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d9322-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9322-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d9322-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d9322-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="d9322-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9322-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9322-128">Request body</span></span>
<span data-ttu-id="d9322-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d9322-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d9322-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d9322-130">Parameter</span></span>    | <span data-ttu-id="d9322-131">型</span><span class="sxs-lookup"><span data-stu-id="d9322-131">Type</span></span>   |<span data-ttu-id="d9322-132">説明</span><span class="sxs-lookup"><span data-stu-id="d9322-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9322-133">options</span><span class="sxs-lookup"><span data-stu-id="d9322-133">options</span></span>|<span data-ttu-id="d9322-134">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="d9322-134">WorksheetProtectionOptions</span></span>|<span data-ttu-id="d9322-p106">省略可能。シートの保護のオプション。</span><span class="sxs-lookup"><span data-stu-id="d9322-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="d9322-137">応答</span><span class="sxs-lookup"><span data-stu-id="d9322-137">Response</span></span>

<span data-ttu-id="d9322-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d9322-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9322-140">例</span><span class="sxs-lookup"><span data-stu-id="d9322-140">Example</span></span>
<span data-ttu-id="d9322-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d9322-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d9322-142">要求</span><span class="sxs-lookup"><span data-stu-id="d9322-142">Request</span></span>
<span data-ttu-id="d9322-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d9322-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d9322-144">応答</span><span class="sxs-lookup"><span data-stu-id="d9322-144">Response</span></span>
<span data-ttu-id="d9322-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d9322-145">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheetprotection-protect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
