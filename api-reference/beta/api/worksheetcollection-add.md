---
title: 'WorksheetCollection: add'
description: 上に .activate()。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0958f8f82502c92eff08ec80a7b116c1b0c4a5f0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508049"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="9214c-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="9214c-103">WorksheetCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9214c-p101">新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。新しく追加したワークシートをアクティブにする場合は、そのワークシートに対して ".activate() を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="9214c-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="9214c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9214c-107">Permissions</span></span>
<span data-ttu-id="9214c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9214c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9214c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9214c-110">Permission type</span></span>      | <span data-ttu-id="9214c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9214c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9214c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9214c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9214c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9214c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9214c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9214c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9214c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9214c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9214c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9214c-116">Application</span></span> | <span data-ttu-id="9214c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9214c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9214c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9214c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="9214c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9214c-119">Request headers</span></span>
| <span data-ttu-id="9214c-120">名前</span><span class="sxs-lookup"><span data-stu-id="9214c-120">Name</span></span>       | <span data-ttu-id="9214c-121">説明</span><span class="sxs-lookup"><span data-stu-id="9214c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9214c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9214c-122">Authorization</span></span>  | <span data-ttu-id="9214c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9214c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9214c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9214c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9214c-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="9214c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9214c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="9214c-128">Request body</span></span>
<span data-ttu-id="9214c-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9214c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9214c-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9214c-130">Parameter</span></span>    | <span data-ttu-id="9214c-131">型</span><span class="sxs-lookup"><span data-stu-id="9214c-131">Type</span></span>   |<span data-ttu-id="9214c-132">説明</span><span class="sxs-lookup"><span data-stu-id="9214c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9214c-133">name</span><span class="sxs-lookup"><span data-stu-id="9214c-133">name</span></span>|<span data-ttu-id="9214c-134">文字列</span><span class="sxs-lookup"><span data-stu-id="9214c-134">string</span></span>|<span data-ttu-id="9214c-p105">省略可能。追加するワークシートの名前。指定する場合、名前は一意である必要があります。指定されていない場合は、Excel が新しいワークシートの名前を決定します。</span><span class="sxs-lookup"><span data-stu-id="9214c-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="9214c-139">応答</span><span class="sxs-lookup"><span data-stu-id="9214c-139">Response</span></span>

<span data-ttu-id="9214c-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ワークシート](../resources/worksheet.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9214c-140">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9214c-141">例</span><span class="sxs-lookup"><span data-stu-id="9214c-141">Example</span></span>
<span data-ttu-id="9214c-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9214c-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9214c-143">要求</span><span class="sxs-lookup"><span data-stu-id="9214c-143">Request</span></span>
<span data-ttu-id="9214c-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9214c-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9214c-145">応答</span><span class="sxs-lookup"><span data-stu-id="9214c-145">Response</span></span>
<span data-ttu-id="9214c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9214c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
