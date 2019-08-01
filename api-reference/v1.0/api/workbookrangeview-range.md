---
title: 'workbookRangeView: range'
description: rangeView リソースに関連付けられている範囲を返します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 71c2a27326d67adf25268717af5e927ac6f88570
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026312"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="36b1c-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="36b1c-103">workbookRangeView: range</span></span>
<span data-ttu-id="36b1c-104">rangeView リソースに関連付けられている範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="36b1c-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="36b1c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="36b1c-105">Permissions</span></span>
<span data-ttu-id="36b1c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36b1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="36b1c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36b1c-108">Permission type</span></span>      | <span data-ttu-id="36b1c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="36b1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36b1c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36b1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36b1c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36b1c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36b1c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36b1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36b1c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36b1c-113">Not supported.</span></span>    |
|<span data-ttu-id="36b1c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36b1c-114">Application</span></span> | <span data-ttu-id="36b1c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36b1c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36b1c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36b1c-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36b1c-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="36b1c-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="36b1c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36b1c-118">Request headers</span></span>
| <span data-ttu-id="36b1c-119">名前</span><span class="sxs-lookup"><span data-stu-id="36b1c-119">Name</span></span>       | <span data-ttu-id="36b1c-120">説明</span><span class="sxs-lookup"><span data-stu-id="36b1c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="36b1c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36b1c-121">Authorization</span></span>  | <span data-ttu-id="36b1c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="36b1c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36b1c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="36b1c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="36b1c-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="36b1c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36b1c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="36b1c-127">Request body</span></span>

### <a name="response"></a><span data-ttu-id="36b1c-128">応答</span><span class="sxs-lookup"><span data-stu-id="36b1c-128">Response</span></span>
<span data-ttu-id="36b1c-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="36b1c-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36b1c-130">例</span><span class="sxs-lookup"><span data-stu-id="36b1c-130">Example</span></span>
<span data-ttu-id="36b1c-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="36b1c-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="36b1c-132">要求</span><span class="sxs-lookup"><span data-stu-id="36b1c-132">Request</span></span>
<span data-ttu-id="36b1c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36b1c-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36b1c-134">C#</span><span class="sxs-lookup"><span data-stu-id="36b1c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36b1c-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="36b1c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36b1c-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="36b1c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="36b1c-137">Java</span><span class="sxs-lookup"><span data-stu-id="36b1c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrangeview-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36b1c-138">応答</span><span class="sxs-lookup"><span data-stu-id="36b1c-138">Response</span></span>
<span data-ttu-id="36b1c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36b1c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
