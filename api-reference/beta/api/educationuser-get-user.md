---
title: Get user
description: この **educationUser** に対応する単純なディレクトリ **user** を取得します。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f0c731130abb88a2eef4aec0343fb0c9d3bdddd2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984837"
---
# <a name="get-user"></a><span data-ttu-id="896c7-103">ユーザーを取得する</span><span class="sxs-lookup"><span data-stu-id="896c7-103">Get user</span></span>

> <span data-ttu-id="896c7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="896c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="896c7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="896c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="896c7-106">この **educationUser** に対応する単純なディレクトリ **user** を取得します。</span><span class="sxs-lookup"><span data-stu-id="896c7-106">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="896c7-107">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="896c7-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="896c7-108">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="896c7-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="896c7-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="896c7-109">Permissions</span></span>
<span data-ttu-id="896c7-110">この API を呼び出すには、アクセス許可の組み合わせが必要です。</span><span class="sxs-lookup"><span data-stu-id="896c7-110">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="896c7-111">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="896c7-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="896c7-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="896c7-112">Permission type</span></span>      | <span data-ttu-id="896c7-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="896c7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="896c7-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="896c7-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="896c7-115">One from EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write plus either Directory.Read.All or User.Read</span><span class="sxs-lookup"><span data-stu-id="896c7-115">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="896c7-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="896c7-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="896c7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="896c7-117">Not supported.</span></span>  |
|<span data-ttu-id="896c7-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="896c7-118">Application</span></span> | <span data-ttu-id="896c7-119">EduRoster.Read.All、EduRoster.ReadWrite.All plus Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="896c7-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="896c7-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="896c7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="896c7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="896c7-121">Request headers</span></span>
| <span data-ttu-id="896c7-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="896c7-122">Header</span></span>       | <span data-ttu-id="896c7-123">値</span><span class="sxs-lookup"><span data-stu-id="896c7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="896c7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="896c7-124">Authorization</span></span>  | <span data-ttu-id="896c7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="896c7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="896c7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="896c7-127">Request body</span></span>
<span data-ttu-id="896c7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="896c7-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="896c7-129">応答</span><span class="sxs-lookup"><span data-stu-id="896c7-129">Response</span></span>
<span data-ttu-id="896c7-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="896c7-130">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="896c7-131">例</span><span class="sxs-lookup"><span data-stu-id="896c7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="896c7-132">要求</span><span class="sxs-lookup"><span data-stu-id="896c7-132">Request</span></span>
<span data-ttu-id="896c7-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="896c7-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/user
```
##### <a name="response"></a><span data-ttu-id="896c7-134">応答</span><span class="sxs-lookup"><span data-stu-id="896c7-134">Response</span></span>
<span data-ttu-id="896c7-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="896c7-135">The following is an example of the response.</span></span> 

><span data-ttu-id="896c7-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="896c7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

<!-- uuid: FC4AAF57-A0ED-4899-B104-A8B89B72AD5A
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
