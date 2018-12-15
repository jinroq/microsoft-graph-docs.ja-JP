---
title: OrgContact を取得します。
description: プロパティと orgcontact オブジェクトの関係を取得します。
ms.openlocfilehash: 9297297bf341d622070c6ca200d99087588a8ce6
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283613"
---
# <a name="get-orgcontact"></a><span data-ttu-id="95d98-103">OrgContact を取得します。</span><span class="sxs-lookup"><span data-stu-id="95d98-103">Get orgContact</span></span>

> <span data-ttu-id="95d98-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95d98-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95d98-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95d98-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95d98-106">プロパティと orgcontact オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="95d98-106">Retrieve the properties and relationships of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="95d98-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="95d98-107">Permissions</span></span>
<span data-ttu-id="95d98-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95d98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95d98-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95d98-110">Permission type</span></span>      | <span data-ttu-id="95d98-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="95d98-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95d98-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95d98-112">Delegated (work or school account)</span></span> | <span data-ttu-id="95d98-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="95d98-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="95d98-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95d98-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95d98-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95d98-115">Not supported.</span></span>    |
|<span data-ttu-id="95d98-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95d98-116">Application</span></span> | <span data-ttu-id="95d98-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95d98-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95d98-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95d98-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="95d98-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="95d98-119">Optional query parameters</span></span>
<span data-ttu-id="95d98-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="95d98-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95d98-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95d98-121">Request headers</span></span>
| <span data-ttu-id="95d98-122">名前</span><span class="sxs-lookup"><span data-stu-id="95d98-122">Name</span></span>       | <span data-ttu-id="95d98-123">種類</span><span class="sxs-lookup"><span data-stu-id="95d98-123">Type</span></span> | <span data-ttu-id="95d98-124">説明</span><span class="sxs-lookup"><span data-stu-id="95d98-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="95d98-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="95d98-125">Authorization</span></span>  | <span data-ttu-id="95d98-126">string</span><span class="sxs-lookup"><span data-stu-id="95d98-126">string</span></span>  | <span data-ttu-id="95d98-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="95d98-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95d98-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="95d98-129">Request body</span></span>
<span data-ttu-id="95d98-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95d98-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95d98-131">応答</span><span class="sxs-lookup"><span data-stu-id="95d98-131">Response</span></span>

<span data-ttu-id="95d98-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[orgContact](../resources/orgcontact.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="95d98-132">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="95d98-133">例</span><span class="sxs-lookup"><span data-stu-id="95d98-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95d98-134">要求</span><span class="sxs-lookup"><span data-stu-id="95d98-134">Request</span></span>
<span data-ttu-id="95d98-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95d98-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="95d98-136">応答</span><span class="sxs-lookup"><span data-stu-id="95d98-136">Response</span></span>
<span data-ttu-id="95d98-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95d98-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->