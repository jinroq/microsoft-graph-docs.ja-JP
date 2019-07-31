---
title: rangeView 行を一覧表示する
description: 範囲ビュー オブジェクトの一覧を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fef2dfa9f6a1540868b7f22365a489ea34516ee2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995847"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="39111-103">rangeView 行を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="39111-103">List rangeView rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39111-104">範囲ビュー オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="39111-104">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="39111-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="39111-105">Permissions</span></span>
<span data-ttu-id="39111-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="39111-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39111-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="39111-108">Permission type</span></span>      | <span data-ttu-id="39111-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="39111-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39111-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="39111-110">Delegated (work or school account)</span></span> | <span data-ttu-id="39111-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39111-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39111-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="39111-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39111-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39111-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39111-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="39111-114">Application</span></span> | <span data-ttu-id="39111-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39111-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39111-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="39111-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="39111-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="39111-117">Optional query parameters</span></span>
<span data-ttu-id="39111-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="39111-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39111-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="39111-119">Request headers</span></span>
| <span data-ttu-id="39111-120">名前</span><span class="sxs-lookup"><span data-stu-id="39111-120">Name</span></span>      |<span data-ttu-id="39111-121">説明</span><span class="sxs-lookup"><span data-stu-id="39111-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39111-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="39111-122">Authorization</span></span>  | <span data-ttu-id="39111-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="39111-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39111-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="39111-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="39111-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="39111-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39111-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="39111-128">Request body</span></span>
<span data-ttu-id="39111-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="39111-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39111-130">応答</span><span class="sxs-lookup"><span data-stu-id="39111-130">Response</span></span>

<span data-ttu-id="39111-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRangeView](../resources/workbookrangeview.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="39111-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="39111-132">例</span><span class="sxs-lookup"><span data-stu-id="39111-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39111-133">要求</span><span class="sxs-lookup"><span data-stu-id="39111-133">Request</span></span>
<span data-ttu-id="39111-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="39111-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/rows 
```
##### <a name="response"></a><span data-ttu-id="39111-135">応答</span><span class="sxs-lookup"><span data-stu-id="39111-135">Response</span></span>
<span data-ttu-id="39111-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="39111-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
