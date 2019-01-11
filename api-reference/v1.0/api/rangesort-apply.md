---
title: 'RangeSort: 適用'
description: 並べ替え操作を実行します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6298bc4368126debc384b4eafcbb05154c35aab6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825628"
---
# <a name="rangesort-apply"></a><span data-ttu-id="3a590-103">RangeSort: 適用</span><span class="sxs-lookup"><span data-stu-id="3a590-103">RangeSort: apply</span></span>

<span data-ttu-id="3a590-104">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="3a590-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a590-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3a590-105">Permissions</span></span>
<span data-ttu-id="3a590-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a590-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a590-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a590-108">Permission type</span></span>      | <span data-ttu-id="3a590-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a590-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a590-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a590-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a590-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a590-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a590-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a590-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a590-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a590-113">Not supported.</span></span>    |
|<span data-ttu-id="3a590-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a590-114">Application</span></span> | <span data-ttu-id="3a590-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a590-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a590-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a590-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="3a590-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a590-117">Request headers</span></span>
| <span data-ttu-id="3a590-118">名前</span><span class="sxs-lookup"><span data-stu-id="3a590-118">Name</span></span>       | <span data-ttu-id="3a590-119">説明</span><span class="sxs-lookup"><span data-stu-id="3a590-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3a590-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a590-120">Authorization</span></span>  | <span data-ttu-id="3a590-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3a590-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a590-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3a590-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3a590-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3a590-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a590-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a590-126">Request body</span></span>
<span data-ttu-id="3a590-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3a590-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a590-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a590-128">Parameter</span></span>    | <span data-ttu-id="3a590-129">Type</span><span class="sxs-lookup"><span data-stu-id="3a590-129">Type</span></span>   |<span data-ttu-id="3a590-130">説明</span><span class="sxs-lookup"><span data-stu-id="3a590-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a590-131">fields</span><span class="sxs-lookup"><span data-stu-id="3a590-131">fields</span></span>|<span data-ttu-id="3a590-132">WorkbookSortField コレクション</span><span class="sxs-lookup"><span data-stu-id="3a590-132">WorkbookSortField collection</span></span>|<span data-ttu-id="3a590-133">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="3a590-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="3a590-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="3a590-134">matchCase</span></span>|<span data-ttu-id="3a590-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="3a590-135">boolean</span></span>|<span data-ttu-id="3a590-p104">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="3a590-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="3a590-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="3a590-138">hasHeaders</span></span>|<span data-ttu-id="3a590-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="3a590-139">boolean</span></span>|<span data-ttu-id="3a590-p105">省略可能。範囲にヘッダーがあるかどうか。</span><span class="sxs-lookup"><span data-stu-id="3a590-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="3a590-142">orientation</span><span class="sxs-lookup"><span data-stu-id="3a590-142">orientation</span></span>|<span data-ttu-id="3a590-143">文字列</span><span class="sxs-lookup"><span data-stu-id="3a590-143">string</span></span>|<span data-ttu-id="3a590-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="3a590-144">Optional.</span></span> <span data-ttu-id="3a590-145">かどうか操作が行または列を並べ替え。</span><span class="sxs-lookup"><span data-stu-id="3a590-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="3a590-146">可能な値: `Rows`、 `Columns`。</span><span class="sxs-lookup"><span data-stu-id="3a590-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="3a590-147">method</span><span class="sxs-lookup"><span data-stu-id="3a590-147">method</span></span>|<span data-ttu-id="3a590-148">文字列</span><span class="sxs-lookup"><span data-stu-id="3a590-148">string</span></span>|<span data-ttu-id="3a590-149">省略可能。</span><span class="sxs-lookup"><span data-stu-id="3a590-149">Optional.</span></span> <span data-ttu-id="3a590-150">中国語の文字に使用される順序の指定方法です。</span><span class="sxs-lookup"><span data-stu-id="3a590-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="3a590-151">可能な値: `PinYin`、 `StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="3a590-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="3a590-152">応答</span><span class="sxs-lookup"><span data-stu-id="3a590-152">Response</span></span>

<span data-ttu-id="3a590-p108">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3a590-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a590-155">例</span><span class="sxs-lookup"><span data-stu-id="3a590-155">Example</span></span>
<span data-ttu-id="3a590-156">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3a590-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a590-157">要求</span><span class="sxs-lookup"><span data-stu-id="3a590-157">Request</span></span>
<span data-ttu-id="3a590-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a590-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
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

##### <a name="response"></a><span data-ttu-id="3a590-159">応答</span><span class="sxs-lookup"><span data-stu-id="3a590-159">Response</span></span>
<span data-ttu-id="3a590-160">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3a590-160">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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
