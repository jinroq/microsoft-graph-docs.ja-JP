---
title: FormatProtection の取得
description: formatprotection オブジェクトのプロパティと関係を読み取ります。
localization_priority: Normal
ms.openlocfilehash: 88c220bef0536b9bc921a28441b2e80a47dc3025
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325040"
---
# <a name="get-formatprotection"></a><span data-ttu-id="c0ab0-103">FormatProtection の取得</span><span class="sxs-lookup"><span data-stu-id="c0ab0-103">Get FormatProtection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0ab0-104">formatprotection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c0ab0-104">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0ab0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c0ab0-105">Permissions</span></span>
<span data-ttu-id="c0ab0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0ab0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0ab0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0ab0-108">Permission type</span></span>      | <span data-ttu-id="c0ab0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0ab0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0ab0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0ab0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0ab0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0ab0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0ab0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0ab0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0ab0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0ab0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0ab0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0ab0-114">Application</span></span> | <span data-ttu-id="c0ab0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0ab0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0ab0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0ab0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0ab0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c0ab0-117">Optional query parameters</span></span>
<span data-ttu-id="c0ab0-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c0ab0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0ab0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0ab0-119">Request headers</span></span>
| <span data-ttu-id="c0ab0-120">名前</span><span class="sxs-lookup"><span data-stu-id="c0ab0-120">Name</span></span>      |<span data-ttu-id="c0ab0-121">説明</span><span class="sxs-lookup"><span data-stu-id="c0ab0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0ab0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0ab0-122">Authorization</span></span>  | <span data-ttu-id="c0ab0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c0ab0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0ab0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0ab0-125">Request body</span></span>
<span data-ttu-id="c0ab0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c0ab0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0ab0-127">応答</span><span class="sxs-lookup"><span data-stu-id="c0ab0-127">Response</span></span>

<span data-ttu-id="c0ab0-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [FormatProtection](../resources/formatprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c0ab0-128">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0ab0-129">例</span><span class="sxs-lookup"><span data-stu-id="c0ab0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0ab0-130">要求</span><span class="sxs-lookup"><span data-stu-id="c0ab0-130">Request</span></span>
<span data-ttu-id="c0ab0-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0ab0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="c0ab0-132">応答</span><span class="sxs-lookup"><span data-stu-id="c0ab0-132">Response</span></span>
<span data-ttu-id="c0ab0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0ab0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
