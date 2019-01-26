---
title: 'WorksheetCollection: add'
description: 上に .activate()。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4c943cc041c00cd0f1a50384f5e891472f214301
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577516"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="6d0e0-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="6d0e0-103">WorksheetCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d0e0-p101">新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。新しく追加したワークシートをアクティブにする場合は、そのワークシートに対して ".activate() を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="6d0e0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6d0e0-107">Permissions</span></span>
<span data-ttu-id="6d0e0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d0e0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d0e0-110">Permission type</span></span>      | <span data-ttu-id="6d0e0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d0e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d0e0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d0e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6d0e0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d0e0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6d0e0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d0e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d0e0-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d0e0-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6d0e0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d0e0-116">Application</span></span> | <span data-ttu-id="6d0e0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d0e0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d0e0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="6d0e0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d0e0-119">Request headers</span></span>
| <span data-ttu-id="6d0e0-120">名前</span><span class="sxs-lookup"><span data-stu-id="6d0e0-120">Name</span></span>       | <span data-ttu-id="6d0e0-121">説明</span><span class="sxs-lookup"><span data-stu-id="6d0e0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6d0e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d0e0-122">Authorization</span></span>  | <span data-ttu-id="6d0e0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6d0e0-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6d0e0-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6d0e0-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d0e0-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d0e0-128">Request body</span></span>
<span data-ttu-id="6d0e0-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6d0e0-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6d0e0-130">Parameter</span></span>    | <span data-ttu-id="6d0e0-131">型</span><span class="sxs-lookup"><span data-stu-id="6d0e0-131">Type</span></span>   |<span data-ttu-id="6d0e0-132">説明</span><span class="sxs-lookup"><span data-stu-id="6d0e0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d0e0-133">name</span><span class="sxs-lookup"><span data-stu-id="6d0e0-133">name</span></span>|<span data-ttu-id="6d0e0-134">文字列</span><span class="sxs-lookup"><span data-stu-id="6d0e0-134">string</span></span>|<span data-ttu-id="6d0e0-p105">省略可能。追加するワークシートの名前。指定する場合、名前は一意である必要があります。指定されていない場合は、Excel が新しいワークシートの名前を決定します。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="6d0e0-139">応答</span><span class="sxs-lookup"><span data-stu-id="6d0e0-139">Response</span></span>

<span data-ttu-id="6d0e0-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ワークシート](../resources/worksheet.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-140">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d0e0-141">例</span><span class="sxs-lookup"><span data-stu-id="6d0e0-141">Example</span></span>
<span data-ttu-id="6d0e0-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6d0e0-143">要求</span><span class="sxs-lookup"><span data-stu-id="6d0e0-143">Request</span></span>
<span data-ttu-id="6d0e0-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6d0e0-145">応答</span><span class="sxs-lookup"><span data-stu-id="6d0e0-145">Response</span></span>
<span data-ttu-id="6d0e0-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6d0e0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheetcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
