---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。
author: angelgolfer-ms
ms.openlocfilehash: eb80ec34a5c4bb58aa1c401a19e1ab5632f089f8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350884"
---
# <a name="create-contact"></a><span data-ttu-id="4f347-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="4f347-103">Create Contact</span></span>

> <span data-ttu-id="4f347-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4f347-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f347-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f347-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f347-106">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="4f347-106">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f347-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4f347-107">Permissions</span></span>
<span data-ttu-id="4f347-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f347-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f347-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4f347-110">Permission type</span></span>      | <span data-ttu-id="4f347-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4f347-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f347-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4f347-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4f347-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f347-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4f347-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4f347-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f347-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f347-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4f347-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4f347-116">Application</span></span> | <span data-ttu-id="4f347-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f347-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f347-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f347-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="4f347-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f347-119">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="4f347-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f347-120">Request headers</span></span>
| <span data-ttu-id="4f347-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f347-121">Header</span></span>       | <span data-ttu-id="4f347-122">値</span><span class="sxs-lookup"><span data-stu-id="4f347-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4f347-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f347-123">Authorization</span></span>  | <span data-ttu-id="4f347-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4f347-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4f347-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f347-126">Content-Type</span></span>  | <span data-ttu-id="4f347-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4f347-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f347-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="4f347-129">Request body</span></span>
<span data-ttu-id="4f347-130">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4f347-130">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4f347-131">応答</span><span class="sxs-lookup"><span data-stu-id="4f347-131">Response</span></span>

<span data-ttu-id="4f347-132">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4f347-132">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f347-133">例</span><span class="sxs-lookup"><span data-stu-id="4f347-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f347-134">要求</span><span class="sxs-lookup"><span data-stu-id="4f347-134">Request</span></span>
<span data-ttu-id="4f347-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4f347-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
<span data-ttu-id="4f347-136">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4f347-136">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4f347-137">応答</span><span class="sxs-lookup"><span data-stu-id="4f347-137">Response</span></span>
<span data-ttu-id="4f347-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4f347-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
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