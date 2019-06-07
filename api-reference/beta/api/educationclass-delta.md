---
title: 'educationClass: delta'
description: クラスコレクション全体の完全な読み取りを実行しなくても、メンバーシップの変更など、新しく作成された、または更新されたクラスを取得します。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 03a026a479c9502e00b86e41936619613013b9af
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764763"
---
# <a name="educationclass-delta"></a><span data-ttu-id="1f072-103">educationClass: delta</span><span class="sxs-lookup"><span data-stu-id="1f072-103">educationClass: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f072-104">クラスコレクション全体の完全な読み取りを実行しなくても、メンバーシップの変更など、新しく作成された、または更新されたクラスを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f072-104">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="1f072-105">詳細については、「 [Use delta query](/graph/delta-query-overview) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f072-105">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f072-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1f072-106">Permissions</span></span>

<span data-ttu-id="1f072-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f072-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f072-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f072-109">Permission type</span></span>                        | <span data-ttu-id="1f072-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f072-110">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="1f072-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f072-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f072-112">Eduroster.readbasic、Eduroster.readbasic、または Eduroster.readbasic の読み取り/書き込み</span><span class="sxs-lookup"><span data-stu-id="1f072-112">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="1f072-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f072-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f072-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f072-114">Not supported.</span></span>                                                           |
| <span data-ttu-id="1f072-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f072-115">Application</span></span>                            | <span data-ttu-id="1f072-116">Eduroster.readbasic、Eduroster.readbasic、または Eduroster.readbasic のすべての値を取得します。</span><span class="sxs-lookup"><span data-stu-id="1f072-116">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f072-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f072-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/{id}/delta
POST /education/me/classes/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="1f072-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f072-118">Request headers</span></span>

| <span data-ttu-id="1f072-119">名前</span><span class="sxs-lookup"><span data-stu-id="1f072-119">Name</span></span>          | <span data-ttu-id="1f072-120">説明</span><span class="sxs-lookup"><span data-stu-id="1f072-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="1f072-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f072-121">Authorization</span></span> | <span data-ttu-id="1f072-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1f072-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f072-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f072-123">Request body</span></span>

<span data-ttu-id="1f072-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1f072-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f072-125">応答</span><span class="sxs-lookup"><span data-stu-id="1f072-125">Response</span></span>

<span data-ttu-id="1f072-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationClass](../resources/educationclass.md) collection オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1f072-126">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f072-127">例</span><span class="sxs-lookup"><span data-stu-id="1f072-127">Example</span></span>

<span data-ttu-id="1f072-128">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1f072-128">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1f072-129">要求</span><span class="sxs-lookup"><span data-stu-id="1f072-129">Request</span></span>

<span data-ttu-id="1f072-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f072-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="1f072-131">応答</span><span class="sxs-lookup"><span data-stu-id="1f072-131">Response</span></span>

<span data-ttu-id="1f072-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f072-132">The following is an example of the response.</span></span> 

><span data-ttu-id="1f072-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1f072-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 585

{
  "value": [
    {
      "displayName": "displayName-value",
      "mailNickname": "mailNickname-value",
      "description": "description-value",
      "createdBy": {
        "application": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "device": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "user": {
          "displayName": "displayName-value",
          "id": "id-value"
        }
      },
      "classCode": "classCode-value",
      "externalName": "externalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
