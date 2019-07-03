---
title: ContactFolder を作成する　
description: ユーザーの既定の連絡先フォルダーの下に新しい contactFolder を作成します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0600461b0298349ce49cdf9d57d7cd10b9e06e0b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460155"
---
# <a name="create-contactfolder"></a><span data-ttu-id="3c7fe-103">ContactFolder を作成する　</span><span class="sxs-lookup"><span data-stu-id="3c7fe-103">Create ContactFolder</span></span>

<span data-ttu-id="3c7fe-104">ユーザーの既定の連絡先フォルダーの下に新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="3c7fe-104">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="3c7fe-105">また、[指定した連絡先フォルダーの子として新しい contactfolder を作成](contactfolder-post-childfolders.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="3c7fe-105">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3c7fe-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3c7fe-106">Permissions</span></span>
<span data-ttu-id="3c7fe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c7fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c7fe-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c7fe-109">Permission type</span></span>      | <span data-ttu-id="3c7fe-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c7fe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c7fe-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c7fe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c7fe-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c7fe-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3c7fe-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c7fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c7fe-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c7fe-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3c7fe-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c7fe-115">Application</span></span> | <span data-ttu-id="3c7fe-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c7fe-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c7fe-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c7fe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="3c7fe-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c7fe-118">Request headers</span></span>
| <span data-ttu-id="3c7fe-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c7fe-119">Header</span></span>       | <span data-ttu-id="3c7fe-120">値</span><span class="sxs-lookup"><span data-stu-id="3c7fe-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c7fe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c7fe-121">Authorization</span></span>  | <span data-ttu-id="3c7fe-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3c7fe-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3c7fe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c7fe-124">Content-Type</span></span>  | <span data-ttu-id="3c7fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c7fe-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c7fe-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c7fe-126">Request body</span></span>
<span data-ttu-id="3c7fe-127">要求本文で、[ContactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c7fe-127">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3c7fe-128">応答</span><span class="sxs-lookup"><span data-stu-id="3c7fe-128">Response</span></span>

<span data-ttu-id="3c7fe-129">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [ContactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3c7fe-129">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c7fe-130">例</span><span class="sxs-lookup"><span data-stu-id="3c7fe-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c7fe-131">要求</span><span class="sxs-lookup"><span data-stu-id="3c7fe-131">Request</span></span>
<span data-ttu-id="3c7fe-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c7fe-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3c7fe-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3c7fe-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c7fe-134">C#</span><span class="sxs-lookup"><span data-stu-id="3c7fe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c7fe-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c7fe-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c7fe-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="3c7fe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3c7fe-137">要求本文で、[contactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c7fe-137">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3c7fe-138">応答</span><span class="sxs-lookup"><span data-stu-id="3c7fe-138">Response</span></span>
<span data-ttu-id="3c7fe-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3c7fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
