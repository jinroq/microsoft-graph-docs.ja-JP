---
title: Get contactFolder
description: 連絡先フォルダー ID を使用して連絡先フォルダーを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 47d5ba998edc35505d8c7fb6a34f2f58d560eb10
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883973"
---
# <a name="get-contactfolder"></a><span data-ttu-id="cdc39-103">Get contactFolder</span><span class="sxs-lookup"><span data-stu-id="cdc39-103">Get contactFolder</span></span>

<span data-ttu-id="cdc39-104">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="cdc39-104">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="cdc39-105">アプリで別のユーザーの連絡先フォルダーを取得するには、次の2つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="cdc39-105">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="cdc39-106">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="cdc39-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="cdc39-107">アプリに「あるユーザーから適切に委任された[アクセス許可](#permissions)」があり、別のユーザーがそのユーザーとコンタクトフォルダーを共有しているか、そのユーザーに委任されたアクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="cdc39-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="cdc39-108">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdc39-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="cdc39-109">権限</span><span class="sxs-lookup"><span data-stu-id="cdc39-109">Permissions</span></span>
<span data-ttu-id="cdc39-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdc39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc39-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cdc39-112">Permission type</span></span>      | <span data-ttu-id="cdc39-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cdc39-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdc39-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cdc39-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cdc39-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdc39-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cdc39-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cdc39-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdc39-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdc39-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cdc39-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cdc39-118">Application</span></span> | <span data-ttu-id="cdc39-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdc39-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdc39-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cdc39-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cdc39-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cdc39-121">Optional query parameters</span></span>
<span data-ttu-id="cdc39-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cdc39-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cdc39-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdc39-123">Request headers</span></span>
| <span data-ttu-id="cdc39-124">名前</span><span class="sxs-lookup"><span data-stu-id="cdc39-124">Name</span></span>       | <span data-ttu-id="cdc39-125">型</span><span class="sxs-lookup"><span data-stu-id="cdc39-125">Type</span></span> | <span data-ttu-id="cdc39-126">説明</span><span class="sxs-lookup"><span data-stu-id="cdc39-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cdc39-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdc39-127">Authorization</span></span>  | <span data-ttu-id="cdc39-128">string</span><span class="sxs-lookup"><span data-stu-id="cdc39-128">string</span></span>  | <span data-ttu-id="cdc39-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cdc39-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdc39-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="cdc39-131">Request body</span></span>
<span data-ttu-id="cdc39-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cdc39-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdc39-133">応答</span><span class="sxs-lookup"><span data-stu-id="cdc39-133">Response</span></span>

<span data-ttu-id="cdc39-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [contactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cdc39-134">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cdc39-135">例</span><span class="sxs-lookup"><span data-stu-id="cdc39-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdc39-136">要求</span><span class="sxs-lookup"><span data-stu-id="cdc39-136">Request</span></span>
<span data-ttu-id="cdc39-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cdc39-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cdc39-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cdc39-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cdc39-139">C#</span><span class="sxs-lookup"><span data-stu-id="cdc39-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cdc39-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="cdc39-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cdc39-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="cdc39-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cdc39-142">Java</span><span class="sxs-lookup"><span data-stu-id="cdc39-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cdc39-143">応答</span><span class="sxs-lookup"><span data-stu-id="cdc39-143">Response</span></span>
<span data-ttu-id="cdc39-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cdc39-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
