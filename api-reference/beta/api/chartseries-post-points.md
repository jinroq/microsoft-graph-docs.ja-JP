---
title: Create ChartPoints
description: この API を使用して、新しい ChartPoints を作成します。
author: lumine2008
ms.openlocfilehash: bc6d386b7508e98797fbaa79f9b79d066918518a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311579"
---
# <a name="create-chartpoints"></a><span data-ttu-id="42b4b-103">Create ChartPoints</span><span class="sxs-lookup"><span data-stu-id="42b4b-103">Create ChartPoints</span></span>

> <span data-ttu-id="42b4b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="42b4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42b4b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42b4b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42b4b-106">この API を使用して、新しい ChartPoints を作成します。</span><span class="sxs-lookup"><span data-stu-id="42b4b-106">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="42b4b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="42b4b-107">Permissions</span></span>
<span data-ttu-id="42b4b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42b4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42b4b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="42b4b-110">Permission type</span></span>      | <span data-ttu-id="42b4b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="42b4b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42b4b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="42b4b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="42b4b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42b4b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42b4b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="42b4b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42b4b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42b4b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42b4b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="42b4b-116">Application</span></span> | <span data-ttu-id="42b4b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42b4b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42b4b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="42b4b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="42b4b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42b4b-119">Request headers</span></span>
| <span data-ttu-id="42b4b-120">名前</span><span class="sxs-lookup"><span data-stu-id="42b4b-120">Name</span></span>       | <span data-ttu-id="42b4b-121">説明</span><span class="sxs-lookup"><span data-stu-id="42b4b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42b4b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42b4b-122">Authorization</span></span>  | <span data-ttu-id="42b4b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="42b4b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42b4b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="42b4b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="42b4b-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="42b4b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42b4b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="42b4b-128">Request body</span></span>
<span data-ttu-id="42b4b-129">要求本文で、[ChartPoints](../resources/chartpoint.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="42b4b-129">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="42b4b-130">応答</span><span class="sxs-lookup"><span data-stu-id="42b4b-130">Response</span></span>

<span data-ttu-id="42b4b-131">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [ChartPoints](../resources/chartpoint.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="42b4b-131">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42b4b-132">例</span><span class="sxs-lookup"><span data-stu-id="42b4b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42b4b-133">要求</span><span class="sxs-lookup"><span data-stu-id="42b4b-133">Request</span></span>
<span data-ttu-id="42b4b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="42b4b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="42b4b-135">要求本文で、[ChartPoints](../resources/chartpoint.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="42b4b-135">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="42b4b-136">応答</span><span class="sxs-lookup"><span data-stu-id="42b4b-136">Response</span></span>
<span data-ttu-id="42b4b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="42b4b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->