---
title: アイコンを取得する
description: アイコン オブジェクトのプロパティと関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 8d5f7f88892492230d2e77d587dc7f45b863f163
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869105"
---
# <a name="get-icon"></a><span data-ttu-id="a27cf-103">アイコンを取得する</span><span class="sxs-lookup"><span data-stu-id="a27cf-103">Get Icon</span></span>

<span data-ttu-id="a27cf-104">アイコン オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="a27cf-104">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a27cf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a27cf-105">Permissions</span></span>
<span data-ttu-id="a27cf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a27cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a27cf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a27cf-108">Permission type</span></span>      | <span data-ttu-id="a27cf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a27cf-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="a27cf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a27cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a27cf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a27cf-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="a27cf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a27cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a27cf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a27cf-113">Not supported.</span></span>    | 
|<span data-ttu-id="a27cf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a27cf-114">Application</span></span> | <span data-ttu-id="a27cf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a27cf-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a27cf-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a27cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a27cf-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a27cf-117">Optional query parameters</span></span>
<span data-ttu-id="a27cf-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a27cf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a27cf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a27cf-119">Request headers</span></span>
| <span data-ttu-id="a27cf-120">名前</span><span class="sxs-lookup"><span data-stu-id="a27cf-120">Name</span></span>      |<span data-ttu-id="a27cf-121">説明</span><span class="sxs-lookup"><span data-stu-id="a27cf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a27cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a27cf-122">Authorization</span></span>  | <span data-ttu-id="a27cf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a27cf-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a27cf-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a27cf-125">Request body</span></span>
<span data-ttu-id="a27cf-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a27cf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a27cf-127">応答</span><span class="sxs-lookup"><span data-stu-id="a27cf-127">Response</span></span>

<span data-ttu-id="a27cf-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アイコン](../resources/icon.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a27cf-128">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a27cf-129">例</span><span class="sxs-lookup"><span data-stu-id="a27cf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a27cf-130">要求</span><span class="sxs-lookup"><span data-stu-id="a27cf-130">Request</span></span>
<span data-ttu-id="a27cf-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a27cf-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="a27cf-132">応答</span><span class="sxs-lookup"><span data-stu-id="a27cf-132">Response</span></span>
<span data-ttu-id="a27cf-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a27cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
