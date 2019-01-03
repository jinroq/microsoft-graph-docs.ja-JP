---
title: MailFolder を作成する
description: この API を使用して、ユーザーのメールボックスのルート フォルダーに新しいメール フォルダーを作成します。
ms.openlocfilehash: 6e6b42197dcb5b968a59303d2e9c8c8b1ddf6feb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072924"
---
# <a name="create-mailfolder"></a><span data-ttu-id="5b46a-103">MailFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="5b46a-103">Create MailFolder</span></span>

> <span data-ttu-id="5b46a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b46a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b46a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b46a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b46a-106">この API を使用して、ユーザーのメールボックスのルート フォルダーに新しいメール フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="5b46a-106">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b46a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b46a-107">Permissions</span></span>
<span data-ttu-id="5b46a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b46a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b46a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b46a-110">Permission type</span></span>      | <span data-ttu-id="5b46a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b46a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b46a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b46a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5b46a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b46a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5b46a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b46a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b46a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b46a-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5b46a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b46a-116">Application</span></span> | <span data-ttu-id="5b46a-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b46a-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b46a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b46a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="5b46a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b46a-119">Request headers</span></span>
| <span data-ttu-id="5b46a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b46a-120">Header</span></span>       | <span data-ttu-id="5b46a-121">値</span><span class="sxs-lookup"><span data-stu-id="5b46a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b46a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b46a-122">Authorization</span></span>  | <span data-ttu-id="5b46a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b46a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5b46a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b46a-125">Content-Type</span></span>  | <span data-ttu-id="5b46a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b46a-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b46a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b46a-127">Request body</span></span>
<span data-ttu-id="5b46a-p104">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。[MailFolder](../resources/mailfolder.md) オブジェクトに対して書き込み可能なプロパティは **displayName** のみです。</span><span class="sxs-lookup"><span data-stu-id="5b46a-p104">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="5b46a-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b46a-130">Parameter</span></span>    | <span data-ttu-id="5b46a-131">型</span><span class="sxs-lookup"><span data-stu-id="5b46a-131">Type</span></span>   |<span data-ttu-id="5b46a-132">説明</span><span class="sxs-lookup"><span data-stu-id="5b46a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b46a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5b46a-133">displayName</span></span>|<span data-ttu-id="5b46a-134">String</span><span class="sxs-lookup"><span data-stu-id="5b46a-134">String</span></span>|<span data-ttu-id="5b46a-135">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="5b46a-135">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="5b46a-136">応答</span><span class="sxs-lookup"><span data-stu-id="5b46a-136">Response</span></span>

<span data-ttu-id="5b46a-137">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5b46a-137">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b46a-138">例</span><span class="sxs-lookup"><span data-stu-id="5b46a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b46a-139">要求</span><span class="sxs-lookup"><span data-stu-id="5b46a-139">Request</span></span>
<span data-ttu-id="5b46a-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b46a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="5b46a-141">応答</span><span class="sxs-lookup"><span data-stu-id="5b46a-141">Response</span></span>
<span data-ttu-id="5b46a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b46a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->