---
title: 'RangeFormat: autofitRows'
description: 現在の列のデータに基づいて、現在の範囲の行の高さを最適な高さに変更します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a25fdd90f8bb0f7ad92aca5207c1529abc370a65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546153"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="20003-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="20003-103">RangeFormat: autofitRows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20003-104">現在の列のデータに基づいて、現在の範囲の行の高さを最適な高さに変更します。</span><span class="sxs-lookup"><span data-stu-id="20003-104">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="20003-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="20003-105">Permissions</span></span>
<span data-ttu-id="20003-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20003-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20003-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20003-108">Permission type</span></span>      | <span data-ttu-id="20003-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="20003-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20003-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20003-110">Delegated (work or school account)</span></span> | <span data-ttu-id="20003-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20003-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20003-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20003-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20003-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20003-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20003-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20003-114">Application</span></span> | <span data-ttu-id="20003-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20003-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20003-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20003-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="20003-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20003-117">Request headers</span></span>
| <span data-ttu-id="20003-118">名前</span><span class="sxs-lookup"><span data-stu-id="20003-118">Name</span></span>       | <span data-ttu-id="20003-119">説明</span><span class="sxs-lookup"><span data-stu-id="20003-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20003-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="20003-120">Authorization</span></span>  | <span data-ttu-id="20003-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="20003-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20003-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="20003-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="20003-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="20003-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20003-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="20003-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="20003-127">応答</span><span class="sxs-lookup"><span data-stu-id="20003-127">Response</span></span>

<span data-ttu-id="20003-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="20003-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20003-130">例</span><span class="sxs-lookup"><span data-stu-id="20003-130">Example</span></span>
<span data-ttu-id="20003-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="20003-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="20003-132">要求</span><span class="sxs-lookup"><span data-stu-id="20003-132">Request</span></span>
<span data-ttu-id="20003-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="20003-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="20003-134">応答</span><span class="sxs-lookup"><span data-stu-id="20003-134">Response</span></span>
<span data-ttu-id="20003-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="20003-135">Here is an example of the response.</span></span> 
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
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangeformat-autofitrows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
