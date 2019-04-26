---
title: mailFolders を一覧表示する　
description: 'サインイン中のユーザーのルート フォルダーからメール フォルダー コレクションを取得します。 '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f92a933cc7b38ac713722a42809b2fe7f44c516f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571325"
---
# <a name="list-mailfolders"></a><span data-ttu-id="83e20-103">mailFolders を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="83e20-103">List mailFolders</span></span>

<span data-ttu-id="83e20-104">サインイン中のユーザーのルート フォルダーからメール フォルダー コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="83e20-104">Get the mail folder collection under the root folder of the signed-in user.</span></span> 
## <a name="permissions"></a><span data-ttu-id="83e20-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83e20-105">Permissions</span></span>
<span data-ttu-id="83e20-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83e20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83e20-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83e20-108">Permission type</span></span>      | <span data-ttu-id="83e20-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83e20-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83e20-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83e20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83e20-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83e20-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="83e20-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83e20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83e20-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83e20-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="83e20-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83e20-114">Application</span></span> | <span data-ttu-id="83e20-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83e20-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="83e20-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83e20-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83e20-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="83e20-117">Optional query parameters</span></span>
<span data-ttu-id="83e20-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83e20-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="83e20-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83e20-119">Request headers</span></span>
| <span data-ttu-id="83e20-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83e20-120">Header</span></span>       | <span data-ttu-id="83e20-121">値</span><span class="sxs-lookup"><span data-stu-id="83e20-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83e20-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="83e20-122">Authorization</span></span>  | <span data-ttu-id="83e20-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="83e20-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="83e20-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83e20-125">Content-Type</span></span>   | <span data-ttu-id="83e20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83e20-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83e20-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="83e20-127">Request body</span></span>
<span data-ttu-id="83e20-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83e20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83e20-129">応答</span><span class="sxs-lookup"><span data-stu-id="83e20-129">Response</span></span>

<span data-ttu-id="83e20-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="83e20-130">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83e20-131">例</span><span class="sxs-lookup"><span data-stu-id="83e20-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83e20-132">要求</span><span class="sxs-lookup"><span data-stu-id="83e20-132">Request</span></span>
<span data-ttu-id="83e20-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83e20-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="83e20-134">応答</span><span class="sxs-lookup"><span data-stu-id="83e20-134">Response</span></span>
<span data-ttu-id="83e20-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83e20-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
