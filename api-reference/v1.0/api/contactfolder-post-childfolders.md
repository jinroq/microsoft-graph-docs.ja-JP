---
title: ContactFolder を作成する　
description: '指定したフォルダーの子として新しい contactFolder を作成します。 '
ms.openlocfilehash: b6a4779b52a554e3a4050009e68b4124c17ca935
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020890"
---
# <a name="create-contactfolder"></a><span data-ttu-id="a7d5a-103">ContactFolder を作成する　</span><span class="sxs-lookup"><span data-stu-id="a7d5a-103">Create ContactFolder</span></span>

<span data-ttu-id="a7d5a-104">指定したフォルダーの子として新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="a7d5a-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="a7d5a-105">[ユーザーの既定の連絡先フォルダーの下に新しい contactFolder を作成する](user-post-contactfolders.md)こともできます。</span><span class="sxs-lookup"><span data-stu-id="a7d5a-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a7d5a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a7d5a-106">Permissions</span></span>
<span data-ttu-id="a7d5a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7d5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7d5a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7d5a-109">Permission type</span></span>      | <span data-ttu-id="a7d5a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7d5a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7d5a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7d5a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7d5a-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7d5a-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a7d5a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7d5a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7d5a-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7d5a-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a7d5a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7d5a-115">Application</span></span> | <span data-ttu-id="a7d5a-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7d5a-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7d5a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7d5a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="a7d5a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7d5a-118">Request headers</span></span>
| <span data-ttu-id="a7d5a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7d5a-119">Header</span></span>       | <span data-ttu-id="a7d5a-120">値</span><span class="sxs-lookup"><span data-stu-id="a7d5a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7d5a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7d5a-121">Authorization</span></span>  | <span data-ttu-id="a7d5a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a7d5a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a7d5a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7d5a-124">Content-Type</span></span>  | <span data-ttu-id="a7d5a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a7d5a-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7d5a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7d5a-127">Request body</span></span>
<span data-ttu-id="a7d5a-128">要求本文で、[ContactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7d5a-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a7d5a-129">応答</span><span class="sxs-lookup"><span data-stu-id="a7d5a-129">Response</span></span>

<span data-ttu-id="a7d5a-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [ContactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a7d5a-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7d5a-131">例</span><span class="sxs-lookup"><span data-stu-id="a7d5a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7d5a-132">要求</span><span class="sxs-lookup"><span data-stu-id="a7d5a-132">Request</span></span>
<span data-ttu-id="a7d5a-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a7d5a-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="a7d5a-134">要求本文で、[contactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7d5a-134">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a7d5a-135">応答</span><span class="sxs-lookup"><span data-stu-id="a7d5a-135">Response</span></span>
<span data-ttu-id="a7d5a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a7d5a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
