---
title: orgcontact の取得
description: orgcontact へオブジェクトのプロパティと関係を取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 68cb9953eed91cd00fd699f20817ea1231e16b92
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539996"
---
# <a name="get-orgcontact"></a><span data-ttu-id="66f87-103">orgcontact の取得</span><span class="sxs-lookup"><span data-stu-id="66f87-103">Get orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66f87-104">orgcontact へオブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="66f87-104">Retrieve the properties and relationships of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="66f87-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66f87-105">Permissions</span></span>
<span data-ttu-id="66f87-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66f87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66f87-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66f87-108">Permission type</span></span>      | <span data-ttu-id="66f87-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66f87-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66f87-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66f87-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66f87-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66f87-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66f87-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66f87-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66f87-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66f87-113">Not supported.</span></span>    |
|<span data-ttu-id="66f87-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66f87-114">Application</span></span> | <span data-ttu-id="66f87-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66f87-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66f87-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66f87-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66f87-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="66f87-117">Optional query parameters</span></span>
<span data-ttu-id="66f87-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="66f87-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66f87-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66f87-119">Request headers</span></span>
| <span data-ttu-id="66f87-120">名前</span><span class="sxs-lookup"><span data-stu-id="66f87-120">Name</span></span>       | <span data-ttu-id="66f87-121">型</span><span class="sxs-lookup"><span data-stu-id="66f87-121">Type</span></span> | <span data-ttu-id="66f87-122">説明</span><span class="sxs-lookup"><span data-stu-id="66f87-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66f87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66f87-123">Authorization</span></span>  | <span data-ttu-id="66f87-124">string</span><span class="sxs-lookup"><span data-stu-id="66f87-124">string</span></span>  | <span data-ttu-id="66f87-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66f87-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66f87-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="66f87-127">Request body</span></span>
<span data-ttu-id="66f87-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="66f87-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66f87-129">応答</span><span class="sxs-lookup"><span data-stu-id="66f87-129">Response</span></span>

<span data-ttu-id="66f87-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[orgcontact](../resources/orgcontact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="66f87-130">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66f87-131">例</span><span class="sxs-lookup"><span data-stu-id="66f87-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66f87-132">要求</span><span class="sxs-lookup"><span data-stu-id="66f87-132">Request</span></span>
<span data-ttu-id="66f87-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66f87-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="66f87-134">応答</span><span class="sxs-lookup"><span data-stu-id="66f87-134">Response</span></span>
<span data-ttu-id="66f87-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66f87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "addresses":[
      {
        "city": "string",
        "countryOrRegion": "string",
        "officeLocation": "string",
        "postalCode": "string",
        "state": "string",
        "street": "string"
      }
  ],
  "companyName": "companyName-value",
  "department": "department-value",
  "displayName": "displayName-value",
  "phones":[
      {
        "type": "string",
        "number": "string"
      }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
