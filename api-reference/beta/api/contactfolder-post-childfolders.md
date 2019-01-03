---
title: ContactFolder を作成する　
description: '指定したフォルダーの子として新しい contactFolder を作成します。 '
author: angelgolfer-ms
ms.openlocfilehash: a6b638610ed487fe69d80254c36efc3478f476cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336485"
---
# <a name="create-contactfolder"></a><span data-ttu-id="1bec1-103">ContactFolder を作成する　</span><span class="sxs-lookup"><span data-stu-id="1bec1-103">Create ContactFolder</span></span>

> <span data-ttu-id="1bec1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1bec1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bec1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1bec1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1bec1-106">指定したフォルダーの子として新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="1bec1-106">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="1bec1-107">[ユーザーの既定の連絡先フォルダーの下に新しい contactFolder を作成する](user-post-contactfolders.md)こともできます。</span><span class="sxs-lookup"><span data-stu-id="1bec1-107">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1bec1-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1bec1-108">Permissions</span></span>
<span data-ttu-id="1bec1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1bec1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bec1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1bec1-111">Permission type</span></span>      | <span data-ttu-id="1bec1-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1bec1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bec1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1bec1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1bec1-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bec1-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1bec1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1bec1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bec1-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bec1-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1bec1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1bec1-117">Application</span></span> | <span data-ttu-id="1bec1-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bec1-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bec1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1bec1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="1bec1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1bec1-120">Request headers</span></span>
| <span data-ttu-id="1bec1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1bec1-121">Header</span></span>       | <span data-ttu-id="1bec1-122">値</span><span class="sxs-lookup"><span data-stu-id="1bec1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1bec1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bec1-123">Authorization</span></span>  | <span data-ttu-id="1bec1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1bec1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1bec1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1bec1-126">Content-Type</span></span>  | <span data-ttu-id="1bec1-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1bec1-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bec1-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="1bec1-129">Request body</span></span>
<span data-ttu-id="1bec1-130">要求本文で、[ContactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1bec1-130">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1bec1-131">応答</span><span class="sxs-lookup"><span data-stu-id="1bec1-131">Response</span></span>

<span data-ttu-id="1bec1-132">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [ContactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1bec1-132">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bec1-133">例</span><span class="sxs-lookup"><span data-stu-id="1bec1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bec1-134">要求</span><span class="sxs-lookup"><span data-stu-id="1bec1-134">Request</span></span>
<span data-ttu-id="1bec1-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1bec1-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
<span data-ttu-id="1bec1-136">要求本文で、[contactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1bec1-136">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1bec1-137">応答</span><span class="sxs-lookup"><span data-stu-id="1bec1-137">Response</span></span>
<span data-ttu-id="1bec1-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1bec1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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