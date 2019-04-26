---
title: 'ChartLineFormat: clear'
description: グラフ要素の線の書式をクリアします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9de8ea98b56e14714dc856d16b3cd33224d803c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327717"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="b93ac-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="b93ac-103">ChartLineFormat: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b93ac-104">グラフ要素の線の書式をクリアします。</span><span class="sxs-lookup"><span data-stu-id="b93ac-104">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="b93ac-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b93ac-105">Permissions</span></span>
<span data-ttu-id="b93ac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b93ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b93ac-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b93ac-108">Permission type</span></span>      | <span data-ttu-id="b93ac-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b93ac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b93ac-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b93ac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b93ac-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b93ac-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b93ac-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b93ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b93ac-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b93ac-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b93ac-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b93ac-114">Application</span></span> | <span data-ttu-id="b93ac-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b93ac-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b93ac-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b93ac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="b93ac-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b93ac-117">Request headers</span></span>
| <span data-ttu-id="b93ac-118">名前</span><span class="sxs-lookup"><span data-stu-id="b93ac-118">Name</span></span>       | <span data-ttu-id="b93ac-119">説明</span><span class="sxs-lookup"><span data-stu-id="b93ac-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b93ac-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b93ac-120">Authorization</span></span>  | <span data-ttu-id="b93ac-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b93ac-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b93ac-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b93ac-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b93ac-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b93ac-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b93ac-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b93ac-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b93ac-127">応答</span><span class="sxs-lookup"><span data-stu-id="b93ac-127">Response</span></span>

<span data-ttu-id="b93ac-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b93ac-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b93ac-130">例</span><span class="sxs-lookup"><span data-stu-id="b93ac-130">Example</span></span>
<span data-ttu-id="b93ac-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b93ac-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b93ac-132">要求</span><span class="sxs-lookup"><span data-stu-id="b93ac-132">Request</span></span>
<span data-ttu-id="b93ac-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b93ac-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear
```

##### <a name="response"></a><span data-ttu-id="b93ac-134">応答</span><span class="sxs-lookup"><span data-stu-id="b93ac-134">Response</span></span>
<span data-ttu-id="b93ac-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b93ac-135">Here is an example of the response.</span></span> 
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
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
