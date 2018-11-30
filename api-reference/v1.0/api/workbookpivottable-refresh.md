---
title: 'workbookPivotTable: refresh'
description: ピボットテーブルを更新します。
ms.openlocfilehash: 3acbe6efb29d6846b48bfae250731640ad533dad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021361"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="04646-103">workbookPivotTable: refresh</span><span class="sxs-lookup"><span data-stu-id="04646-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="04646-104">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="04646-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="04646-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04646-105">Permissions</span></span>
<span data-ttu-id="04646-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04646-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="04646-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04646-108">Permission type</span></span>      | <span data-ttu-id="04646-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04646-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04646-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04646-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04646-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04646-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="04646-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04646-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04646-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04646-113">Not supported.</span></span>    |
|<span data-ttu-id="04646-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04646-114">Application</span></span> | <span data-ttu-id="04646-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04646-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04646-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04646-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="04646-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04646-117">Request headers</span></span>
| <span data-ttu-id="04646-118">名前</span><span class="sxs-lookup"><span data-stu-id="04646-118">Name</span></span>       | <span data-ttu-id="04646-119">説明</span><span class="sxs-lookup"><span data-stu-id="04646-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="04646-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="04646-120">Authorization</span></span>  | <span data-ttu-id="04646-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04646-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04646-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="04646-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="04646-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="04646-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04646-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="04646-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="04646-127">応答</span><span class="sxs-lookup"><span data-stu-id="04646-127">Response</span></span>
<span data-ttu-id="04646-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="04646-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04646-130">例</span><span class="sxs-lookup"><span data-stu-id="04646-130">Example</span></span>
<span data-ttu-id="04646-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="04646-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="04646-132">要求</span><span class="sxs-lookup"><span data-stu-id="04646-132">Request</span></span>
<span data-ttu-id="04646-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04646-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="04646-134">応答</span><span class="sxs-lookup"><span data-stu-id="04646-134">Response</span></span>
<span data-ttu-id="04646-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="04646-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
