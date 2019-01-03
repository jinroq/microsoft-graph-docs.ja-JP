---
title: 'TableSort: apply　'
description: 並べ替え操作を実行します。
author: lumine2008
ms.openlocfilehash: ed5b862227986e9e280462d0118f2286dd1c9107
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333125"
---
# <a name="tablesort-apply"></a><span data-ttu-id="24f84-103">TableSort: apply　</span><span class="sxs-lookup"><span data-stu-id="24f84-103">TableSort: apply</span></span>

> <span data-ttu-id="24f84-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24f84-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24f84-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24f84-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24f84-106">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="24f84-106">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="24f84-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="24f84-107">Permissions</span></span>
<span data-ttu-id="24f84-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24f84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24f84-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24f84-110">Permission type</span></span>      | <span data-ttu-id="24f84-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="24f84-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24f84-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24f84-112">Delegated (work or school account)</span></span> | <span data-ttu-id="24f84-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24f84-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24f84-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24f84-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24f84-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24f84-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24f84-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24f84-116">Application</span></span> | <span data-ttu-id="24f84-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24f84-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24f84-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24f84-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="24f84-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24f84-119">Request headers</span></span>
| <span data-ttu-id="24f84-120">名前</span><span class="sxs-lookup"><span data-stu-id="24f84-120">Name</span></span>       | <span data-ttu-id="24f84-121">説明</span><span class="sxs-lookup"><span data-stu-id="24f84-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="24f84-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24f84-122">Authorization</span></span>  | <span data-ttu-id="24f84-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="24f84-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24f84-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="24f84-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="24f84-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="24f84-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24f84-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="24f84-128">Request body</span></span>
<span data-ttu-id="24f84-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="24f84-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24f84-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="24f84-130">Parameter</span></span>    | <span data-ttu-id="24f84-131">種類</span><span class="sxs-lookup"><span data-stu-id="24f84-131">Type</span></span>   |<span data-ttu-id="24f84-132">説明</span><span class="sxs-lookup"><span data-stu-id="24f84-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24f84-133">fields</span><span class="sxs-lookup"><span data-stu-id="24f84-133">fields</span></span>|<span data-ttu-id="24f84-134">SortField</span><span class="sxs-lookup"><span data-stu-id="24f84-134">SortField</span></span>|<span data-ttu-id="24f84-135">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="24f84-135">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="24f84-136">matchCase</span><span class="sxs-lookup"><span data-stu-id="24f84-136">matchCase</span></span>|<span data-ttu-id="24f84-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="24f84-137">boolean</span></span>|<span data-ttu-id="24f84-p105">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="24f84-p105">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="24f84-140">method</span><span class="sxs-lookup"><span data-stu-id="24f84-140">method</span></span>|<span data-ttu-id="24f84-141">string</span><span class="sxs-lookup"><span data-stu-id="24f84-141">string</span></span>|<span data-ttu-id="24f84-p106">省略可能。中国語文字に使用される順序付けの方法です。可能な値は、`PinYin`、`StrokeCount` です。</span><span class="sxs-lookup"><span data-stu-id="24f84-p106">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="24f84-145">応答</span><span class="sxs-lookup"><span data-stu-id="24f84-145">Response</span></span>

<span data-ttu-id="24f84-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="24f84-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24f84-148">例</span><span class="sxs-lookup"><span data-stu-id="24f84-148">Example</span></span>
<span data-ttu-id="24f84-149">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="24f84-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24f84-150">要求</span><span class="sxs-lookup"><span data-stu-id="24f84-150">Request</span></span>
<span data-ttu-id="24f84-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24f84-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="24f84-152">応答</span><span class="sxs-lookup"><span data-stu-id="24f84-152">Response</span></span>
<span data-ttu-id="24f84-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="24f84-153">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->