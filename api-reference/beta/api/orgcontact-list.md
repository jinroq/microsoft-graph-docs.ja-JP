---
title: リスト orgContacts
description: この組織の組織の連絡先の一覧を取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 53cfa75edeb1994cabc1f363dab79455b90ce921
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915075"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="65b44-103">リスト orgContacts</span><span class="sxs-lookup"><span data-stu-id="65b44-103">List orgContacts</span></span>

> <span data-ttu-id="65b44-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65b44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65b44-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65b44-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65b44-106">この組織の組織の連絡先の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="65b44-106">Retrieve the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="65b44-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65b44-107">Permissions</span></span>
<span data-ttu-id="65b44-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65b44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65b44-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65b44-110">Permission type</span></span>      | <span data-ttu-id="65b44-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65b44-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65b44-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65b44-112">Delegated (work or school account)</span></span> | <span data-ttu-id="65b44-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65b44-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65b44-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65b44-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65b44-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65b44-115">Not supported.</span></span>    |
|<span data-ttu-id="65b44-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65b44-116">Application</span></span> | <span data-ttu-id="65b44-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65b44-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65b44-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65b44-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65b44-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="65b44-119">Optional query parameters</span></span>
<span data-ttu-id="65b44-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="65b44-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65b44-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65b44-121">Request headers</span></span>
| <span data-ttu-id="65b44-122">名前</span><span class="sxs-lookup"><span data-stu-id="65b44-122">Name</span></span>       | <span data-ttu-id="65b44-123">種類</span><span class="sxs-lookup"><span data-stu-id="65b44-123">Type</span></span> | <span data-ttu-id="65b44-124">説明</span><span class="sxs-lookup"><span data-stu-id="65b44-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65b44-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="65b44-125">Authorization</span></span>  | <span data-ttu-id="65b44-126">string</span><span class="sxs-lookup"><span data-stu-id="65b44-126">string</span></span>  | <span data-ttu-id="65b44-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="65b44-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65b44-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="65b44-129">Request body</span></span>
<span data-ttu-id="65b44-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="65b44-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65b44-131">応答</span><span class="sxs-lookup"><span data-stu-id="65b44-131">Response</span></span>

<span data-ttu-id="65b44-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[orgContact](../resources/orgcontact.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="65b44-132">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65b44-133">例</span><span class="sxs-lookup"><span data-stu-id="65b44-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65b44-134">要求</span><span class="sxs-lookup"><span data-stu-id="65b44-134">Request</span></span>
<span data-ttu-id="65b44-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65b44-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts
```
##### <a name="response"></a><span data-ttu-id="65b44-136">応答</span><span class="sxs-lookup"><span data-stu-id="65b44-136">Response</span></span>
<span data-ttu-id="65b44-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65b44-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
