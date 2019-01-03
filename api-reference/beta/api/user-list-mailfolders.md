---
title: mailFolders を一覧表示する　
description: サインインしているユーザーのメールボックス内のすべてのメール フォルダーを取得します。
ms.openlocfilehash: c93c870447e2414dfbdeb4e248f65c3aa5e0a4a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072196"
---
# <a name="list-mailfolders"></a><span data-ttu-id="eb289-103">mailFolders を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="eb289-103">List mailFolders</span></span>

> <span data-ttu-id="eb289-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eb289-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb289-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb289-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb289-106">サインインしているユーザーのメールボックス内のすべてのメール フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="eb289-106">Get all the mail folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb289-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eb289-107">Permissions</span></span>
<span data-ttu-id="eb289-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb289-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb289-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb289-110">Permission type</span></span>      | <span data-ttu-id="eb289-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb289-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb289-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb289-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb289-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb289-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eb289-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb289-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb289-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb289-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="eb289-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb289-116">Application</span></span> | <span data-ttu-id="eb289-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb289-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb289-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb289-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eb289-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="eb289-119">Optional query parameters</span></span>
<span data-ttu-id="eb289-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="eb289-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eb289-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb289-121">Request headers</span></span>
| <span data-ttu-id="eb289-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb289-122">Header</span></span>       | <span data-ttu-id="eb289-123">値</span><span class="sxs-lookup"><span data-stu-id="eb289-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb289-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb289-124">Authorization</span></span>  | <span data-ttu-id="eb289-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eb289-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eb289-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb289-127">Content-Type</span></span>   | <span data-ttu-id="eb289-128">application/json</span><span class="sxs-lookup"><span data-stu-id="eb289-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb289-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="eb289-129">Request body</span></span>
<span data-ttu-id="eb289-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eb289-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb289-131">応答</span><span class="sxs-lookup"><span data-stu-id="eb289-131">Response</span></span>

<span data-ttu-id="eb289-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="eb289-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eb289-133">例</span><span class="sxs-lookup"><span data-stu-id="eb289-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb289-134">要求</span><span class="sxs-lookup"><span data-stu-id="eb289-134">Request</span></span>
<span data-ttu-id="eb289-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eb289-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="eb289-136">応答</span><span class="sxs-lookup"><span data-stu-id="eb289-136">Response</span></span>
<span data-ttu-id="eb289-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eb289-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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