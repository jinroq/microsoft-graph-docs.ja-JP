---
title: mailFolder を取得する
description: メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eee7adf677696fbf2dc969262604b817c7cddabe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529909"
---
# <a name="get-mailfolder"></a><span data-ttu-id="09e2b-103">mailFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="09e2b-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09e2b-104">メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="09e2b-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="09e2b-105">2 つシナリオは、アプリケーションが別のユーザーのメール フォルダーを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="09e2b-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="09e2b-106">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="09e2b-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="09e2b-107">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任を実行し、別のユーザーは、そのユーザーのメール フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与えを実行します。</span><span class="sxs-lookup"><span data-stu-id="09e2b-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="09e2b-108">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e2b-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="09e2b-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="09e2b-109">Permissions</span></span>
<span data-ttu-id="09e2b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09e2b-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09e2b-112">Permission type</span></span>      | <span data-ttu-id="09e2b-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="09e2b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09e2b-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09e2b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="09e2b-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09e2b-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="09e2b-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09e2b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09e2b-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09e2b-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="09e2b-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09e2b-118">Application</span></span> | <span data-ttu-id="09e2b-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09e2b-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="09e2b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09e2b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09e2b-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="09e2b-121">Optional query parameters</span></span>
<span data-ttu-id="09e2b-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="09e2b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09e2b-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09e2b-123">Request headers</span></span>
| <span data-ttu-id="09e2b-124">名前</span><span class="sxs-lookup"><span data-stu-id="09e2b-124">Name</span></span>       | <span data-ttu-id="09e2b-125">型</span><span class="sxs-lookup"><span data-stu-id="09e2b-125">Type</span></span> | <span data-ttu-id="09e2b-126">説明</span><span class="sxs-lookup"><span data-stu-id="09e2b-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="09e2b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="09e2b-127">Authorization</span></span>  | <span data-ttu-id="09e2b-128">string</span><span class="sxs-lookup"><span data-stu-id="09e2b-128">string</span></span>  | <span data-ttu-id="09e2b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="09e2b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09e2b-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="09e2b-131">Request body</span></span>
<span data-ttu-id="09e2b-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="09e2b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09e2b-133">応答</span><span class="sxs-lookup"><span data-stu-id="09e2b-133">Response</span></span>
<span data-ttu-id="09e2b-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="09e2b-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="09e2b-135">例 1</span><span class="sxs-lookup"><span data-stu-id="09e2b-135">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="09e2b-136">要求 1</span><span class="sxs-lookup"><span data-stu-id="09e2b-136">Request 1</span></span>
<span data-ttu-id="09e2b-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="09e2b-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-1"></a><span data-ttu-id="09e2b-138">応答 1</span><span class="sxs-lookup"><span data-stu-id="09e2b-138">Response 1</span></span>
<span data-ttu-id="09e2b-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="09e2b-139">The following is an example of the response.</span></span>
 ><span data-ttu-id="09e2b-140">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="09e2b-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="09e2b-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="09e2b-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "Inbox",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

## <a name="example-2"></a><span data-ttu-id="09e2b-142">例 2</span><span class="sxs-lookup"><span data-stu-id="09e2b-142">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="09e2b-143">要求 2</span><span class="sxs-lookup"><span data-stu-id="09e2b-143">Request 2</span></span>
<span data-ttu-id="09e2b-144">次に、要求の検索フォルダーの例を示します。</span><span class="sxs-lookup"><span data-stu-id="09e2b-144">The following is a search folder example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-2"></a><span data-ttu-id="09e2b-145">応答 2</span><span class="sxs-lookup"><span data-stu-id="09e2b-145">Response 2</span></span>
<span data-ttu-id="09e2b-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="09e2b-146">The following is an example of the response.</span></span>
 ><span data-ttu-id="09e2b-147">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="09e2b-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="09e2b-148">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="09e2b-148">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "Inbox",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
