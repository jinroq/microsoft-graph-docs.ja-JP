---
title: mailFolder を取得する
description: メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af2cc42c2ee72f1a57a1e0f9402209c107e259f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540902"
---
# <a name="get-mailfolder"></a><span data-ttu-id="13ddf-103">mailFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="13ddf-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13ddf-104">メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="13ddf-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="13ddf-105">アプリで別のユーザーのメールフォルダーを取得するには、次の2つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="13ddf-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="13ddf-106">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="13ddf-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="13ddf-107">あるユーザーからアプリに適切な代理[アクセス許可](#permissions)が与えられ、別のユーザーがそのユーザーとメール フォルダーを共有しているか、そのユーザーに代理アクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="13ddf-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="13ddf-108">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13ddf-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="13ddf-109">権限</span><span class="sxs-lookup"><span data-stu-id="13ddf-109">Permissions</span></span>

<span data-ttu-id="13ddf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13ddf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13ddf-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13ddf-112">Permission type</span></span>      | <span data-ttu-id="13ddf-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="13ddf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13ddf-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13ddf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="13ddf-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13ddf-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="13ddf-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13ddf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13ddf-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13ddf-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="13ddf-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13ddf-118">Application</span></span> | <span data-ttu-id="13ddf-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13ddf-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="13ddf-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13ddf-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13ddf-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="13ddf-121">Optional query parameters</span></span>

<span data-ttu-id="13ddf-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="13ddf-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13ddf-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13ddf-123">Request headers</span></span>

| <span data-ttu-id="13ddf-124">名前</span><span class="sxs-lookup"><span data-stu-id="13ddf-124">Name</span></span>          | <span data-ttu-id="13ddf-125">型</span><span class="sxs-lookup"><span data-stu-id="13ddf-125">Type</span></span>   | <span data-ttu-id="13ddf-126">説明</span><span class="sxs-lookup"><span data-stu-id="13ddf-126">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="13ddf-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="13ddf-127">Authorization</span></span> | <span data-ttu-id="13ddf-128">string</span><span class="sxs-lookup"><span data-stu-id="13ddf-128">string</span></span> | <span data-ttu-id="13ddf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="13ddf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13ddf-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="13ddf-131">Request body</span></span>

<span data-ttu-id="13ddf-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="13ddf-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13ddf-133">応答</span><span class="sxs-lookup"><span data-stu-id="13ddf-133">Response</span></span>

<span data-ttu-id="13ddf-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="13ddf-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13ddf-135">例</span><span class="sxs-lookup"><span data-stu-id="13ddf-135">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="13ddf-136">例 1: メールフォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="13ddf-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="13ddf-137">要求</span><span class="sxs-lookup"><span data-stu-id="13ddf-137">Request</span></span>

<span data-ttu-id="13ddf-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13ddf-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="13ddf-139">応答</span><span class="sxs-lookup"><span data-stu-id="13ddf-139">Response</span></span>

<span data-ttu-id="13ddf-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13ddf-140">The following is an example of the response.</span></span>

> <span data-ttu-id="13ddf-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="13ddf-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="13ddf-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="13ddf-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="13ddf-143">例 2: メール検索フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="13ddf-143">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="13ddf-144">要求</span><span class="sxs-lookup"><span data-stu-id="13ddf-144">Request</span></span>

<span data-ttu-id="13ddf-145">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13ddf-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```

#### <a name="response"></a><span data-ttu-id="13ddf-146">応答</span><span class="sxs-lookup"><span data-stu-id="13ddf-146">Response</span></span>

<span data-ttu-id="13ddf-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13ddf-147">The following is an example of the response.</span></span>

> <span data-ttu-id="13ddf-148">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="13ddf-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="13ddf-149">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="13ddf-149">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzN",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 0,
  "unreadItemCount": 6,
  "totalItemCount": 6,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzM"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
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
