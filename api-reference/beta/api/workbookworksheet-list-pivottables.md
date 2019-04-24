---
title: pivotTables を一覧表示する
description: workbookpivottable オブジェクトの一覧を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 05b0039178b602a7f5b757561693d8afb1b6c569
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461165"
---
# <a name="list-pivottables"></a><span data-ttu-id="784de-103">pivotTables を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="784de-103">List pivotTables</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="784de-104">workbookpivottable オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="784de-104">Retrieve a list of workbookpivottable objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="784de-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="784de-105">Permissions</span></span>
<span data-ttu-id="784de-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="784de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="784de-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="784de-108">Permission type</span></span>      | <span data-ttu-id="784de-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="784de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="784de-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="784de-110">Delegated (work or school account)</span></span> | <span data-ttu-id="784de-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="784de-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="784de-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="784de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="784de-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="784de-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="784de-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="784de-114">Application</span></span> | <span data-ttu-id="784de-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="784de-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="784de-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="784de-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="784de-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="784de-117">Optional query parameters</span></span>
<span data-ttu-id="784de-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="784de-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="784de-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="784de-119">Request headers</span></span>
| <span data-ttu-id="784de-120">名前</span><span class="sxs-lookup"><span data-stu-id="784de-120">Name</span></span>      |<span data-ttu-id="784de-121">説明</span><span class="sxs-lookup"><span data-stu-id="784de-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="784de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="784de-122">Authorization</span></span>  | <span data-ttu-id="784de-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="784de-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="784de-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="784de-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="784de-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="784de-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="784de-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="784de-128">Request body</span></span>
<span data-ttu-id="784de-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="784de-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="784de-130">応答</span><span class="sxs-lookup"><span data-stu-id="784de-130">Response</span></span>

<span data-ttu-id="784de-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookPivotTable](../resources/workbookpivottable.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="784de-131">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="784de-132">例</span><span class="sxs-lookup"><span data-stu-id="784de-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="784de-133">要求</span><span class="sxs-lookup"><span data-stu-id="784de-133">Request</span></span>
<span data-ttu-id="784de-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="784de-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_pivottables"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables
```
##### <a name="response"></a><span data-ttu-id="784de-135">応答</span><span class="sxs-lookup"><span data-stu-id="784de-135">Response</span></span>
<span data-ttu-id="784de-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="784de-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookworksheet-list-pivottables.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
