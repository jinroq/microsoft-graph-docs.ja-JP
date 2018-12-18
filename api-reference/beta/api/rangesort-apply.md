---
title: 'RangeSort: 適用'
description: 並べ替え操作を実行します。
author: lumine2008
ms.openlocfilehash: df083fb9f81e529d3f70363eaedec6e4286fc835
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330220"
---
# <a name="rangesort-apply"></a><span data-ttu-id="c5f03-103">RangeSort: 適用</span><span class="sxs-lookup"><span data-stu-id="c5f03-103">RangeSort: apply</span></span>

> <span data-ttu-id="c5f03-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c5f03-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5f03-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5f03-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5f03-106">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="c5f03-106">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5f03-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c5f03-107">Permissions</span></span>
<span data-ttu-id="c5f03-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5f03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f03-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5f03-110">Permission type</span></span>      | <span data-ttu-id="c5f03-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5f03-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5f03-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5f03-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c5f03-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5f03-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5f03-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5f03-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5f03-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5f03-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5f03-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5f03-116">Application</span></span> | <span data-ttu-id="c5f03-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5f03-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5f03-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5f03-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="c5f03-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5f03-119">Request headers</span></span>
| <span data-ttu-id="c5f03-120">名前</span><span class="sxs-lookup"><span data-stu-id="c5f03-120">Name</span></span>       | <span data-ttu-id="c5f03-121">説明</span><span class="sxs-lookup"><span data-stu-id="c5f03-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5f03-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f03-122">Authorization</span></span>  | <span data-ttu-id="c5f03-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c5f03-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5f03-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c5f03-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c5f03-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c5f03-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f03-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c5f03-128">Request body</span></span>
<span data-ttu-id="c5f03-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5f03-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5f03-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c5f03-130">Parameter</span></span>    | <span data-ttu-id="c5f03-131">種類</span><span class="sxs-lookup"><span data-stu-id="c5f03-131">Type</span></span>   |<span data-ttu-id="c5f03-132">説明</span><span class="sxs-lookup"><span data-stu-id="c5f03-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5f03-133">fields</span><span class="sxs-lookup"><span data-stu-id="c5f03-133">fields</span></span>|<span data-ttu-id="c5f03-134">SortField</span><span class="sxs-lookup"><span data-stu-id="c5f03-134">SortField</span></span>|<span data-ttu-id="c5f03-135">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="c5f03-135">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="c5f03-136">matchCase</span><span class="sxs-lookup"><span data-stu-id="c5f03-136">matchCase</span></span>|<span data-ttu-id="c5f03-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="c5f03-137">boolean</span></span>|<span data-ttu-id="c5f03-p105">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="c5f03-p105">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="c5f03-140">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="c5f03-140">hasHeaders</span></span>|<span data-ttu-id="c5f03-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="c5f03-141">boolean</span></span>|<span data-ttu-id="c5f03-p106">省略可能。範囲にヘッダーがあるかどうか。</span><span class="sxs-lookup"><span data-stu-id="c5f03-p106">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="c5f03-144">orientation</span><span class="sxs-lookup"><span data-stu-id="c5f03-144">orientation</span></span>|<span data-ttu-id="c5f03-145">string</span><span class="sxs-lookup"><span data-stu-id="c5f03-145">string</span></span>|<span data-ttu-id="c5f03-p107">省略可能。操作が行と列のどちらの並べ替えかを示します。可能な値は、`Rows`、`Columns` です。</span><span class="sxs-lookup"><span data-stu-id="c5f03-p107">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="c5f03-149">method</span><span class="sxs-lookup"><span data-stu-id="c5f03-149">method</span></span>|<span data-ttu-id="c5f03-150">string</span><span class="sxs-lookup"><span data-stu-id="c5f03-150">string</span></span>|<span data-ttu-id="c5f03-p108">省略可能。中国語文字に使用される順序付けの方法です。可能な値は、`PinYin`、`StrokeCount` です。</span><span class="sxs-lookup"><span data-stu-id="c5f03-p108">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="c5f03-154">応答</span><span class="sxs-lookup"><span data-stu-id="c5f03-154">Response</span></span>

<span data-ttu-id="c5f03-p109">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c5f03-p109">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f03-157">例</span><span class="sxs-lookup"><span data-stu-id="c5f03-157">Example</span></span>
<span data-ttu-id="c5f03-158">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c5f03-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c5f03-159">要求</span><span class="sxs-lookup"><span data-stu-id="c5f03-159">Request</span></span>
<span data-ttu-id="c5f03-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c5f03-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
Content-type: application/json
Content-length: 358

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
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="c5f03-161">応答</span><span class="sxs-lookup"><span data-stu-id="c5f03-161">Response</span></span>
<span data-ttu-id="c5f03-162">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c5f03-162">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->