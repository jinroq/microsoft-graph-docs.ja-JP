---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。
author: dkershaw10
ms.openlocfilehash: bb6e9cc223ef547bfafb190be4381f828a0c230f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337899"
---
# <a name="create-contact"></a><span data-ttu-id="77fb7-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="77fb7-103">Create Contact</span></span>

<span data-ttu-id="77fb7-104">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="77fb7-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="77fb7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77fb7-105">Permissions</span></span>
<span data-ttu-id="77fb7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77fb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77fb7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77fb7-108">Permission type</span></span>      | <span data-ttu-id="77fb7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77fb7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77fb7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77fb7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77fb7-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77fb7-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="77fb7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77fb7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77fb7-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77fb7-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="77fb7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77fb7-114">Application</span></span> | <span data-ttu-id="77fb7-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77fb7-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="77fb7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77fb7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="77fb7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77fb7-117">Request headers</span></span>
| <span data-ttu-id="77fb7-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77fb7-118">Header</span></span>       | <span data-ttu-id="77fb7-119">値</span><span class="sxs-lookup"><span data-stu-id="77fb7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77fb7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="77fb7-120">Authorization</span></span>  | <span data-ttu-id="77fb7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="77fb7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="77fb7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77fb7-123">Content-Type</span></span>  | <span data-ttu-id="77fb7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="77fb7-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77fb7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="77fb7-125">Request body</span></span>
<span data-ttu-id="77fb7-126">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="77fb7-126">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="77fb7-127">応答</span><span class="sxs-lookup"><span data-stu-id="77fb7-127">Response</span></span>

<span data-ttu-id="77fb7-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="77fb7-128">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77fb7-129">例</span><span class="sxs-lookup"><span data-stu-id="77fb7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77fb7-130">要求</span><span class="sxs-lookup"><span data-stu-id="77fb7-130">Request</span></span>
<span data-ttu-id="77fb7-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77fb7-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky"
    }
  ],
  "businessPhones": [
    "+1 732 555 0102"
  ]
}
```
<span data-ttu-id="77fb7-132">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="77fb7-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="77fb7-133">応答</span><span class="sxs-lookup"><span data-stu-id="77fb7-133">Response</span></span>
<span data-ttu-id="77fb7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="77fb7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "createdDateTime": "2015-11-09T02:14:32Z",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z",
   "displayName": "Pavel Bansky"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
