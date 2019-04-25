---
title: 'workbookRangeView: range'
description: rangeView リソースに関連付けられている範囲を返します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b6a1b678b77cf4bd4d20d9d3d0a68178dbc07151
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535986"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="52f53-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="52f53-103">workbookRangeView: range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52f53-104">rangeView リソースに関連付けられている範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="52f53-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="52f53-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="52f53-105">Permissions</span></span>
<span data-ttu-id="52f53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52f53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="52f53-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52f53-108">Permission type</span></span>      | <span data-ttu-id="52f53-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52f53-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52f53-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52f53-110">Delegated (work or school account)</span></span> | <span data-ttu-id="52f53-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52f53-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52f53-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52f53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52f53-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52f53-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52f53-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52f53-114">Application</span></span> | <span data-ttu-id="52f53-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52f53-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52f53-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52f53-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="52f53-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52f53-117">Request headers</span></span>
| <span data-ttu-id="52f53-118">名前</span><span class="sxs-lookup"><span data-stu-id="52f53-118">Name</span></span>       | <span data-ttu-id="52f53-119">説明</span><span class="sxs-lookup"><span data-stu-id="52f53-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="52f53-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="52f53-120">Authorization</span></span>  | <span data-ttu-id="52f53-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="52f53-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52f53-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="52f53-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="52f53-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="52f53-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52f53-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="52f53-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="52f53-127">応答</span><span class="sxs-lookup"><span data-stu-id="52f53-127">Response</span></span>

<span data-ttu-id="52f53-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="52f53-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52f53-129">例</span><span class="sxs-lookup"><span data-stu-id="52f53-129">Example</span></span>
<span data-ttu-id="52f53-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="52f53-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="52f53-131">要求</span><span class="sxs-lookup"><span data-stu-id="52f53-131">Request</span></span>
<span data-ttu-id="52f53-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="52f53-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="52f53-133">応答</span><span class="sxs-lookup"><span data-stu-id="52f53-133">Response</span></span>
<span data-ttu-id="52f53-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="52f53-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrangeview-range.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
