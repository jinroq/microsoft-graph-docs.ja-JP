---
title: クラスをリストする
description: 'クラス オブジェクトのリストを取得します。 委任されたトークンを使用した場合、メンバーは自分のクラスに関する情報以外を参照できません。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: ba276c72cc34c502670d73b70d10958954ccd691
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859826"
---
# <a name="list-classes"></a><span data-ttu-id="e3f3d-104">クラスをリストする</span><span class="sxs-lookup"><span data-stu-id="e3f3d-104">List classes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3f3d-105">クラス オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-105">Retrieve a list of class objects.</span></span> <span data-ttu-id="e3f3d-106">委任されたトークンを使用した場合、メンバーは自分のクラスに関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-106">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="e3f3d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3f3d-107">Permissions</span></span>
<span data-ttu-id="e3f3d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3f3d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3f3d-110">Permission type</span></span>      | <span data-ttu-id="e3f3d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3f3d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3f3d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3f3d-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e3f3d-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e3f3d-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="e3f3d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3f3d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e3f3d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-115">Not supported.</span></span>  |
|<span data-ttu-id="e3f3d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3f3d-116">Application</span></span> | <span data-ttu-id="e3f3d-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f3d-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e3f3d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3f3d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3f3d-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e3f3d-119">Optional query parameters</span></span>
<span data-ttu-id="e3f3d-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3f3d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3f3d-121">Request headers</span></span>
| <span data-ttu-id="e3f3d-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3f3d-122">Header</span></span>       | <span data-ttu-id="e3f3d-123">値</span><span class="sxs-lookup"><span data-stu-id="e3f3d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3f3d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3f3d-124">Authorization</span></span>  | <span data-ttu-id="e3f3d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3f3d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3f3d-127">Request body</span></span>
<span data-ttu-id="e3f3d-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e3f3d-129">応答</span><span class="sxs-lookup"><span data-stu-id="e3f3d-129">Response</span></span>
<span data-ttu-id="e3f3d-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3f3d-131">例</span><span class="sxs-lookup"><span data-stu-id="e3f3d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3f3d-132">要求</span><span class="sxs-lookup"><span data-stu-id="e3f3d-132">Request</span></span>
<span data-ttu-id="e3f3d-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e3f3d-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e3f3d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/classes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e3f3d-135">C#</span><span class="sxs-lookup"><span data-stu-id="e3f3d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3f3d-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3f3d-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e3f3d-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="e3f3d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e3f3d-138">Java</span><span class="sxs-lookup"><span data-stu-id="e3f3d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e3f3d-139">応答</span><span class="sxs-lookup"><span data-stu-id="e3f3d-139">Response</span></span>
<span data-ttu-id="e3f3d-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-140">The following is an example of the response.</span></span> 

><span data-ttu-id="e3f3d-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e3f3d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
