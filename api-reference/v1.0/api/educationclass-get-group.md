---
title: グループを取得する
description: この **educationClass** に対応する Office 365 **グループ**を取得します。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dd0cc9f78a9686354b560a0296c545d19a3c0dc3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370460"
---
# <a name="get-group"></a><span data-ttu-id="35046-103">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="35046-103">Get group</span></span>

<span data-ttu-id="35046-104">この **educationClass** に対応する Office 365 **グループ**を取得します。</span><span class="sxs-lookup"><span data-stu-id="35046-104">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="35046-105">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="35046-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="35046-106">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="35046-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="35046-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="35046-107">Permissions</span></span>
<span data-ttu-id="35046-108">この API を呼び出すには、アクセス許可の組み合わせが必要です。</span><span class="sxs-lookup"><span data-stu-id="35046-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="35046-109">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35046-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35046-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35046-110">Permission type</span></span>      | <span data-ttu-id="35046-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="35046-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35046-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35046-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="35046-113">One from EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write plus Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="35046-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="35046-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35046-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="35046-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35046-115">Not supported.</span></span>  |
|<span data-ttu-id="35046-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35046-116">Application</span></span> | <span data-ttu-id="35046-117">EduRoster.Read.All、EduRoster.ReadWrite.All plus Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="35046-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="35046-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35046-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="35046-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35046-119">Request headers</span></span>
| <span data-ttu-id="35046-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35046-120">Header</span></span>       | <span data-ttu-id="35046-121">値</span><span class="sxs-lookup"><span data-stu-id="35046-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="35046-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35046-122">Authorization</span></span>  | <span data-ttu-id="35046-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="35046-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="35046-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="35046-125">Request body</span></span>
<span data-ttu-id="35046-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="35046-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="35046-127">応答</span><span class="sxs-lookup"><span data-stu-id="35046-127">Response</span></span>
<span data-ttu-id="35046-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="35046-128">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35046-129">例</span><span class="sxs-lookup"><span data-stu-id="35046-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35046-130">要求</span><span class="sxs-lookup"><span data-stu-id="35046-130">Request</span></span>
<span data-ttu-id="35046-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="35046-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="35046-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="35046-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35046-133">C#</span><span class="sxs-lookup"><span data-stu-id="35046-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35046-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35046-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35046-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="35046-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="35046-136">Java</span><span class="sxs-lookup"><span data-stu-id="35046-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="35046-137">応答</span><span class="sxs-lookup"><span data-stu-id="35046-137">Response</span></span>
<span data-ttu-id="35046-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="35046-138">The following is an example of the response.</span></span> 

><span data-ttu-id="35046-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="35046-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
