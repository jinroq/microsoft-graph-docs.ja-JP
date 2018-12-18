---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。
author: angelgolfer-ms
ms.openlocfilehash: 29432762aca0ad8d80b8d755ae3c0f45e754cb45
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321442"
---
# <a name="create-contact"></a><span data-ttu-id="2c632-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="2c632-103">Create contact</span></span>

<span data-ttu-id="2c632-104">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="2c632-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c632-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2c632-105">Permissions</span></span>

<span data-ttu-id="2c632-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2c632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c632-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2c632-108">Permission type</span></span>      | <span data-ttu-id="2c632-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2c632-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c632-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2c632-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c632-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c632-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2c632-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2c632-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c632-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c632-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2c632-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2c632-114">Application</span></span> | <span data-ttu-id="2c632-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c632-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c632-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2c632-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="2c632-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2c632-117">Request headers</span></span>

| <span data-ttu-id="2c632-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2c632-118">Header</span></span>       | <span data-ttu-id="2c632-119">値</span><span class="sxs-lookup"><span data-stu-id="2c632-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c632-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c632-120">Authorization</span></span>  | <span data-ttu-id="2c632-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2c632-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2c632-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c632-123">Content-Type</span></span>  | <span data-ttu-id="2c632-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2c632-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c632-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2c632-126">Request body</span></span>
<span data-ttu-id="2c632-127">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2c632-127">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2c632-128">応答</span><span class="sxs-lookup"><span data-stu-id="2c632-128">Response</span></span>

<span data-ttu-id="2c632-129">成功した場合、このメソッドは `201 Created` 応答コードと[連絡先](../resources/contact.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="2c632-129">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c632-130">例</span><span class="sxs-lookup"><span data-stu-id="2c632-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c632-131">要求</span><span class="sxs-lookup"><span data-stu-id="2c632-131">Request</span></span>

<span data-ttu-id="2c632-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2c632-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<span data-ttu-id="2c632-133">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2c632-133">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="2c632-134">応答</span><span class="sxs-lookup"><span data-stu-id="2c632-134">Response</span></span>

<span data-ttu-id="2c632-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2c632-135">Here is an example of the response.</span></span> <span data-ttu-id="2c632-136">**注:** 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2c632-136">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2c632-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2c632-137">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
