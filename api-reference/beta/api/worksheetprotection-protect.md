---
title: 'workbookWorksheetProtection: 保護'
description: ワークシートを保護します。 ワークシートが保護されている場合はスローします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 252fc45ec855d40cdd315b092d307675f0c88630
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325716"
---
# <a name="workbookworksheetprotection-protect"></a><span data-ttu-id="9419d-104">workbookWorksheetProtection: 保護</span><span class="sxs-lookup"><span data-stu-id="9419d-104">workbookWorksheetProtection: protect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9419d-p102">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="9419d-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="9419d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9419d-107">Permissions</span></span>
<span data-ttu-id="9419d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9419d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9419d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9419d-110">Permission type</span></span>      | <span data-ttu-id="9419d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9419d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9419d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9419d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9419d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9419d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9419d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9419d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9419d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9419d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9419d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9419d-116">Application</span></span> | <span data-ttu-id="9419d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9419d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9419d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9419d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="9419d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9419d-119">Request headers</span></span>
| <span data-ttu-id="9419d-120">名前</span><span class="sxs-lookup"><span data-stu-id="9419d-120">Name</span></span>       | <span data-ttu-id="9419d-121">説明</span><span class="sxs-lookup"><span data-stu-id="9419d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9419d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9419d-122">Authorization</span></span>  | <span data-ttu-id="9419d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9419d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9419d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9419d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9419d-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="9419d-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9419d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="9419d-128">Request body</span></span>
<span data-ttu-id="9419d-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9419d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9419d-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9419d-130">Parameter</span></span>    | <span data-ttu-id="9419d-131">型</span><span class="sxs-lookup"><span data-stu-id="9419d-131">Type</span></span>   |<span data-ttu-id="9419d-132">説明</span><span class="sxs-lookup"><span data-stu-id="9419d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9419d-133">オプション</span><span class="sxs-lookup"><span data-stu-id="9419d-133">options</span></span>|[<span data-ttu-id="9419d-134">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="9419d-134">workbookWorksheetProtectionOptions</span></span>](../resources/workbookworksheetprotectionoptions.md)|<span data-ttu-id="9419d-p106">省略可能。シートの保護のオプション。</span><span class="sxs-lookup"><span data-stu-id="9419d-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="9419d-137">応答</span><span class="sxs-lookup"><span data-stu-id="9419d-137">Response</span></span>

<span data-ttu-id="9419d-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9419d-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9419d-140">例</span><span class="sxs-lookup"><span data-stu-id="9419d-140">Example</span></span>
<span data-ttu-id="9419d-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9419d-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9419d-142">要求</span><span class="sxs-lookup"><span data-stu-id="9419d-142">Request</span></span>
<span data-ttu-id="9419d-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9419d-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9419d-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9419d-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9419d-145">C#</span><span class="sxs-lookup"><span data-stu-id="9419d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookworksheetprotection-protect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9419d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9419d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookworksheetprotection-protect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9419d-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="9419d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookworksheetprotection-protect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9419d-148">Java</span><span class="sxs-lookup"><span data-stu-id="9419d-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookworksheetprotection-protect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9419d-149">応答</span><span class="sxs-lookup"><span data-stu-id="9419d-149">Response</span></span>
<span data-ttu-id="9419d-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9419d-150">Here is an example of the response.</span></span> 
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
