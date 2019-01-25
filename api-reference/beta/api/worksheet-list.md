---
title: WorksheetCollection を一覧表示する
description: ワークシート オブジェクトの一覧を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 585faae105955f24b80a64b834dba207f740d67a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530133"
---
# <a name="list-worksheetcollection"></a><span data-ttu-id="14e33-103">WorksheetCollection を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="14e33-103">List WorksheetCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14e33-104">ワークシート オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="14e33-104">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="14e33-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="14e33-105">Permissions</span></span>
<span data-ttu-id="14e33-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14e33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14e33-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="14e33-108">Permission type</span></span>      | <span data-ttu-id="14e33-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="14e33-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14e33-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="14e33-110">Delegated (work or school account)</span></span> | <span data-ttu-id="14e33-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14e33-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="14e33-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="14e33-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14e33-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14e33-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="14e33-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="14e33-114">Application</span></span> | <span data-ttu-id="14e33-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14e33-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14e33-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="14e33-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14e33-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="14e33-117">Optional query parameters</span></span>
<span data-ttu-id="14e33-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="14e33-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14e33-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14e33-119">Request headers</span></span>
| <span data-ttu-id="14e33-120">名前</span><span class="sxs-lookup"><span data-stu-id="14e33-120">Name</span></span>      |<span data-ttu-id="14e33-121">説明</span><span class="sxs-lookup"><span data-stu-id="14e33-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14e33-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="14e33-122">Authorization</span></span>  | <span data-ttu-id="14e33-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="14e33-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14e33-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="14e33-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="14e33-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="14e33-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14e33-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="14e33-128">Request body</span></span>
<span data-ttu-id="14e33-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="14e33-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14e33-130">応答</span><span class="sxs-lookup"><span data-stu-id="14e33-130">Response</span></span>

<span data-ttu-id="14e33-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Worksheet](../resources/worksheet.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="14e33-131">If successful, this method returns a `200 OK` response code and collection of [Worksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14e33-132">例</span><span class="sxs-lookup"><span data-stu-id="14e33-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14e33-133">要求</span><span class="sxs-lookup"><span data-stu-id="14e33-133">Request</span></span>
<span data-ttu-id="14e33-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="14e33-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheetcollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="14e33-135">応答</span><span class="sxs-lookup"><span data-stu-id="14e33-135">Response</span></span>
<span data-ttu-id="14e33-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="14e33-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List WorksheetCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
