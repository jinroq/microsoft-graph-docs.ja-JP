---
title: MailFolder を作成する
description: この API を使用して、ユーザーのメールボックスのルート フォルダーに新しいメール フォルダーを作成します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 05619c948c4db80711873daa9e052677f5b49a1e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460134"
---
# <a name="create-mailfolder"></a><span data-ttu-id="f6268-103">MailFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="f6268-103">Create MailFolder</span></span>

<span data-ttu-id="f6268-104">この API を使用して、ユーザーのメールボックスのルート フォルダーに新しいメール フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="f6268-104">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6268-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6268-105">Permissions</span></span>
<span data-ttu-id="f6268-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6268-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6268-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6268-108">Permission type</span></span>      | <span data-ttu-id="f6268-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6268-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6268-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6268-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6268-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6268-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f6268-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6268-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6268-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6268-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f6268-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6268-114">Application</span></span> | <span data-ttu-id="f6268-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6268-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6268-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6268-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="f6268-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6268-117">Request headers</span></span>
| <span data-ttu-id="f6268-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6268-118">Header</span></span>       | <span data-ttu-id="f6268-119">値</span><span class="sxs-lookup"><span data-stu-id="f6268-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6268-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6268-120">Authorization</span></span>  | <span data-ttu-id="f6268-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f6268-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f6268-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6268-123">Content-Type</span></span>  | <span data-ttu-id="f6268-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f6268-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6268-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6268-125">Request body</span></span>
<span data-ttu-id="f6268-p103">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。[MailFolder](../resources/mailfolder.md) オブジェクトに対して書き込み可能なプロパティは **displayName** のみです。</span><span class="sxs-lookup"><span data-stu-id="f6268-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="f6268-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f6268-128">Parameter</span></span>    | <span data-ttu-id="f6268-129">型</span><span class="sxs-lookup"><span data-stu-id="f6268-129">Type</span></span>   |<span data-ttu-id="f6268-130">説明</span><span class="sxs-lookup"><span data-stu-id="f6268-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6268-131">displayName</span><span class="sxs-lookup"><span data-stu-id="f6268-131">displayName</span></span>|<span data-ttu-id="f6268-132">String</span><span class="sxs-lookup"><span data-stu-id="f6268-132">String</span></span>|<span data-ttu-id="f6268-133">新しいフォルダーの表示名です。</span><span class="sxs-lookup"><span data-stu-id="f6268-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="f6268-134">応答</span><span class="sxs-lookup"><span data-stu-id="f6268-134">Response</span></span>

<span data-ttu-id="f6268-135">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f6268-135">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6268-136">例</span><span class="sxs-lookup"><span data-stu-id="f6268-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6268-137">要求</span><span class="sxs-lookup"><span data-stu-id="f6268-137">Request</span></span>
<span data-ttu-id="f6268-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6268-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f6268-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f6268-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6268-140">C#</span><span class="sxs-lookup"><span data-stu-id="f6268-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6268-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="f6268-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6268-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="f6268-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f6268-143">応答</span><span class="sxs-lookup"><span data-stu-id="f6268-143">Response</span></span>
<span data-ttu-id="f6268-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f6268-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
