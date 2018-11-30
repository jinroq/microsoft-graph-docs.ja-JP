---
title: 学生を削除する
description: educationClass から educationUser を削除する
ms.openlocfilehash: 538eb6f69e30fcc355a9ea3ce88af8afffd5993e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023105"
---
# <a name="remove-a-student"></a><span data-ttu-id="2f1eb-103">学生を削除する</span><span class="sxs-lookup"><span data-stu-id="2f1eb-103">Remove a student</span></span>

<span data-ttu-id="2f1eb-104">[educationClass](../resources/educationclass.md) から [educationUser](../resources/educationuser.md) を削除する</span><span class="sxs-lookup"><span data-stu-id="2f1eb-104">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="2f1eb-105">**メモ:** 教師_および_学生は、クラス **members** コレクションに所属します。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-105">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="2f1eb-106">この API を呼び出す前に、削除する **educationUser** が教師でないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-106">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="2f1eb-107">[educationclass_list_teachers](educationclass-list-teachers.md) を呼び出して教師のリストを取得し、削除対象のユーザーのユーザー ID が返された教師リストにないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-107">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f1eb-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2f1eb-108">Permissions</span></span>
<span data-ttu-id="2f1eb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f1eb-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f1eb-111">Permission type</span></span>      | <span data-ttu-id="2f1eb-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f1eb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f1eb-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f1eb-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f1eb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-114">Not supported.</span></span>  |
|<span data-ttu-id="2f1eb-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f1eb-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2f1eb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-116">Not supported.</span></span>  |
|<span data-ttu-id="2f1eb-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f1eb-117">Application</span></span> | <span data-ttu-id="2f1eb-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f1eb-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f1eb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f1eb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2f1eb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f1eb-120">Request headers</span></span>
| <span data-ttu-id="2f1eb-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f1eb-121">Header</span></span>       | <span data-ttu-id="2f1eb-122">値</span><span class="sxs-lookup"><span data-stu-id="2f1eb-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f1eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f1eb-123">Authorization</span></span>  | <span data-ttu-id="2f1eb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f1eb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f1eb-126">Request body</span></span>
<span data-ttu-id="2f1eb-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2f1eb-128">応答</span><span class="sxs-lookup"><span data-stu-id="2f1eb-128">Response</span></span>
<span data-ttu-id="2f1eb-129">成功した場合、このメソッドは `204 No Content` 応答コードと空の応答本文を返します。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-129">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f1eb-130">例</span><span class="sxs-lookup"><span data-stu-id="2f1eb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f1eb-131">要求</span><span class="sxs-lookup"><span data-stu-id="2f1eb-131">Request</span></span>
<span data-ttu-id="2f1eb-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/{member-id}
```

##### <a name="response"></a><span data-ttu-id="2f1eb-133">応答</span><span class="sxs-lookup"><span data-stu-id="2f1eb-133">Response</span></span>
<span data-ttu-id="2f1eb-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f1eb-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
