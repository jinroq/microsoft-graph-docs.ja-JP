---
title: 'workbookPivotTable: refreshAll'
description: 指定されたワークシート内のピボットテーブルを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1d245bd773ad493c6a2fb002666512ad92cae95f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534662"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="cc8de-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="cc8de-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="cc8de-104">指定されたワークシート内のピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="cc8de-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc8de-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc8de-105">Permissions</span></span>
<span data-ttu-id="cc8de-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc8de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc8de-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc8de-108">Permission type</span></span>      | <span data-ttu-id="cc8de-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc8de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc8de-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc8de-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cc8de-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc8de-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cc8de-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc8de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc8de-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc8de-113">Not supported.</span></span>    |
|<span data-ttu-id="cc8de-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc8de-114">Application</span></span> | <span data-ttu-id="cc8de-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc8de-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc8de-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc8de-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="cc8de-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc8de-117">Request headers</span></span>
| <span data-ttu-id="cc8de-118">名前</span><span class="sxs-lookup"><span data-stu-id="cc8de-118">Name</span></span>       | <span data-ttu-id="cc8de-119">説明</span><span class="sxs-lookup"><span data-stu-id="cc8de-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cc8de-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc8de-120">Authorization</span></span>  | <span data-ttu-id="cc8de-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc8de-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc8de-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cc8de-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cc8de-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="cc8de-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc8de-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc8de-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="cc8de-127">応答</span><span class="sxs-lookup"><span data-stu-id="cc8de-127">Response</span></span>
<span data-ttu-id="cc8de-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cc8de-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc8de-130">例</span><span class="sxs-lookup"><span data-stu-id="cc8de-130">Example</span></span>
<span data-ttu-id="cc8de-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="cc8de-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cc8de-132">要求</span><span class="sxs-lookup"><span data-stu-id="cc8de-132">Request</span></span>
<span data-ttu-id="cc8de-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc8de-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="cc8de-134">応答</span><span class="sxs-lookup"><span data-stu-id="cc8de-134">Response</span></span>
<span data-ttu-id="cc8de-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cc8de-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
