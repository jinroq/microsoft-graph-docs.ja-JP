---
title: 'workbookPivotTable: refresh'
description: ピボットテーブルを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3238f67fc7f017e64ab327619a4f4f90fba71d1f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970781"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="77816-103">workbookPivotTable: refresh</span><span class="sxs-lookup"><span data-stu-id="77816-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="77816-104">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="77816-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="77816-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77816-105">Permissions</span></span>
<span data-ttu-id="77816-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77816-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="77816-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77816-108">Permission type</span></span>      | <span data-ttu-id="77816-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77816-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77816-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77816-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77816-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77816-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="77816-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77816-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77816-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77816-113">Not supported.</span></span>    |
|<span data-ttu-id="77816-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77816-114">Application</span></span> | <span data-ttu-id="77816-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77816-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77816-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77816-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="77816-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77816-117">Request headers</span></span>
| <span data-ttu-id="77816-118">名前</span><span class="sxs-lookup"><span data-stu-id="77816-118">Name</span></span>       | <span data-ttu-id="77816-119">説明</span><span class="sxs-lookup"><span data-stu-id="77816-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="77816-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="77816-120">Authorization</span></span>  | <span data-ttu-id="77816-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="77816-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77816-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="77816-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="77816-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="77816-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77816-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="77816-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="77816-127">応答</span><span class="sxs-lookup"><span data-stu-id="77816-127">Response</span></span>
<span data-ttu-id="77816-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="77816-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77816-130">例</span><span class="sxs-lookup"><span data-stu-id="77816-130">Example</span></span>
<span data-ttu-id="77816-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="77816-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="77816-132">要求</span><span class="sxs-lookup"><span data-stu-id="77816-132">Request</span></span>
<span data-ttu-id="77816-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77816-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="77816-134">応答</span><span class="sxs-lookup"><span data-stu-id="77816-134">Response</span></span>
<span data-ttu-id="77816-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="77816-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
