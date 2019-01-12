---
title: workbookPivotTable を取得する
description: workbookPivotTable オブジェクトのプロパティと関係を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: af32cfb118b8752e2598eaec1ca3b401e340bcc9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934353"
---
# <a name="get-workbookpivottable"></a><span data-ttu-id="08c00-103">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="08c00-103">Get workbookPivotTable</span></span>

<span data-ttu-id="08c00-104">workbookPivotTable オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="08c00-104">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="08c00-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08c00-105">Permissions</span></span>
<span data-ttu-id="08c00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08c00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="08c00-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08c00-108">Permission type</span></span>      | <span data-ttu-id="08c00-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08c00-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08c00-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08c00-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08c00-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08c00-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="08c00-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08c00-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08c00-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08c00-113">Not supported.</span></span>    |
|<span data-ttu-id="08c00-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08c00-114">Application</span></span> | <span data-ttu-id="08c00-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08c00-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08c00-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08c00-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="08c00-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="08c00-117">Optional query parameters</span></span>
<span data-ttu-id="08c00-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08c00-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08c00-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08c00-119">Request headers</span></span>
| <span data-ttu-id="08c00-120">名前</span><span class="sxs-lookup"><span data-stu-id="08c00-120">Name</span></span>      |<span data-ttu-id="08c00-121">説明</span><span class="sxs-lookup"><span data-stu-id="08c00-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08c00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08c00-122">Authorization</span></span>  | <span data-ttu-id="08c00-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08c00-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08c00-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="08c00-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="08c00-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="08c00-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08c00-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="08c00-128">Request body</span></span>
<span data-ttu-id="08c00-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="08c00-129">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="08c00-130">応答</span><span class="sxs-lookup"><span data-stu-id="08c00-130">Response</span></span>
<span data-ttu-id="08c00-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookPivotTable](../resources/workbookpivottable.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="08c00-131">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08c00-132">例</span><span class="sxs-lookup"><span data-stu-id="08c00-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08c00-133">要求</span><span class="sxs-lookup"><span data-stu-id="08c00-133">Request</span></span>
<span data-ttu-id="08c00-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="08c00-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="08c00-135">応答</span><span class="sxs-lookup"><span data-stu-id="08c00-135">Response</span></span>
<span data-ttu-id="08c00-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="08c00-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```
