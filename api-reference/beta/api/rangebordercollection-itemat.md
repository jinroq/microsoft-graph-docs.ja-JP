---
title: 'RangeBorderCollection: ItemAt'
description: オブジェクトのインデックスを使用して、境界線オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f0308049046cd91484d996d2e3de84b007c89223
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524556"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="f76e3-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="f76e3-103">RangeBorderCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f76e3-104">オブジェクトのインデックスを使用して、境界線オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="f76e3-104">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="f76e3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f76e3-105">Permissions</span></span>
<span data-ttu-id="f76e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f76e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f76e3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f76e3-108">Permission type</span></span>      | <span data-ttu-id="f76e3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f76e3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f76e3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f76e3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f76e3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f76e3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f76e3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f76e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f76e3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f76e3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f76e3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f76e3-114">Application</span></span> | <span data-ttu-id="f76e3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f76e3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f76e3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f76e3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders/ItemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="f76e3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f76e3-117">Request headers</span></span>
| <span data-ttu-id="f76e3-118">名前</span><span class="sxs-lookup"><span data-stu-id="f76e3-118">Name</span></span>       | <span data-ttu-id="f76e3-119">説明</span><span class="sxs-lookup"><span data-stu-id="f76e3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f76e3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f76e3-120">Authorization</span></span>  | <span data-ttu-id="f76e3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f76e3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f76e3-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f76e3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f76e3-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f76e3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f76e3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f76e3-126">Request body</span></span>
<span data-ttu-id="f76e3-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f76e3-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f76e3-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f76e3-128">Parameter</span></span>    | <span data-ttu-id="f76e3-129">型</span><span class="sxs-lookup"><span data-stu-id="f76e3-129">Type</span></span>   |<span data-ttu-id="f76e3-130">説明</span><span class="sxs-lookup"><span data-stu-id="f76e3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f76e3-131">index</span><span class="sxs-lookup"><span data-stu-id="f76e3-131">index</span></span>|<span data-ttu-id="f76e3-132">number</span><span class="sxs-lookup"><span data-stu-id="f76e3-132">number</span></span>|<span data-ttu-id="f76e3-p104">取得するオブジェクトのインデックス値。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="f76e3-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="f76e3-135">応答</span><span class="sxs-lookup"><span data-stu-id="f76e3-135">Response</span></span>

<span data-ttu-id="f76e3-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [RangeBorder](../resources/rangeborder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f76e3-136">If successful, this method returns `200 OK` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f76e3-137">例</span><span class="sxs-lookup"><span data-stu-id="f76e3-137">Example</span></span>
<span data-ttu-id="f76e3-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f76e3-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f76e3-139">要求</span><span class="sxs-lookup"><span data-stu-id="f76e3-139">Request</span></span>
<span data-ttu-id="f76e3-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f76e3-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="f76e3-141">応答</span><span class="sxs-lookup"><span data-stu-id="f76e3-141">Response</span></span>
<span data-ttu-id="f76e3-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f76e3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangebordercollection-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
