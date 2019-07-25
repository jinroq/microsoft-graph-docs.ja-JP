---
title: 'workbookWorksheetProtection: 保護'
description: ワークシートを保護します。 ワークシートが保護されている場合はスローします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 74184a84e7411a908be8dc084b78560f4b4061d0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866031"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="d9b19-104">workbookWorksheetProtection: 保護</span><span class="sxs-lookup"><span data-stu-id="d9b19-104">workbookWorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9b19-p102">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="d9b19-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9b19-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d9b19-107">Permissions</span></span>
<span data-ttu-id="d9b19-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9b19-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9b19-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9b19-110">Permission type</span></span>      | <span data-ttu-id="d9b19-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9b19-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9b19-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9b19-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9b19-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9b19-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9b19-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9b19-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9b19-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9b19-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9b19-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9b19-116">Application</span></span> | <span data-ttu-id="d9b19-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9b19-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9b19-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9b19-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="d9b19-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9b19-119">Request headers</span></span>
| <span data-ttu-id="d9b19-120">名前</span><span class="sxs-lookup"><span data-stu-id="d9b19-120">Name</span></span>       | <span data-ttu-id="d9b19-121">説明</span><span class="sxs-lookup"><span data-stu-id="d9b19-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9b19-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9b19-122">Authorization</span></span>  | <span data-ttu-id="d9b19-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d9b19-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9b19-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d9b19-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d9b19-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="d9b19-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9b19-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9b19-128">Request body</span></span>
<span data-ttu-id="d9b19-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d9b19-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d9b19-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d9b19-130">Parameter</span></span>    | <span data-ttu-id="d9b19-131">型</span><span class="sxs-lookup"><span data-stu-id="d9b19-131">Type</span></span>   |<span data-ttu-id="d9b19-132">説明</span><span class="sxs-lookup"><span data-stu-id="d9b19-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9b19-133">オプション</span><span class="sxs-lookup"><span data-stu-id="d9b19-133">options</span></span>|[<span data-ttu-id="d9b19-134">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="d9b19-134">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="d9b19-p106">省略可能。シートの保護のオプション。</span><span class="sxs-lookup"><span data-stu-id="d9b19-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="d9b19-137">応答</span><span class="sxs-lookup"><span data-stu-id="d9b19-137">Response</span></span>

<span data-ttu-id="d9b19-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d9b19-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9b19-140">例</span><span class="sxs-lookup"><span data-stu-id="d9b19-140">Example</span></span>
<span data-ttu-id="d9b19-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d9b19-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d9b19-142">要求</span><span class="sxs-lookup"><span data-stu-id="d9b19-142">Request</span></span>
<span data-ttu-id="d9b19-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d9b19-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d9b19-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d9b19-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookworksheetprotection_protect"
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d9b19-145">C#</span><span class="sxs-lookup"><span data-stu-id="d9b19-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9b19-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="d9b19-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d9b19-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="d9b19-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d9b19-148">Java</span><span class="sxs-lookup"><span data-stu-id="d9b19-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookworksheetprotection-protect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d9b19-149">応答</span><span class="sxs-lookup"><span data-stu-id="d9b19-149">Response</span></span>
<span data-ttu-id="d9b19-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d9b19-150">Here is an example of the response.</span></span> 
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
  "description": "workbookWorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
