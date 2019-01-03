---
title: workbookPivotTable を取得する
description: workbookPivotTable オブジェクトのプロパティと関係を取得します。
author: lumine2008
ms.openlocfilehash: 00f994fcbffeb8214a6326130746c0200c162107
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344892"
---
# <a name="get-workbookpivottable"></a><span data-ttu-id="3a477-103">workbookPivotTable を取得する</span><span class="sxs-lookup"><span data-stu-id="3a477-103">Get workbookPivotTable</span></span>

> <span data-ttu-id="3a477-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3a477-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a477-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a477-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a477-106">workbookPivotTable オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="3a477-106">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a477-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3a477-107">Permissions</span></span>
<span data-ttu-id="3a477-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a477-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3a477-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a477-110">Permission type</span></span>      | <span data-ttu-id="3a477-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a477-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a477-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a477-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a477-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a477-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a477-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a477-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a477-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a477-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a477-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a477-116">Application</span></span> | <span data-ttu-id="3a477-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a477-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a477-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a477-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a477-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a477-119">Optional query parameters</span></span>
<span data-ttu-id="3a477-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3a477-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a477-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a477-121">Request headers</span></span>
| <span data-ttu-id="3a477-122">名前</span><span class="sxs-lookup"><span data-stu-id="3a477-122">Name</span></span>      |<span data-ttu-id="3a477-123">説明</span><span class="sxs-lookup"><span data-stu-id="3a477-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a477-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a477-124">Authorization</span></span>  | <span data-ttu-id="3a477-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3a477-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a477-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3a477-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="3a477-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3a477-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a477-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a477-130">Request body</span></span>
<span data-ttu-id="3a477-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3a477-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a477-132">応答</span><span class="sxs-lookup"><span data-stu-id="3a477-132">Response</span></span>

<span data-ttu-id="3a477-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookPivotTable](../resources/workbookpivottable.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3a477-133">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a477-134">例</span><span class="sxs-lookup"><span data-stu-id="3a477-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a477-135">要求</span><span class="sxs-lookup"><span data-stu-id="3a477-135">Request</span></span>
<span data-ttu-id="3a477-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a477-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="3a477-137">応答</span><span class="sxs-lookup"><span data-stu-id="3a477-137">Response</span></span>
<span data-ttu-id="3a477-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3a477-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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