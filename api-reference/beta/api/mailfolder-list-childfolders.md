---
title: childFolders を一覧表示する
description: '指定したフォルダーの下のフォルダーのコレクションを取得します。 使用することができます、 `.../me/MailFolders` 、最上位レベルを取得するショートカット '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9d54828b97bb82c9ce0ee9eceeee86a4aa975c3d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512550"
---
# <a name="list-childfolders"></a><span data-ttu-id="a6df2-104">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a6df2-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6df2-p102">指定したフォルダーの下のフォルダーのコレクションを取得します。`.../me/MailFolders` ショートカットを使用して、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="a6df2-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6df2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6df2-107">Permissions</span></span>
<span data-ttu-id="a6df2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6df2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6df2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6df2-110">Permission type</span></span>      | <span data-ttu-id="a6df2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6df2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6df2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6df2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6df2-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6df2-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a6df2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6df2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6df2-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6df2-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a6df2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6df2-116">Application</span></span> | <span data-ttu-id="a6df2-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6df2-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6df2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6df2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6df2-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a6df2-119">Optional query parameters</span></span>
<span data-ttu-id="a6df2-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a6df2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6df2-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6df2-121">Request headers</span></span>
| <span data-ttu-id="a6df2-122">名前</span><span class="sxs-lookup"><span data-stu-id="a6df2-122">Name</span></span>       | <span data-ttu-id="a6df2-123">型</span><span class="sxs-lookup"><span data-stu-id="a6df2-123">Type</span></span> | <span data-ttu-id="a6df2-124">説明</span><span class="sxs-lookup"><span data-stu-id="a6df2-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a6df2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6df2-125">Authorization</span></span>  | <span data-ttu-id="a6df2-126">string</span><span class="sxs-lookup"><span data-stu-id="a6df2-126">string</span></span>  | <span data-ttu-id="a6df2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a6df2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6df2-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6df2-129">Request body</span></span>
<span data-ttu-id="a6df2-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a6df2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6df2-131">応答</span><span class="sxs-lookup"><span data-stu-id="a6df2-131">Response</span></span>
<span data-ttu-id="a6df2-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a6df2-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="a6df2-133">例 1</span><span class="sxs-lookup"><span data-stu-id="a6df2-133">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="a6df2-134">要求 1</span><span class="sxs-lookup"><span data-stu-id="a6df2-134">Request 1</span></span>
<span data-ttu-id="a6df2-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6df2-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

#### <a name="response-1"></a><span data-ttu-id="a6df2-136">応答 1</span><span class="sxs-lookup"><span data-stu-id="a6df2-136">Response 1</span></span>
<span data-ttu-id="a6df2-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6df2-137">The following is an example of the response.</span></span>
><span data-ttu-id="a6df2-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a6df2-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a6df2-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a6df2-139">All the properties will be returned from an actual call.</span></span>

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

## <a name="example-2"></a><span data-ttu-id="a6df2-140">例 2</span><span class="sxs-lookup"><span data-stu-id="a6df2-140">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="a6df2-141">要求 2</span><span class="sxs-lookup"><span data-stu-id="a6df2-141">Request 2</span></span>
<span data-ttu-id="a6df2-142">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6df2-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response-2"></a><span data-ttu-id="a6df2-143">応答 2</span><span class="sxs-lookup"><span data-stu-id="a6df2-143">Response 2</span></span>
<span data-ttu-id="a6df2-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6df2-144">The following is an example of the response.</span></span>
><span data-ttu-id="a6df2-145">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a6df2-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a6df2-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a6df2-146">All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
