---
title: 'WorksheetProtection: unprotect'
description: ワークシートの保護を解除します。
author: lumine2008
ms.openlocfilehash: 11dc000919fc1b60bae7646d00cc669f63a3f690
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341042"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="6c6fb-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="6c6fb-103">WorksheetProtection: unprotect</span></span>

> <span data-ttu-id="6c6fb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c6fb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c6fb-106">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-106">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="6c6fb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c6fb-107">Permissions</span></span>
<span data-ttu-id="6c6fb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c6fb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c6fb-110">Permission type</span></span>      | <span data-ttu-id="6c6fb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c6fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c6fb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c6fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6c6fb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c6fb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c6fb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c6fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c6fb-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c6fb-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c6fb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c6fb-116">Application</span></span> | <span data-ttu-id="6c6fb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c6fb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c6fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="6c6fb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c6fb-119">Request headers</span></span>
| <span data-ttu-id="6c6fb-120">名前</span><span class="sxs-lookup"><span data-stu-id="6c6fb-120">Name</span></span>       | <span data-ttu-id="6c6fb-121">説明</span><span class="sxs-lookup"><span data-stu-id="6c6fb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6c6fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c6fb-122">Authorization</span></span>  | <span data-ttu-id="6c6fb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c6fb-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6c6fb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6c6fb-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c6fb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c6fb-128">Request body</span></span>
<span data-ttu-id="6c6fb-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6c6fb-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6c6fb-130">Parameter</span></span>    | <span data-ttu-id="6c6fb-131">種類</span><span class="sxs-lookup"><span data-stu-id="6c6fb-131">Type</span></span>   |<span data-ttu-id="6c6fb-132">説明</span><span class="sxs-lookup"><span data-stu-id="6c6fb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c6fb-133">password</span><span class="sxs-lookup"><span data-stu-id="6c6fb-133">password</span></span>|<span data-ttu-id="6c6fb-134">string</span><span class="sxs-lookup"><span data-stu-id="6c6fb-134">string</span></span>|<span data-ttu-id="6c6fb-p105">省略可能。シートの保護パスワード。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-p105">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="6c6fb-137">応答</span><span class="sxs-lookup"><span data-stu-id="6c6fb-137">Response</span></span>

<span data-ttu-id="6c6fb-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c6fb-140">例</span><span class="sxs-lookup"><span data-stu-id="6c6fb-140">Example</span></span>
<span data-ttu-id="6c6fb-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6c6fb-142">要求</span><span class="sxs-lookup"><span data-stu-id="6c6fb-142">Request</span></span>
<span data-ttu-id="6c6fb-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="6c6fb-144">応答</span><span class="sxs-lookup"><span data-stu-id="6c6fb-144">Response</span></span>
<span data-ttu-id="6c6fb-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6c6fb-145">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->