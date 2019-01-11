---
title: childFolders を一覧表示する
description: '指定したフォルダーの下のフォルダーのコレクションを取得します。 使用することができます、 `.../me/MailFolders` 、最上位レベルを取得するショートカット '
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 1d1a002bef6d1e16c48cc484211abe752e4adbe7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819916"
---
# <a name="list-childfolders"></a><span data-ttu-id="2b95d-104">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2b95d-104">List childFolders</span></span>

<span data-ttu-id="2b95d-p102">指定したフォルダーの下のフォルダーのコレクションを取得します。`.../me/MailFolders` ショートカットを使用して、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="2b95d-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b95d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b95d-107">Permissions</span></span>
<span data-ttu-id="2b95d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b95d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b95d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b95d-110">Permission type</span></span>      | <span data-ttu-id="2b95d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b95d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b95d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b95d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b95d-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b95d-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2b95d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b95d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b95d-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b95d-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2b95d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b95d-116">Application</span></span> | <span data-ttu-id="2b95d-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b95d-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b95d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b95d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2b95d-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2b95d-119">Optional query parameters</span></span>
<span data-ttu-id="2b95d-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b95d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2b95d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b95d-121">Request headers</span></span>
| <span data-ttu-id="2b95d-122">名前</span><span class="sxs-lookup"><span data-stu-id="2b95d-122">Name</span></span>       | <span data-ttu-id="2b95d-123">種類</span><span class="sxs-lookup"><span data-stu-id="2b95d-123">Type</span></span> | <span data-ttu-id="2b95d-124">説明</span><span class="sxs-lookup"><span data-stu-id="2b95d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2b95d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b95d-125">Authorization</span></span>  | <span data-ttu-id="2b95d-126">string</span><span class="sxs-lookup"><span data-stu-id="2b95d-126">string</span></span>  | <span data-ttu-id="2b95d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2b95d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b95d-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b95d-129">Request body</span></span>
<span data-ttu-id="2b95d-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2b95d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b95d-131">応答</span><span class="sxs-lookup"><span data-stu-id="2b95d-131">Response</span></span>

<span data-ttu-id="2b95d-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2b95d-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b95d-133">例</span><span class="sxs-lookup"><span data-stu-id="2b95d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b95d-134">要求</span><span class="sxs-lookup"><span data-stu-id="2b95d-134">Request</span></span>
<span data-ttu-id="2b95d-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b95d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="2b95d-136">応答</span><span class="sxs-lookup"><span data-stu-id="2b95d-136">Response</span></span>
<span data-ttu-id="2b95d-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2b95d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
