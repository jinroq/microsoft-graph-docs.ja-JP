---
title: リスト orgContacts
description: この組織の組織の連絡先の一覧を取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b8a3549a6933cbc6b965b2c708cc7275c3744f36
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516638"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="1ef1d-103">リスト orgContacts</span><span class="sxs-lookup"><span data-stu-id="1ef1d-103">List orgContacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ef1d-104">この組織の組織の連絡先の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1ef1d-104">Retrieve the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ef1d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ef1d-105">Permissions</span></span>
<span data-ttu-id="1ef1d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ef1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ef1d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ef1d-108">Permission type</span></span>      | <span data-ttu-id="1ef1d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ef1d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ef1d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ef1d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ef1d-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1ef1d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1ef1d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ef1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ef1d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ef1d-113">Not supported.</span></span>    |
|<span data-ttu-id="1ef1d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ef1d-114">Application</span></span> | <span data-ttu-id="1ef1d-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ef1d-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ef1d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ef1d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1ef1d-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1ef1d-117">Optional query parameters</span></span>
<span data-ttu-id="1ef1d-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1ef1d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ef1d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ef1d-119">Request headers</span></span>
| <span data-ttu-id="1ef1d-120">名前</span><span class="sxs-lookup"><span data-stu-id="1ef1d-120">Name</span></span>       | <span data-ttu-id="1ef1d-121">型</span><span class="sxs-lookup"><span data-stu-id="1ef1d-121">Type</span></span> | <span data-ttu-id="1ef1d-122">説明</span><span class="sxs-lookup"><span data-stu-id="1ef1d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1ef1d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ef1d-123">Authorization</span></span>  | <span data-ttu-id="1ef1d-124">string</span><span class="sxs-lookup"><span data-stu-id="1ef1d-124">string</span></span>  | <span data-ttu-id="1ef1d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1ef1d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ef1d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ef1d-127">Request body</span></span>
<span data-ttu-id="1ef1d-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1ef1d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ef1d-129">応答</span><span class="sxs-lookup"><span data-stu-id="1ef1d-129">Response</span></span>

<span data-ttu-id="1ef1d-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[orgContact](../resources/orgcontact.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1ef1d-130">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ef1d-131">例</span><span class="sxs-lookup"><span data-stu-id="1ef1d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ef1d-132">要求</span><span class="sxs-lookup"><span data-stu-id="1ef1d-132">Request</span></span>
<span data-ttu-id="1ef1d-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1ef1d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts
```
##### <a name="response"></a><span data-ttu-id="1ef1d-134">応答</span><span class="sxs-lookup"><span data-stu-id="1ef1d-134">Response</span></span>
<span data-ttu-id="1ef1d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1ef1d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
