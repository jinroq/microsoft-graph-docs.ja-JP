---
title: Get educationClass
description: "  グループの管理者は、クラスの先生を表しています。 委任されたトークンを使用している場合、ユーザーはユーザーがメンバーになっているクラスのみを参照できます。"
ms.openlocfilehash: 36dfe4802fbd8042d4baee2da10763b0d9e4c5cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024112"
---
# <a name="get-educationclass"></a><span data-ttu-id="c96cb-104">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="c96cb-104">Get educationClass</span></span>

<span data-ttu-id="c96cb-105">システムからクラスを取得します。</span><span class="sxs-lookup"><span data-stu-id="c96cb-105">Retrieve a class from the system.</span></span> <span data-ttu-id="c96cb-106">クラスは、グループがクラスであることをシステムに示す特別なプロパティを持つユニバーサル グループです。</span><span class="sxs-lookup"><span data-stu-id="c96cb-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="c96cb-107">グループのメンバーは学生を表します。グループ管理者はクラスの教師を表します。</span><span class="sxs-lookup"><span data-stu-id="c96cb-107">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="c96cb-108">委任されたトークンを使用している場合、ユーザーはユーザーがメンバーになっているクラスのみを参照できます。</span><span class="sxs-lookup"><span data-stu-id="c96cb-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="c96cb-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c96cb-109">Permissions</span></span>
<span data-ttu-id="c96cb-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c96cb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c96cb-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c96cb-112">Permission type</span></span>      | <span data-ttu-id="c96cb-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c96cb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c96cb-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c96cb-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="c96cb-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c96cb-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c96cb-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c96cb-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c96cb-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="c96cb-117">Not supported</span></span>  |
|<span data-ttu-id="c96cb-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c96cb-118">Application</span></span> | <span data-ttu-id="c96cb-119">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c96cb-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c96cb-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c96cb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c96cb-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c96cb-121">Optional query parameters</span></span>
<span data-ttu-id="c96cb-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c96cb-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c96cb-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c96cb-123">Request headers</span></span>
| <span data-ttu-id="c96cb-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c96cb-124">Header</span></span>       | <span data-ttu-id="c96cb-125">値</span><span class="sxs-lookup"><span data-stu-id="c96cb-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c96cb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c96cb-126">Authorization</span></span>  | <span data-ttu-id="c96cb-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c96cb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c96cb-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c96cb-129">Request body</span></span>
<span data-ttu-id="c96cb-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c96cb-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c96cb-131">応答</span><span class="sxs-lookup"><span data-stu-id="c96cb-131">Response</span></span>
<span data-ttu-id="c96cb-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c96cb-132">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c96cb-133">例</span><span class="sxs-lookup"><span data-stu-id="c96cb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c96cb-134">要求</span><span class="sxs-lookup"><span data-stu-id="c96cb-134">Request</span></span>
<span data-ttu-id="c96cb-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c96cb-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="c96cb-136">応答</span><span class="sxs-lookup"><span data-stu-id="c96cb-136">Response</span></span>
<span data-ttu-id="c96cb-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c96cb-137">The following is an example of the response.</span></span> 

><span data-ttu-id="c96cb-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c96cb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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