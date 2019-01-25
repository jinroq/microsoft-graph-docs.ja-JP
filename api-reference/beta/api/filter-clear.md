---
title: 'フィルター: クリア'
description: 指定した列のフィルターをクリアします。
localization_priority: Normal
ms.openlocfilehash: 3567ee187a9b3becb1afa296c97cc7c3442bf667
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518038"
---
# <a name="filter-clear"></a><span data-ttu-id="36c4e-103">フィルター: クリア</span><span class="sxs-lookup"><span data-stu-id="36c4e-103">Filter: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36c4e-104">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="36c4e-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="36c4e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="36c4e-105">Permissions</span></span>
<span data-ttu-id="36c4e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36c4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36c4e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36c4e-108">Permission type</span></span>      | <span data-ttu-id="36c4e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="36c4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36c4e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36c4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36c4e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36c4e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36c4e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36c4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36c4e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36c4e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36c4e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36c4e-114">Application</span></span> | <span data-ttu-id="36c4e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36c4e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36c4e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36c4e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="36c4e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36c4e-117">Request headers</span></span>
| <span data-ttu-id="36c4e-118">名前</span><span class="sxs-lookup"><span data-stu-id="36c4e-118">Name</span></span>       | <span data-ttu-id="36c4e-119">説明</span><span class="sxs-lookup"><span data-stu-id="36c4e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="36c4e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="36c4e-120">Authorization</span></span>  | <span data-ttu-id="36c4e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="36c4e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36c4e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="36c4e-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="36c4e-124">応答</span><span class="sxs-lookup"><span data-stu-id="36c4e-124">Response</span></span>

<span data-ttu-id="36c4e-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="36c4e-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36c4e-127">例</span><span class="sxs-lookup"><span data-stu-id="36c4e-127">Example</span></span>
<span data-ttu-id="36c4e-128">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="36c4e-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="36c4e-129">要求</span><span class="sxs-lookup"><span data-stu-id="36c4e-129">Request</span></span>
<span data-ttu-id="36c4e-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36c4e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="36c4e-131">応答</span><span class="sxs-lookup"><span data-stu-id="36c4e-131">Response</span></span>
<span data-ttu-id="36c4e-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="36c4e-132">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/filter-clear.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
