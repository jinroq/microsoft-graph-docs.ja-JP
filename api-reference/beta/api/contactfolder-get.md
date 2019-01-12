---
title: Get contactFolder
description: 連絡先フォルダー ID を使用して連絡先フォルダーを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 86f2adf867737e31d96a75d40f50442b10a468b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985117"
---
# <a name="get-contactfolder"></a><span data-ttu-id="8393f-103">Get contactFolder</span><span class="sxs-lookup"><span data-stu-id="8393f-103">Get contactFolder</span></span>

> <span data-ttu-id="8393f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8393f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8393f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8393f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8393f-106">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="8393f-106">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="8393f-107">2 つシナリオは、アプリケーションが別のユーザーの連絡先フォルダーを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="8393f-107">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="8393f-108">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="8393f-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="8393f-109">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーの連絡先フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="8393f-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="8393f-110">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8393f-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="8393f-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8393f-111">Permissions</span></span>
<span data-ttu-id="8393f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8393f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8393f-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8393f-114">Permission type</span></span>      | <span data-ttu-id="8393f-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8393f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8393f-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8393f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8393f-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8393f-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8393f-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8393f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8393f-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8393f-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8393f-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8393f-120">Application</span></span> | <span data-ttu-id="8393f-121">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8393f-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8393f-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8393f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8393f-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8393f-123">Optional query parameters</span></span>
<span data-ttu-id="8393f-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8393f-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8393f-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8393f-125">Request headers</span></span>
| <span data-ttu-id="8393f-126">名前</span><span class="sxs-lookup"><span data-stu-id="8393f-126">Name</span></span>       | <span data-ttu-id="8393f-127">型</span><span class="sxs-lookup"><span data-stu-id="8393f-127">Type</span></span> | <span data-ttu-id="8393f-128">説明</span><span class="sxs-lookup"><span data-stu-id="8393f-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8393f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8393f-129">Authorization</span></span>  | <span data-ttu-id="8393f-130">string</span><span class="sxs-lookup"><span data-stu-id="8393f-130">string</span></span>  | <span data-ttu-id="8393f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8393f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8393f-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="8393f-133">Request body</span></span>
<span data-ttu-id="8393f-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8393f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8393f-135">応答</span><span class="sxs-lookup"><span data-stu-id="8393f-135">Response</span></span>

<span data-ttu-id="8393f-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [contactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8393f-136">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8393f-137">例</span><span class="sxs-lookup"><span data-stu-id="8393f-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8393f-138">要求</span><span class="sxs-lookup"><span data-stu-id="8393f-138">Request</span></span>
<span data-ttu-id="8393f-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8393f-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="8393f-140">応答</span><span class="sxs-lookup"><span data-stu-id="8393f-140">Response</span></span>
<span data-ttu-id="8393f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8393f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "wellKnownName": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
