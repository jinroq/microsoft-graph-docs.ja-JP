---
title: educationClasses をリストする
description: 学校が所有するクラスのリストを取得します。
author: mmast-msft
ms.openlocfilehash: e1c4681b9194defc2362e4f24ad1593e8885680c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330731"
---
# <a name="list-educationclasses"></a><span data-ttu-id="b6998-103">educationClasses をリストする</span><span class="sxs-lookup"><span data-stu-id="b6998-103">List educationClasses</span></span>

> <span data-ttu-id="b6998-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b6998-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6998-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6998-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6998-106">学校が所有するクラスのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="b6998-106">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6998-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6998-107">Permissions</span></span>
<span data-ttu-id="b6998-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6998-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6998-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6998-110">Permission type</span></span>      | <span data-ttu-id="b6998-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6998-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6998-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6998-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="b6998-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b6998-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="b6998-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6998-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b6998-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6998-115">Not supported.</span></span>  |
|<span data-ttu-id="b6998-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6998-116">Application</span></span> | <span data-ttu-id="b6998-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6998-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b6998-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6998-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6998-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b6998-119">Optional query parameters</span></span>
<span data-ttu-id="b6998-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b6998-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6998-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6998-121">Request headers</span></span>
| <span data-ttu-id="b6998-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6998-122">Header</span></span>       | <span data-ttu-id="b6998-123">値</span><span class="sxs-lookup"><span data-stu-id="b6998-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b6998-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6998-124">Authorization</span></span>  | <span data-ttu-id="b6998-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b6998-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b6998-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6998-127">Request body</span></span>
<span data-ttu-id="b6998-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b6998-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b6998-129">応答</span><span class="sxs-lookup"><span data-stu-id="b6998-129">Response</span></span>
<span data-ttu-id="b6998-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b6998-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6998-131">例</span><span class="sxs-lookup"><span data-stu-id="b6998-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6998-132">要求</span><span class="sxs-lookup"><span data-stu-id="b6998-132">Request</span></span>
<span data-ttu-id="b6998-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b6998-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/classes
```
##### <a name="response"></a><span data-ttu-id="b6998-134">応答</span><span class="sxs-lookup"><span data-stu-id="b6998-134">Response</span></span>
<span data-ttu-id="b6998-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b6998-135">The following is an example of the response.</span></span> 

><span data-ttu-id="b6998-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b6998-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
