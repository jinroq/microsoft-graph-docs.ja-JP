---
title: childFolders を一覧表示する
description: '指定したフォルダーの下のフォルダーのコレクションを取得します。 使用することができます、 `.../me/MailFolders` 、最上位レベルを取得するショートカット '
author: angelgolfer-ms
ms.openlocfilehash: b852e245ee0b553d83e144eb42a719060837ef68
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351668"
---
# <a name="list-childfolders"></a><span data-ttu-id="98aef-104">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="98aef-104">List childFolders</span></span>

> <span data-ttu-id="98aef-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="98aef-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98aef-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98aef-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98aef-p103">指定したフォルダーの下のフォルダーのコレクションを取得します。`.../me/MailFolders` ショートカットを使用して、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="98aef-p103">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="98aef-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="98aef-109">Permissions</span></span>
<span data-ttu-id="98aef-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98aef-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98aef-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98aef-112">Permission type</span></span>      | <span data-ttu-id="98aef-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="98aef-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98aef-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98aef-114">Delegated (work or school account)</span></span> | <span data-ttu-id="98aef-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98aef-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="98aef-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98aef-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98aef-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98aef-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="98aef-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98aef-118">Application</span></span> | <span data-ttu-id="98aef-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98aef-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="98aef-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98aef-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98aef-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="98aef-121">Optional query parameters</span></span>
<span data-ttu-id="98aef-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="98aef-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98aef-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98aef-123">Request headers</span></span>
| <span data-ttu-id="98aef-124">名前</span><span class="sxs-lookup"><span data-stu-id="98aef-124">Name</span></span>       | <span data-ttu-id="98aef-125">種類</span><span class="sxs-lookup"><span data-stu-id="98aef-125">Type</span></span> | <span data-ttu-id="98aef-126">説明</span><span class="sxs-lookup"><span data-stu-id="98aef-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="98aef-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="98aef-127">Authorization</span></span>  | <span data-ttu-id="98aef-128">string</span><span class="sxs-lookup"><span data-stu-id="98aef-128">string</span></span>  | <span data-ttu-id="98aef-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="98aef-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98aef-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="98aef-131">Request body</span></span>
<span data-ttu-id="98aef-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="98aef-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98aef-133">応答</span><span class="sxs-lookup"><span data-stu-id="98aef-133">Response</span></span>
<span data-ttu-id="98aef-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="98aef-134">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="98aef-135">例 1</span><span class="sxs-lookup"><span data-stu-id="98aef-135">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="98aef-136">要求 1</span><span class="sxs-lookup"><span data-stu-id="98aef-136">Request 1</span></span>
<span data-ttu-id="98aef-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="98aef-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

#### <a name="response-1"></a><span data-ttu-id="98aef-138">応答 1</span><span class="sxs-lookup"><span data-stu-id="98aef-138">Response 1</span></span>
<span data-ttu-id="98aef-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="98aef-139">The following is an example of the response.</span></span>
><span data-ttu-id="98aef-140">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="98aef-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="98aef-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="98aef-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
        "id": "AAMkAGVmMDEzA",
        "displayName": "Internal Screens",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 2,
        "totalItemCount": 2,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzB",
        "displayName": "Project Falcon",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 5,
        "totalItemCount": 5,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzMA",
        "displayName": "Finder",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 4,
        "unreadItemCount": 0,
        "totalItemCount": 0,
        "wellKnownName": "searchfolders"
    }
  ]
}
```

## <a name="example-2"></a><span data-ttu-id="98aef-142">例 2</span><span class="sxs-lookup"><span data-stu-id="98aef-142">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="98aef-143">要求 2</span><span class="sxs-lookup"><span data-stu-id="98aef-143">Request 2</span></span>
<span data-ttu-id="98aef-144">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="98aef-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response-2"></a><span data-ttu-id="98aef-145">応答 2</span><span class="sxs-lookup"><span data-stu-id="98aef-145">Response 2</span></span>
<span data-ttu-id="98aef-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="98aef-146">The following is an example of the response.</span></span>
><span data-ttu-id="98aef-147">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="98aef-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="98aef-148">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="98aef-148">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
        "id": "AAMkAGVmMDEzA",
        "displayName": "Internal Screens",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 2,
        "totalItemCount": 2,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzB",
        "displayName": "Project Falcon",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 5,
        "totalItemCount": 5,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzMA",
        "displayName": "Finder",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 4,
        "unreadItemCount": 0,
        "totalItemCount": 0,
        "wellKnownName": "searchfolders"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
