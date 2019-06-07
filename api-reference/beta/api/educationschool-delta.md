---
title: 'educationSchool: delta'
description: 学校コレクション全体の完全な読み取りを行わずに、新しく作成または更新された教育機関を取得します。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ef31d8cfa9f7b3680c4371e87eb86a46051f75bf
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764766"
---
# <a name="educationschool-delta"></a><span data-ttu-id="5acd5-103">educationSchool: delta</span><span class="sxs-lookup"><span data-stu-id="5acd5-103">educationSchool: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5acd5-104">学校コレクション全体の完全な読み取りを行わずに、新しく作成または更新された教育機関を取得します。</span><span class="sxs-lookup"><span data-stu-id="5acd5-104">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="5acd5-105">詳細については、「 [Use delta query](/graph/delta-query-overview) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5acd5-105">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="5acd5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5acd5-106">Permissions</span></span>

<span data-ttu-id="5acd5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5acd5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5acd5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5acd5-109">Permission type</span></span>                        | <span data-ttu-id="5acd5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5acd5-110">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="5acd5-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5acd5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5acd5-112">Eduroster.readbasic、Eduroster.readbasic、または Eduroster.readbasic の読み取り/書き込み</span><span class="sxs-lookup"><span data-stu-id="5acd5-112">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="5acd5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5acd5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5acd5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5acd5-114">Not supported.</span></span>                                                           |
| <span data-ttu-id="5acd5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5acd5-115">Application</span></span>                            | <span data-ttu-id="5acd5-116">Eduroster.readbasic、Eduroster.readbasic、または Eduroster.readbasic のすべての値を取得します。</span><span class="sxs-lookup"><span data-stu-id="5acd5-116">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5acd5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5acd5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/schools/{id}/delta
POST /education/me/schools/{id}/delta
POST /education/users/{id}/schools/{id}/delta

```

## <a name="request-headers"></a><span data-ttu-id="5acd5-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5acd5-118">Request headers</span></span>

| <span data-ttu-id="5acd5-119">名前</span><span class="sxs-lookup"><span data-stu-id="5acd5-119">Name</span></span>          | <span data-ttu-id="5acd5-120">説明</span><span class="sxs-lookup"><span data-stu-id="5acd5-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="5acd5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5acd5-121">Authorization</span></span> | <span data-ttu-id="5acd5-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5acd5-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5acd5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5acd5-123">Request body</span></span>

<span data-ttu-id="5acd5-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5acd5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5acd5-125">応答</span><span class="sxs-lookup"><span data-stu-id="5acd5-125">Response</span></span>

<span data-ttu-id="5acd5-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationSchool](../resources/educationschool.md) collection オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5acd5-126">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5acd5-127">例</span><span class="sxs-lookup"><span data-stu-id="5acd5-127">Example</span></span>

<span data-ttu-id="5acd5-128">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5acd5-128">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5acd5-129">要求</span><span class="sxs-lookup"><span data-stu-id="5acd5-129">Request</span></span>

<span data-ttu-id="5acd5-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5acd5-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="5acd5-131">応答</span><span class="sxs-lookup"><span data-stu-id="5acd5-131">Response</span></span>

<span data-ttu-id="5acd5-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5acd5-132">The following is an example of the response.</span></span> 

><span data-ttu-id="5acd5-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5acd5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "principalEmail": "principalEmail-value",
      "principalName": "principalName-value",
      "externalPrincipalId": "externalPrincipalId-value",
      "lowestGrade": "lowestGrade-value",
      "highestGrade": "highestGrade-value",
      "schoolNumber": "schoolNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
