---
title: アイコンを取得する
description: アイコン オブジェクトのプロパティと関係を取得します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6ad126aa04f1d977ad065a9baaa2ce2cc2a72065
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014453"
---
# <a name="get-icon"></a><span data-ttu-id="369d3-103">アイコンを取得する</span><span class="sxs-lookup"><span data-stu-id="369d3-103">Get Icon</span></span>

<span data-ttu-id="369d3-104">アイコン オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="369d3-104">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="369d3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="369d3-105">Permissions</span></span>
<span data-ttu-id="369d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="369d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="369d3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="369d3-108">Permission type</span></span>      | <span data-ttu-id="369d3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="369d3-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="369d3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="369d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="369d3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="369d3-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="369d3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="369d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="369d3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="369d3-113">Not supported.</span></span>    | 
|<span data-ttu-id="369d3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="369d3-114">Application</span></span> | <span data-ttu-id="369d3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="369d3-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="369d3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="369d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="369d3-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="369d3-117">Optional query parameters</span></span>
<span data-ttu-id="369d3-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="369d3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="369d3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="369d3-119">Request headers</span></span>
| <span data-ttu-id="369d3-120">名前</span><span class="sxs-lookup"><span data-stu-id="369d3-120">Name</span></span>      |<span data-ttu-id="369d3-121">説明</span><span class="sxs-lookup"><span data-stu-id="369d3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="369d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="369d3-122">Authorization</span></span>  | <span data-ttu-id="369d3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="369d3-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="369d3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="369d3-125">Request body</span></span>
<span data-ttu-id="369d3-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="369d3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="369d3-127">応答</span><span class="sxs-lookup"><span data-stu-id="369d3-127">Response</span></span>

<span data-ttu-id="369d3-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アイコン](../resources/icon.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="369d3-128">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="369d3-129">例</span><span class="sxs-lookup"><span data-stu-id="369d3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="369d3-130">要求</span><span class="sxs-lookup"><span data-stu-id="369d3-130">Request</span></span>
<span data-ttu-id="369d3-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="369d3-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="369d3-132">応答</span><span class="sxs-lookup"><span data-stu-id="369d3-132">Response</span></span>
<span data-ttu-id="369d3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="369d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
