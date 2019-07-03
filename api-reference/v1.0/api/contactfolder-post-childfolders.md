---
title: ContactFolder を作成する　
description: '指定したフォルダーの子として新しい contactFolder を作成します。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 61bf132688fbe0b7b8580c4fdb1f637b26ef7cb9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443022"
---
# <a name="create-contactfolder"></a><span data-ttu-id="56fc4-103">ContactFolder を作成する　</span><span class="sxs-lookup"><span data-stu-id="56fc4-103">Create ContactFolder</span></span>

<span data-ttu-id="56fc4-104">指定したフォルダーの子として新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="56fc4-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="56fc4-105">[ユーザーの既定の連絡先フォルダーの下に新しい contactFolder を作成する](user-post-contactfolders.md)こともできます。</span><span class="sxs-lookup"><span data-stu-id="56fc4-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="56fc4-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="56fc4-106">Permissions</span></span>
<span data-ttu-id="56fc4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56fc4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56fc4-109">Permission type</span></span>      | <span data-ttu-id="56fc4-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="56fc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56fc4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56fc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="56fc4-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56fc4-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="56fc4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56fc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56fc4-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56fc4-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="56fc4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56fc4-115">Application</span></span> | <span data-ttu-id="56fc4-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56fc4-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="56fc4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56fc4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="56fc4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56fc4-118">Request headers</span></span>
| <span data-ttu-id="56fc4-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56fc4-119">Header</span></span>       | <span data-ttu-id="56fc4-120">値</span><span class="sxs-lookup"><span data-stu-id="56fc4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="56fc4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56fc4-121">Authorization</span></span>  | <span data-ttu-id="56fc4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="56fc4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="56fc4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56fc4-124">Content-Type</span></span>  | <span data-ttu-id="56fc4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="56fc4-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56fc4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="56fc4-127">Request body</span></span>
<span data-ttu-id="56fc4-128">要求本文で、[ContactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="56fc4-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="56fc4-129">応答</span><span class="sxs-lookup"><span data-stu-id="56fc4-129">Response</span></span>

<span data-ttu-id="56fc4-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [ContactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="56fc4-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56fc4-131">例</span><span class="sxs-lookup"><span data-stu-id="56fc4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56fc4-132">要求</span><span class="sxs-lookup"><span data-stu-id="56fc4-132">Request</span></span>
<span data-ttu-id="56fc4-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56fc4-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="56fc4-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="56fc4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="56fc4-135">C#</span><span class="sxs-lookup"><span data-stu-id="56fc4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56fc4-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="56fc4-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56fc4-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="56fc4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="56fc4-138">要求本文で、[contactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="56fc4-138">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="56fc4-139">応答</span><span class="sxs-lookup"><span data-stu-id="56fc4-139">Response</span></span>
<span data-ttu-id="56fc4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56fc4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
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
