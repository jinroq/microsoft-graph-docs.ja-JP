---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cd0c6d8473347ed86aff0bd83a8cd663e9b2c1ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967120"
---
# <a name="create-contact"></a><span data-ttu-id="0439b-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="0439b-103">Create contact</span></span>

<span data-ttu-id="0439b-104">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="0439b-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="0439b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0439b-105">Permissions</span></span>

<span data-ttu-id="0439b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0439b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0439b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0439b-108">Permission type</span></span>      | <span data-ttu-id="0439b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0439b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0439b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0439b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0439b-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0439b-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0439b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0439b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0439b-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0439b-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0439b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0439b-114">Application</span></span> | <span data-ttu-id="0439b-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0439b-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0439b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0439b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="0439b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0439b-117">Request headers</span></span>

| <span data-ttu-id="0439b-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0439b-118">Header</span></span>       | <span data-ttu-id="0439b-119">値</span><span class="sxs-lookup"><span data-stu-id="0439b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0439b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0439b-120">Authorization</span></span>  | <span data-ttu-id="0439b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0439b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0439b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0439b-123">Content-Type</span></span>  | <span data-ttu-id="0439b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0439b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0439b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0439b-126">Request body</span></span>
<span data-ttu-id="0439b-127">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0439b-127">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0439b-128">応答</span><span class="sxs-lookup"><span data-stu-id="0439b-128">Response</span></span>

<span data-ttu-id="0439b-129">成功した場合、このメソッドは `201 Created` 応答コードと[連絡先](../resources/contact.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="0439b-129">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0439b-130">例</span><span class="sxs-lookup"><span data-stu-id="0439b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0439b-131">要求</span><span class="sxs-lookup"><span data-stu-id="0439b-131">Request</span></span>

<span data-ttu-id="0439b-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0439b-132">Here is an example of the request.</span></span>

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

<span data-ttu-id="0439b-133">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0439b-133">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="0439b-134">応答</span><span class="sxs-lookup"><span data-stu-id="0439b-134">Response</span></span>

<span data-ttu-id="0439b-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0439b-135">Here is an example of the response.</span></span> <span data-ttu-id="0439b-136">**注:** 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0439b-136">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0439b-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0439b-137">All the properties will be returned from an actual call.</span></span>

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
