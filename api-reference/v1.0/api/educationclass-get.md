---
title: Get educationClass
description: "  グループの管理者は、クラスの先生を表しています。 委任されたトークンを使用している場合、ユーザーはユーザーがメンバーになっているクラスのみを参照できます。"
localization_priority: Normal
ms.openlocfilehash: 56717404d996e04c57ff194dafdb8231cf96f55f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849589"
---
# <a name="get-educationclass"></a><span data-ttu-id="827ba-104">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="827ba-104">Get educationClass</span></span>

<span data-ttu-id="827ba-105">システムからクラスを取得します。</span><span class="sxs-lookup"><span data-stu-id="827ba-105">Retrieve a class from the system.</span></span> <span data-ttu-id="827ba-106">クラスは、グループがクラスであることをシステムに示す特別なプロパティを持つユニバーサル グループです。</span><span class="sxs-lookup"><span data-stu-id="827ba-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="827ba-107">グループのメンバーは学生を表します。グループ管理者はクラスの教師を表します。</span><span class="sxs-lookup"><span data-stu-id="827ba-107">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="827ba-108">委任されたトークンを使用している場合、ユーザーはユーザーがメンバーになっているクラスのみを参照できます。</span><span class="sxs-lookup"><span data-stu-id="827ba-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="827ba-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="827ba-109">Permissions</span></span>
<span data-ttu-id="827ba-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="827ba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="827ba-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="827ba-112">Permission type</span></span>      | <span data-ttu-id="827ba-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="827ba-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="827ba-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="827ba-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="827ba-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="827ba-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="827ba-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="827ba-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="827ba-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="827ba-117">Not supported</span></span>  |
|<span data-ttu-id="827ba-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="827ba-118">Application</span></span> | <span data-ttu-id="827ba-119">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="827ba-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="827ba-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="827ba-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="827ba-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="827ba-121">Optional query parameters</span></span>
<span data-ttu-id="827ba-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="827ba-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="827ba-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="827ba-123">Request headers</span></span>
| <span data-ttu-id="827ba-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="827ba-124">Header</span></span>       | <span data-ttu-id="827ba-125">値</span><span class="sxs-lookup"><span data-stu-id="827ba-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="827ba-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="827ba-126">Authorization</span></span>  | <span data-ttu-id="827ba-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="827ba-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="827ba-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="827ba-129">Request body</span></span>
<span data-ttu-id="827ba-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="827ba-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="827ba-131">応答</span><span class="sxs-lookup"><span data-stu-id="827ba-131">Response</span></span>
<span data-ttu-id="827ba-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="827ba-132">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="827ba-133">例</span><span class="sxs-lookup"><span data-stu-id="827ba-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="827ba-134">要求</span><span class="sxs-lookup"><span data-stu-id="827ba-134">Request</span></span>
<span data-ttu-id="827ba-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="827ba-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="827ba-136">応答</span><span class="sxs-lookup"><span data-stu-id="827ba-136">Response</span></span>
<span data-ttu-id="827ba-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="827ba-137">The following is an example of the response.</span></span> 

><span data-ttu-id="827ba-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="827ba-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
