---
title: Get user
description: この **educationUser** に対応する単純なディレクトリ **user** を取得します。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 1212057af13057f691e5721bd21a351e59a82511
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526236"
---
# <a name="get-user"></a><span data-ttu-id="0df3c-103">Get user</span><span class="sxs-lookup"><span data-stu-id="0df3c-103">Get user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df3c-104">この **educationUser** に対応する単純なディレクトリ **user** を取得します。</span><span class="sxs-lookup"><span data-stu-id="0df3c-104">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="0df3c-105">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="0df3c-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="0df3c-106">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="0df3c-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="0df3c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0df3c-107">Permissions</span></span>
<span data-ttu-id="0df3c-108">この API を呼び出すには、アクセス許可の組み合わせが必要です。</span><span class="sxs-lookup"><span data-stu-id="0df3c-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="0df3c-109">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0df3c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0df3c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0df3c-110">Permission type</span></span>      | <span data-ttu-id="0df3c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0df3c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0df3c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0df3c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0df3c-113">One from EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write plus either Directory.Read.All or User.Read</span><span class="sxs-lookup"><span data-stu-id="0df3c-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="0df3c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0df3c-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0df3c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0df3c-115">Not supported.</span></span>  |
|<span data-ttu-id="0df3c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0df3c-116">Application</span></span> | <span data-ttu-id="0df3c-117">EduRoster.Read.All、EduRoster.ReadWrite.All plus Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0df3c-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="0df3c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0df3c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="0df3c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0df3c-119">Request headers</span></span>
| <span data-ttu-id="0df3c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0df3c-120">Header</span></span>       | <span data-ttu-id="0df3c-121">値</span><span class="sxs-lookup"><span data-stu-id="0df3c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0df3c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0df3c-122">Authorization</span></span>  | <span data-ttu-id="0df3c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0df3c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0df3c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0df3c-125">Request body</span></span>
<span data-ttu-id="0df3c-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0df3c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0df3c-127">応答</span><span class="sxs-lookup"><span data-stu-id="0df3c-127">Response</span></span>
<span data-ttu-id="0df3c-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0df3c-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0df3c-129">例</span><span class="sxs-lookup"><span data-stu-id="0df3c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0df3c-130">要求</span><span class="sxs-lookup"><span data-stu-id="0df3c-130">Request</span></span>
<span data-ttu-id="0df3c-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0df3c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/user
```
##### <a name="response"></a><span data-ttu-id="0df3c-132">応答</span><span class="sxs-lookup"><span data-stu-id="0df3c-132">Response</span></span>
<span data-ttu-id="0df3c-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0df3c-133">The following is an example of the response.</span></span> 

><span data-ttu-id="0df3c-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0df3c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationuser-get-user.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
