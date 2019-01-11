---
title: FormatProtection の取得
description: formatprotection オブジェクトのプロパティと関係を読み取ります。
localization_priority: Normal
ms.openlocfilehash: c8588e6fc33c1fe5b1bf761a6408b1e3d2f77b8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883700"
---
# <a name="get-formatprotection"></a><span data-ttu-id="5c575-103">FormatProtection の取得</span><span class="sxs-lookup"><span data-stu-id="5c575-103">Get FormatProtection</span></span>

> <span data-ttu-id="5c575-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5c575-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c575-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c575-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c575-106">formatprotection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5c575-106">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c575-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5c575-107">Permissions</span></span>
<span data-ttu-id="5c575-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c575-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c575-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c575-110">Permission type</span></span>      | <span data-ttu-id="5c575-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c575-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c575-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c575-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5c575-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c575-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c575-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c575-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c575-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c575-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c575-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c575-116">Application</span></span> | <span data-ttu-id="5c575-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c575-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c575-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c575-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5c575-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5c575-119">Optional query parameters</span></span>
<span data-ttu-id="5c575-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5c575-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c575-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c575-121">Request headers</span></span>
| <span data-ttu-id="5c575-122">名前</span><span class="sxs-lookup"><span data-stu-id="5c575-122">Name</span></span>      |<span data-ttu-id="5c575-123">説明</span><span class="sxs-lookup"><span data-stu-id="5c575-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c575-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c575-124">Authorization</span></span>  | <span data-ttu-id="5c575-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5c575-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c575-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c575-127">Request body</span></span>
<span data-ttu-id="5c575-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5c575-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c575-129">応答</span><span class="sxs-lookup"><span data-stu-id="5c575-129">Response</span></span>

<span data-ttu-id="5c575-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [FormatProtection](../resources/formatprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5c575-130">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c575-131">例</span><span class="sxs-lookup"><span data-stu-id="5c575-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c575-132">要求</span><span class="sxs-lookup"><span data-stu-id="5c575-132">Request</span></span>
<span data-ttu-id="5c575-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5c575-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="5c575-134">応答</span><span class="sxs-lookup"><span data-stu-id="5c575-134">Response</span></span>
<span data-ttu-id="5c575-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5c575-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
