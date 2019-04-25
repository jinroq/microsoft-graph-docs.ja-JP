---
title: 'WorksheetProtection: unprotect'
description: ワークシートの保護を解除します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9fe503034e2d54dd1df7282c2c0e5fa0819bfdfd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535819"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="cafce-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="cafce-103">WorksheetProtection: unprotect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cafce-104">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="cafce-104">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="cafce-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cafce-105">Permissions</span></span>
<span data-ttu-id="cafce-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cafce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cafce-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cafce-108">Permission type</span></span>      | <span data-ttu-id="cafce-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cafce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cafce-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cafce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cafce-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cafce-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cafce-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cafce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cafce-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cafce-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cafce-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cafce-114">Application</span></span> | <span data-ttu-id="cafce-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cafce-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cafce-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cafce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="cafce-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cafce-117">Request headers</span></span>
| <span data-ttu-id="cafce-118">名前</span><span class="sxs-lookup"><span data-stu-id="cafce-118">Name</span></span>       | <span data-ttu-id="cafce-119">説明</span><span class="sxs-lookup"><span data-stu-id="cafce-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cafce-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cafce-120">Authorization</span></span>  | <span data-ttu-id="cafce-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cafce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cafce-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cafce-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cafce-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="cafce-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cafce-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cafce-126">Request body</span></span>
<span data-ttu-id="cafce-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="cafce-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cafce-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cafce-128">Parameter</span></span>    | <span data-ttu-id="cafce-129">型</span><span class="sxs-lookup"><span data-stu-id="cafce-129">Type</span></span>   |<span data-ttu-id="cafce-130">説明</span><span class="sxs-lookup"><span data-stu-id="cafce-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cafce-131">password</span><span class="sxs-lookup"><span data-stu-id="cafce-131">password</span></span>|<span data-ttu-id="cafce-132">string</span><span class="sxs-lookup"><span data-stu-id="cafce-132">string</span></span>|<span data-ttu-id="cafce-p104">省略可能。シートの保護パスワード。</span><span class="sxs-lookup"><span data-stu-id="cafce-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="cafce-135">応答</span><span class="sxs-lookup"><span data-stu-id="cafce-135">Response</span></span>

<span data-ttu-id="cafce-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cafce-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cafce-138">例</span><span class="sxs-lookup"><span data-stu-id="cafce-138">Example</span></span>
<span data-ttu-id="cafce-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="cafce-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cafce-140">要求</span><span class="sxs-lookup"><span data-stu-id="cafce-140">Request</span></span>
<span data-ttu-id="cafce-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cafce-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="cafce-142">応答</span><span class="sxs-lookup"><span data-stu-id="cafce-142">Response</span></span>
<span data-ttu-id="cafce-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cafce-143">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheetprotection-unprotect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
