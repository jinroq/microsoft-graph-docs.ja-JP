---
title: 'RangeSort: 適用'
description: 並べ替え操作を実行します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: beaced8da56e82599fd2e900c04e909947d1893b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332169"
---
# <a name="rangesort-apply"></a><span data-ttu-id="df8b4-103">RangeSort: 適用</span><span class="sxs-lookup"><span data-stu-id="df8b4-103">RangeSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df8b4-104">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="df8b4-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="df8b4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="df8b4-105">Permissions</span></span>
<span data-ttu-id="df8b4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df8b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df8b4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df8b4-108">Permission type</span></span>      | <span data-ttu-id="df8b4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="df8b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df8b4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df8b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="df8b4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df8b4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="df8b4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="df8b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df8b4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df8b4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="df8b4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df8b4-114">Application</span></span> | <span data-ttu-id="df8b4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df8b4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df8b4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df8b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="df8b4-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df8b4-117">Request headers</span></span>
| <span data-ttu-id="df8b4-118">名前</span><span class="sxs-lookup"><span data-stu-id="df8b4-118">Name</span></span>       | <span data-ttu-id="df8b4-119">説明</span><span class="sxs-lookup"><span data-stu-id="df8b4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="df8b4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="df8b4-120">Authorization</span></span>  | <span data-ttu-id="df8b4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="df8b4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df8b4-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="df8b4-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="df8b4-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="df8b4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df8b4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="df8b4-126">Request body</span></span>
<span data-ttu-id="df8b4-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="df8b4-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="df8b4-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="df8b4-128">Parameter</span></span>    | <span data-ttu-id="df8b4-129">型</span><span class="sxs-lookup"><span data-stu-id="df8b4-129">Type</span></span>   |<span data-ttu-id="df8b4-130">説明</span><span class="sxs-lookup"><span data-stu-id="df8b4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df8b4-131">fields</span><span class="sxs-lookup"><span data-stu-id="df8b4-131">fields</span></span>|<span data-ttu-id="df8b4-132">workbookSortField コレクション</span><span class="sxs-lookup"><span data-stu-id="df8b4-132">workbookSortField collection</span></span>|<span data-ttu-id="df8b4-133">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="df8b4-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="df8b4-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="df8b4-134">matchCase</span></span>|<span data-ttu-id="df8b4-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="df8b4-135">boolean</span></span>|<span data-ttu-id="df8b4-p104">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="df8b4-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="df8b4-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="df8b4-138">hasHeaders</span></span>|<span data-ttu-id="df8b4-139">boolean</span><span class="sxs-lookup"><span data-stu-id="df8b4-139">boolean</span></span>|<span data-ttu-id="df8b4-p105">省略可能。範囲にヘッダーがあるかどうか。</span><span class="sxs-lookup"><span data-stu-id="df8b4-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="df8b4-142">orientation</span><span class="sxs-lookup"><span data-stu-id="df8b4-142">orientation</span></span>|<span data-ttu-id="df8b4-143">string</span><span class="sxs-lookup"><span data-stu-id="df8b4-143">string</span></span>|<span data-ttu-id="df8b4-p106">省略可能。操作が行と列のどちらの並べ替えかを示します。可能な値は、`Rows`、`Columns` です。</span><span class="sxs-lookup"><span data-stu-id="df8b4-p106">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="df8b4-147">method</span><span class="sxs-lookup"><span data-stu-id="df8b4-147">method</span></span>|<span data-ttu-id="df8b4-148">string</span><span class="sxs-lookup"><span data-stu-id="df8b4-148">string</span></span>|<span data-ttu-id="df8b4-p107">省略可能。中国語文字に使用される順序付けの方法です。可能な値は、`PinYin`、`StrokeCount` です。</span><span class="sxs-lookup"><span data-stu-id="df8b4-p107">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="df8b4-152">応答</span><span class="sxs-lookup"><span data-stu-id="df8b4-152">Response</span></span>

<span data-ttu-id="df8b4-p108">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="df8b4-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df8b4-155">例</span><span class="sxs-lookup"><span data-stu-id="df8b4-155">Example</span></span>
<span data-ttu-id="df8b4-156">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="df8b4-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="df8b4-157">要求</span><span class="sxs-lookup"><span data-stu-id="df8b4-157">Request</span></span>
<span data-ttu-id="df8b4-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="df8b4-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
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

##### <a name="response"></a><span data-ttu-id="df8b4-159">応答</span><span class="sxs-lookup"><span data-stu-id="df8b4-159">Response</span></span>
<span data-ttu-id="df8b4-160">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="df8b4-160">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
