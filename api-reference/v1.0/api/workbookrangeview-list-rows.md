---
title: rangeView 行を一覧表示する
description: 範囲ビュー オブジェクトの一覧を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 36e7c93133dd4298aa53898d05557cb88ca127c0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951277"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="c369c-103">rangeView 行を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c369c-103">List rangeView rows</span></span>

<span data-ttu-id="c369c-104">範囲ビュー オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c369c-104">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c369c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c369c-105">Permissions</span></span>
<span data-ttu-id="c369c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c369c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c369c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c369c-108">Permission type</span></span>      | <span data-ttu-id="c369c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c369c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c369c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c369c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c369c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c369c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c369c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c369c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c369c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c369c-113">Not supported.</span></span>    |
|<span data-ttu-id="c369c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c369c-114">Application</span></span> | <span data-ttu-id="c369c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c369c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c369c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c369c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="c369c-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c369c-117">Optional query parameters</span></span>
<span data-ttu-id="c369c-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c369c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c369c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c369c-119">Request headers</span></span>
| <span data-ttu-id="c369c-120">名前</span><span class="sxs-lookup"><span data-stu-id="c369c-120">Name</span></span>      |<span data-ttu-id="c369c-121">説明</span><span class="sxs-lookup"><span data-stu-id="c369c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c369c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c369c-122">Authorization</span></span>  | <span data-ttu-id="c369c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c369c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c369c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c369c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c369c-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c369c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c369c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c369c-128">Request body</span></span>
<span data-ttu-id="c369c-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c369c-129">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="c369c-130">応答</span><span class="sxs-lookup"><span data-stu-id="c369c-130">Response</span></span>
<span data-ttu-id="c369c-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRangeView](../resources/workbookrangeview.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c369c-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c369c-132">例</span><span class="sxs-lookup"><span data-stu-id="c369c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c369c-133">要求</span><span class="sxs-lookup"><span data-stu-id="c369c-133">Request</span></span>
<span data-ttu-id="c369c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c369c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows
```
##### <a name="response"></a><span data-ttu-id="c369c-135">応答</span><span class="sxs-lookup"><span data-stu-id="c369c-135">Response</span></span>
<span data-ttu-id="c369c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c369c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c369c-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="c369c-139">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c369c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c369c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_rows-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="c369c-141">C#</span><span class="sxs-lookup"><span data-stu-id="c369c-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_rows-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbookrangeview-list-rows.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrangeview-list-rows.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
