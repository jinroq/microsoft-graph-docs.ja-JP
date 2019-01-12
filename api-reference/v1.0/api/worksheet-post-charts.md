---
title: グラフを作成します。
description: この API を使用して、新しいグラフを作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dbef3e97651d5b65b64488f308212ff0fe2d89b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915614"
---
# <a name="create-chart"></a><span data-ttu-id="f76ca-103">グラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="f76ca-103">Create Chart</span></span>

<span data-ttu-id="f76ca-104">この API を使用して、新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="f76ca-104">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="f76ca-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f76ca-105">Permissions</span></span>
<span data-ttu-id="f76ca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f76ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f76ca-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f76ca-108">Permission type</span></span>      | <span data-ttu-id="f76ca-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f76ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f76ca-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f76ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f76ca-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f76ca-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f76ca-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f76ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f76ca-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f76ca-113">Not supported.</span></span>    |
|<span data-ttu-id="f76ca-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f76ca-114">Application</span></span> | <span data-ttu-id="f76ca-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f76ca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f76ca-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f76ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="f76ca-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f76ca-117">Request headers</span></span>
| <span data-ttu-id="f76ca-118">名前</span><span class="sxs-lookup"><span data-stu-id="f76ca-118">Name</span></span>       | <span data-ttu-id="f76ca-119">説明</span><span class="sxs-lookup"><span data-stu-id="f76ca-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f76ca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f76ca-120">Authorization</span></span>  | <span data-ttu-id="f76ca-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f76ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f76ca-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f76ca-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f76ca-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f76ca-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f76ca-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f76ca-126">Request body</span></span>
<span data-ttu-id="f76ca-127">要求の本文には、 [WorkbookChart](../resources/chart.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="f76ca-127">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f76ca-128">応答</span><span class="sxs-lookup"><span data-stu-id="f76ca-128">Response</span></span>

<span data-ttu-id="f76ca-129">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[WorkbookChart](../resources/chart.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f76ca-129">If successful, this method returns `201 Created` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f76ca-130">例</span><span class="sxs-lookup"><span data-stu-id="f76ca-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f76ca-131">要求</span><span class="sxs-lookup"><span data-stu-id="f76ca-131">Request</span></span>
<span data-ttu-id="f76ca-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f76ca-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="f76ca-133">要求の本文には、 [WorkbookChart](../resources/chart.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="f76ca-133">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f76ca-134">応答</span><span class="sxs-lookup"><span data-stu-id="f76ca-134">Response</span></span>
<span data-ttu-id="f76ca-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f76ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
