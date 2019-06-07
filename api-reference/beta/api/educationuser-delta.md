---
title: 'educationUser: delta'
description: ユーザーコレクション全体の完全な読み取りを実行せずに、新しく作成または更新されたユーザーを取得します。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c89c065d5e4bd8510d6821a3c7a13bd106ce9eb8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764764"
---
# <a name="educationuser-delta"></a><span data-ttu-id="65289-103">educationUser: delta</span><span class="sxs-lookup"><span data-stu-id="65289-103">educationUser: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65289-104">コレクション全体の完全な読み取りを実行せずに、新しく作成または更新された[educationUser](../resources/educationuser.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="65289-104">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="65289-105">詳細については、「 [Use delta query](/graph/delta-query-overview) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65289-105">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="65289-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65289-106">Permissions</span></span>

<span data-ttu-id="65289-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65289-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65289-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65289-109">Permission type</span></span>                        | <span data-ttu-id="65289-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65289-110">Permissions (from least to most privileged)</span></span>     |
| :------------------------------------- | :---------------------------------------------- |
| <span data-ttu-id="65289-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65289-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65289-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65289-112">Not supported.</span></span>                                  |
| <span data-ttu-id="65289-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65289-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65289-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65289-114">Not supported.</span></span>                                  |
| <span data-ttu-id="65289-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65289-115">Application</span></span>                            | <span data-ttu-id="65289-116">Eduroster.readbasic または Eduroster.readbasic のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="65289-116">EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65289-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65289-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/delta
POST /education/users/{id}/delta
POST /education/schools/{id}/users/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="65289-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65289-118">Request headers</span></span>

| <span data-ttu-id="65289-119">名前</span><span class="sxs-lookup"><span data-stu-id="65289-119">Name</span></span>          | <span data-ttu-id="65289-120">説明</span><span class="sxs-lookup"><span data-stu-id="65289-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="65289-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65289-121">Authorization</span></span> | <span data-ttu-id="65289-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="65289-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="65289-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="65289-123">Request body</span></span>

<span data-ttu-id="65289-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="65289-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65289-125">応答</span><span class="sxs-lookup"><span data-stu-id="65289-125">Response</span></span>

<span data-ttu-id="65289-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationUser](../resources/educationuser.md) collection オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="65289-126">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65289-127">例</span><span class="sxs-lookup"><span data-stu-id="65289-127">Example</span></span>

<span data-ttu-id="65289-128">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="65289-128">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="65289-129">要求</span><span class="sxs-lookup"><span data-stu-id="65289-129">Request</span></span>

<span data-ttu-id="65289-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65289-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/me/delta
```

##### <a name="response"></a><span data-ttu-id="65289-131">応答</span><span class="sxs-lookup"><span data-stu-id="65289-131">Response</span></span>

<span data-ttu-id="65289-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65289-132">The following is an example of the response.</span></span>

><span data-ttu-id="65289-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="65289-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1039

{
  "value": [
    {
      "primaryRole": "primaryRole-value",
      "middleName": "middleName-value",
      "externalSource": "externalSource-value",
      "residenceAddress": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "mailingAddress": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "student": {
        "graduationYear": "graduationYear-value",
        "grade": "grade-value",
        "birthDate": "datetime-value",
        "gender": "gender-value",
        "studentNumber": "studentNumber-value",
        "externalId": "externalId-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
