---
title: 'Worksheet: delete'
description: ブックからワークシートを削除します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 44bc958cc806745e91af01ec38bb2b57a271b093
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526789"
---
# <a name="worksheet-delete"></a><span data-ttu-id="8c287-103">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="8c287-103">Worksheet: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c287-104">ブックからワークシートを削除します。</span><span class="sxs-lookup"><span data-stu-id="8c287-104">Deletes the worksheet from the workbook.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c287-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c287-105">Permissions</span></span>
<span data-ttu-id="8c287-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c287-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c287-108">Permission type</span></span>      | <span data-ttu-id="8c287-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c287-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c287-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c287-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c287-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c287-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c287-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c287-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c287-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c287-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c287-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c287-114">Application</span></span> | <span data-ttu-id="8c287-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c287-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c287-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c287-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="8c287-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c287-117">Request headers</span></span>
| <span data-ttu-id="8c287-118">名前</span><span class="sxs-lookup"><span data-stu-id="8c287-118">Name</span></span>       | <span data-ttu-id="8c287-119">説明</span><span class="sxs-lookup"><span data-stu-id="8c287-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c287-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c287-120">Authorization</span></span>  | <span data-ttu-id="8c287-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c287-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c287-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8c287-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8c287-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="8c287-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c287-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c287-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8c287-127">応答</span><span class="sxs-lookup"><span data-stu-id="8c287-127">Response</span></span>

<span data-ttu-id="8c287-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8c287-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c287-130">例</span><span class="sxs-lookup"><span data-stu-id="8c287-130">Example</span></span>
<span data-ttu-id="8c287-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8c287-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c287-132">要求</span><span class="sxs-lookup"><span data-stu-id="8c287-132">Request</span></span>
<span data-ttu-id="8c287-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c287-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="8c287-134">応答</span><span class="sxs-lookup"><span data-stu-id="8c287-134">Response</span></span>
<span data-ttu-id="8c287-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8c287-135">Here is an example of the response.</span></span> 
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
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
