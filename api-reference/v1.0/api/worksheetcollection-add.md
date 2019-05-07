---
title: 'WorksheetCollection: add'
description: . を有効にします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3805879e27ad3cc16b1a14fd8f4c31a5ebecdce3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601076"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="1287d-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="1287d-103">WorksheetCollection: add</span></span>

<span data-ttu-id="1287d-p101">新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。新しく追加したワークシートをアクティブにする場合は、そのワークシートに対して ".activate() を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="1287d-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="1287d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1287d-107">Permissions</span></span>
<span data-ttu-id="1287d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1287d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1287d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1287d-110">Permission type</span></span>      | <span data-ttu-id="1287d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1287d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1287d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1287d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1287d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1287d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1287d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1287d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1287d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1287d-115">Not supported.</span></span>    |
|<span data-ttu-id="1287d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1287d-116">Application</span></span> | <span data-ttu-id="1287d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1287d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1287d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1287d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="1287d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1287d-119">Request headers</span></span>
| <span data-ttu-id="1287d-120">名前</span><span class="sxs-lookup"><span data-stu-id="1287d-120">Name</span></span>       | <span data-ttu-id="1287d-121">説明</span><span class="sxs-lookup"><span data-stu-id="1287d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1287d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1287d-122">Authorization</span></span>  | <span data-ttu-id="1287d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1287d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1287d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1287d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1287d-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1287d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1287d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1287d-128">Request body</span></span>
<span data-ttu-id="1287d-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1287d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1287d-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1287d-130">Parameter</span></span>    | <span data-ttu-id="1287d-131">型</span><span class="sxs-lookup"><span data-stu-id="1287d-131">Type</span></span>   |<span data-ttu-id="1287d-132">説明</span><span class="sxs-lookup"><span data-stu-id="1287d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1287d-133">name</span><span class="sxs-lookup"><span data-stu-id="1287d-133">name</span></span>|<span data-ttu-id="1287d-134">string</span><span class="sxs-lookup"><span data-stu-id="1287d-134">string</span></span>|<span data-ttu-id="1287d-p105">省略可能。追加するワークシートの名前。指定する場合、名前は一意である必要があります。指定されていない場合は、Excel が新しいワークシートの名前を決定します。</span><span class="sxs-lookup"><span data-stu-id="1287d-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="1287d-139">応答</span><span class="sxs-lookup"><span data-stu-id="1287d-139">Response</span></span>

<span data-ttu-id="1287d-140">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[WorkbookWorksheet](../resources/worksheet.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1287d-140">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1287d-141">例</span><span class="sxs-lookup"><span data-stu-id="1287d-141">Example</span></span>
<span data-ttu-id="1287d-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1287d-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1287d-143">要求</span><span class="sxs-lookup"><span data-stu-id="1287d-143">Request</span></span>
<span data-ttu-id="1287d-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1287d-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="1287d-145">応答</span><span class="sxs-lookup"><span data-stu-id="1287d-145">Response</span></span>
<span data-ttu-id="1287d-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1287d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1287d-149">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1287d-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1287d-150">Visual</span><span class="sxs-lookup"><span data-stu-id="1287d-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheetcollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1287d-151">Java</span><span class="sxs-lookup"><span data-stu-id="1287d-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheetcollection_add-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheetcollection-add.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheetcollection-add.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
