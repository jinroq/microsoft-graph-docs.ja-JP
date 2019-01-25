---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3fd45ee7f77e2d485b7a972b8454807368796226
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528061"
---
# <a name="create-contact"></a><span data-ttu-id="73b94-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="73b94-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73b94-104">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="73b94-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="73b94-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73b94-105">Permissions</span></span>
<span data-ttu-id="73b94-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73b94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73b94-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73b94-108">Permission type</span></span>      | <span data-ttu-id="73b94-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="73b94-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73b94-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73b94-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73b94-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73b94-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="73b94-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73b94-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73b94-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73b94-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="73b94-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73b94-114">Application</span></span> | <span data-ttu-id="73b94-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73b94-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="73b94-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73b94-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="73b94-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73b94-117">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="73b94-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73b94-118">Request headers</span></span>
| <span data-ttu-id="73b94-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73b94-119">Header</span></span>       | <span data-ttu-id="73b94-120">値</span><span class="sxs-lookup"><span data-stu-id="73b94-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73b94-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="73b94-121">Authorization</span></span>  | <span data-ttu-id="73b94-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="73b94-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="73b94-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73b94-124">Content-Type</span></span>  | <span data-ttu-id="73b94-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="73b94-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73b94-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="73b94-127">Request body</span></span>
<span data-ttu-id="73b94-128">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="73b94-128">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="73b94-129">応答</span><span class="sxs-lookup"><span data-stu-id="73b94-129">Response</span></span>

<span data-ttu-id="73b94-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="73b94-130">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73b94-131">例</span><span class="sxs-lookup"><span data-stu-id="73b94-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73b94-132">要求</span><span class="sxs-lookup"><span data-stu-id="73b94-132">Request</span></span>
<span data-ttu-id="73b94-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73b94-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="73b94-134">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="73b94-134">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="73b94-135">応答</span><span class="sxs-lookup"><span data-stu-id="73b94-135">Response</span></span>
<span data-ttu-id="73b94-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73b94-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-post-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
