---
title: クラスをリストする
description: 'すべてのクラス オブジェクトのリストを取得します。 '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 74639acd39ee6b11a7338692b23e5e14a7020eda
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823927"
---
# <a name="list-classes"></a><span data-ttu-id="5d4d6-103">クラスをリストする</span><span class="sxs-lookup"><span data-stu-id="5d4d6-103">List classes</span></span>

> <span data-ttu-id="5d4d6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d4d6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d4d6-106">すべてのクラス オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-106">Retrieve a list of all class objects.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5d4d6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5d4d6-107">Permissions</span></span>
<span data-ttu-id="5d4d6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d4d6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d4d6-110">Permission type</span></span>      | <span data-ttu-id="5d4d6-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d4d6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d4d6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d4d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5d4d6-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="5d4d6-113">EduRoster.ReadBasic</span></span> |
|<span data-ttu-id="5d4d6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d4d6-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5d4d6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-115">Not supported.</span></span>  |
|<span data-ttu-id="5d4d6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d4d6-116">Application</span></span> | <span data-ttu-id="5d4d6-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d4d6-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5d4d6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d4d6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5d4d6-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5d4d6-119">Optional query parameters</span></span>
<span data-ttu-id="5d4d6-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d4d6-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d4d6-121">Request headers</span></span>
| <span data-ttu-id="5d4d6-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d4d6-122">Header</span></span>       | <span data-ttu-id="5d4d6-123">値</span><span class="sxs-lookup"><span data-stu-id="5d4d6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5d4d6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d4d6-124">Authorization</span></span>  | <span data-ttu-id="5d4d6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-p103">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="5d4d6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d4d6-127">Request body</span></span>
<span data-ttu-id="5d4d6-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5d4d6-129">応答</span><span class="sxs-lookup"><span data-stu-id="5d4d6-129">Response</span></span>
<span data-ttu-id="5d4d6-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d4d6-131">例</span><span class="sxs-lookup"><span data-stu-id="5d4d6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d4d6-132">要求</span><span class="sxs-lookup"><span data-stu-id="5d4d6-132">Request</span></span>
<span data-ttu-id="5d4d6-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes
```
##### <a name="response"></a><span data-ttu-id="5d4d6-134">応答</span><span class="sxs-lookup"><span data-stu-id="5d4d6-134">Response</span></span>
<span data-ttu-id="5d4d6-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-135">The following is an example of the response.</span></span> 

><span data-ttu-id="5d4d6-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5d4d6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    }  
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
