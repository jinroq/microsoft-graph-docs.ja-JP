---
title: mailFolder を取得する
description: メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: d2f61152b8edd98aa11fc7c6b34d2c2b04b72f55
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565481"
---
# <a name="get-mailfolder"></a><span data-ttu-id="b9a5c-103">mailFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="b9a5c-103">Get mailFolder</span></span>

<span data-ttu-id="b9a5c-104">メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="b9a5c-105">アプリで別のユーザーのメール フォルダーを取得するシナリオは 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-105">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="b9a5c-106">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="b9a5c-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="b9a5c-107">あるユーザーからアプリに適切な代理[アクセス許可](#permissions)が与えられ、別のユーザーがそのユーザーとメール フォルダーを共有しているか、そのユーザーに代理アクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="b9a5c-108">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="b9a5c-109">権限</span><span class="sxs-lookup"><span data-stu-id="b9a5c-109">Permissions</span></span>
<span data-ttu-id="b9a5c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9a5c-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9a5c-112">Permission type</span></span>      | <span data-ttu-id="b9a5c-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9a5c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9a5c-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9a5c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b9a5c-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9a5c-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b9a5c-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9a5c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a5c-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9a5c-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b9a5c-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9a5c-118">Application</span></span> | <span data-ttu-id="b9a5c-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9a5c-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9a5c-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9a5c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9a5c-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b9a5c-121">Optional query parameters</span></span>
<span data-ttu-id="b9a5c-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b9a5c-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9a5c-123">Request headers</span></span>
| <span data-ttu-id="b9a5c-124">名前</span><span class="sxs-lookup"><span data-stu-id="b9a5c-124">Name</span></span>       | <span data-ttu-id="b9a5c-125">型</span><span class="sxs-lookup"><span data-stu-id="b9a5c-125">Type</span></span> | <span data-ttu-id="b9a5c-126">説明</span><span class="sxs-lookup"><span data-stu-id="b9a5c-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b9a5c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9a5c-127">Authorization</span></span>  | <span data-ttu-id="b9a5c-128">string</span><span class="sxs-lookup"><span data-stu-id="b9a5c-128">string</span></span>  | <span data-ttu-id="b9a5c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9a5c-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9a5c-131">Request body</span></span>
<span data-ttu-id="b9a5c-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a5c-133">応答</span><span class="sxs-lookup"><span data-stu-id="b9a5c-133">Response</span></span>

<span data-ttu-id="b9a5c-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9a5c-135">例</span><span class="sxs-lookup"><span data-stu-id="b9a5c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9a5c-136">要求</span><span class="sxs-lookup"><span data-stu-id="b9a5c-136">Request</span></span>
<span data-ttu-id="b9a5c-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="b9a5c-138">応答</span><span class="sxs-lookup"><span data-stu-id="b9a5c-138">Response</span></span>
<span data-ttu-id="b9a5c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b9a5c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
