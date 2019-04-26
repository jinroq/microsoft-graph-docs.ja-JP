---
title: childFolders を一覧表示する
description: '指定したフォルダーの下のフォルダー コレクションを取得します。 `.../me/MailFolders`ショートカットを使用してトップレベルを取得できます。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f551e78cd7c713554b8283542f50c1ee6da05556
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338727"
---
# <a name="list-childfolders"></a><span data-ttu-id="fa26d-104">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fa26d-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa26d-p102">指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="fa26d-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa26d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fa26d-107">Permissions</span></span>

<span data-ttu-id="fa26d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa26d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa26d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa26d-110">Permission type</span></span>                        | <span data-ttu-id="fa26d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa26d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="fa26d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa26d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa26d-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa26d-113">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="fa26d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa26d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa26d-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa26d-115">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="fa26d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa26d-116">Application</span></span>                            | <span data-ttu-id="fa26d-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa26d-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="fa26d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa26d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa26d-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fa26d-119">Optional query parameters</span></span>

<span data-ttu-id="fa26d-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fa26d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa26d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa26d-121">Request headers</span></span>

| <span data-ttu-id="fa26d-122">名前</span><span class="sxs-lookup"><span data-stu-id="fa26d-122">Name</span></span>          | <span data-ttu-id="fa26d-123">型</span><span class="sxs-lookup"><span data-stu-id="fa26d-123">Type</span></span>   | <span data-ttu-id="fa26d-124">説明</span><span class="sxs-lookup"><span data-stu-id="fa26d-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="fa26d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa26d-125">Authorization</span></span> | <span data-ttu-id="fa26d-126">string</span><span class="sxs-lookup"><span data-stu-id="fa26d-126">string</span></span> | <span data-ttu-id="fa26d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fa26d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa26d-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa26d-129">Request body</span></span>

<span data-ttu-id="fa26d-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fa26d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa26d-131">応答</span><span class="sxs-lookup"><span data-stu-id="fa26d-131">Response</span></span>

<span data-ttu-id="fa26d-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fa26d-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa26d-133">例</span><span class="sxs-lookup"><span data-stu-id="fa26d-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="fa26d-134">例 1: メールフォルダーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fa26d-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="fa26d-135">要求</span><span class="sxs-lookup"><span data-stu-id="fa26d-135">Request</span></span>

<span data-ttu-id="fa26d-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa26d-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="fa26d-137">応答</span><span class="sxs-lookup"><span data-stu-id="fa26d-137">Response</span></span>

<span data-ttu-id="fa26d-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa26d-138">The following is an example of the response.</span></span>

> <span data-ttu-id="fa26d-139">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="fa26d-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fa26d-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fa26d-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="fa26d-141">例 2: メール検索フォルダーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fa26d-141">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="fa26d-142">要求</span><span class="sxs-lookup"><span data-stu-id="fa26d-142">Request</span></span>

<span data-ttu-id="fa26d-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa26d-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="fa26d-144">応答</span><span class="sxs-lookup"><span data-stu-id="fa26d-144">Response</span></span>

<span data-ttu-id="fa26d-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fa26d-145">The following is an example of the response.</span></span>

> <span data-ttu-id="fa26d-146">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="fa26d-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fa26d-147">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fa26d-147">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMz",
      "displayName": "Get MyAnalytics",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 6,
      "totalItemCount": 6,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'MyAnalytics')"
    },
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMy",
      "displayName": "Action Required",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 4,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'ACTION REQUIRED')"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
