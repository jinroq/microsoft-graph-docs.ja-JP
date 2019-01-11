---
title: ContactFolder を作成する　
description: ユーザーの既定の連絡先フォルダーの下に新しい contactFolder を作成します。
localization_priority: Normal
ms.openlocfilehash: 4bd4fb26c78127fce9fff691cf187020428d9ab5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889710"
---
# <a name="create-contactfolder"></a><span data-ttu-id="211a7-103">ContactFolder を作成する　</span><span class="sxs-lookup"><span data-stu-id="211a7-103">Create ContactFolder</span></span>

> <span data-ttu-id="211a7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="211a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="211a7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="211a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="211a7-106">ユーザーの既定の連絡先フォルダーの下に新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="211a7-106">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="211a7-107">また、[指定した連絡先フォルダーの子として新しい contactfolder を作成](contactfolder-post-childfolders.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="211a7-107">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="211a7-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="211a7-108">Permissions</span></span>
<span data-ttu-id="211a7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="211a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="211a7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="211a7-111">Permission type</span></span>      | <span data-ttu-id="211a7-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="211a7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="211a7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="211a7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="211a7-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="211a7-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="211a7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="211a7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="211a7-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="211a7-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="211a7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="211a7-117">Application</span></span> | <span data-ttu-id="211a7-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="211a7-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="211a7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="211a7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="211a7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="211a7-120">Request headers</span></span>
| <span data-ttu-id="211a7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="211a7-121">Header</span></span>       | <span data-ttu-id="211a7-122">値</span><span class="sxs-lookup"><span data-stu-id="211a7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="211a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="211a7-123">Authorization</span></span>  | <span data-ttu-id="211a7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="211a7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="211a7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="211a7-126">Content-Type</span></span>  | <span data-ttu-id="211a7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="211a7-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="211a7-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="211a7-128">Request body</span></span>
<span data-ttu-id="211a7-129">要求本文で、[ContactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="211a7-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="211a7-130">応答</span><span class="sxs-lookup"><span data-stu-id="211a7-130">Response</span></span>

<span data-ttu-id="211a7-131">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [ContactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="211a7-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="211a7-132">例</span><span class="sxs-lookup"><span data-stu-id="211a7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="211a7-133">要求</span><span class="sxs-lookup"><span data-stu-id="211a7-133">Request</span></span>
<span data-ttu-id="211a7-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="211a7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="211a7-135">要求本文で、[contactFolder](../resources/contactfolder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="211a7-135">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="211a7-136">応答</span><span class="sxs-lookup"><span data-stu-id="211a7-136">Response</span></span>
<span data-ttu-id="211a7-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="211a7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
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
