---
title: 連絡先を一覧表示する
description: サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得する (`.../me/contacts`) か、指定した連絡先フォルダーから取得します。
localization_priority: Normal
ms.openlocfilehash: a617cae074ee467d0c47ffcc86351a5e4d65e45a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855469"
---
# <a name="list-contacts"></a><span data-ttu-id="ed96e-103">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ed96e-103">List contacts</span></span>

<span data-ttu-id="ed96e-104">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得する (`.../me/contacts`) か、指定した連絡先フォルダーから取得します。</span><span class="sxs-lookup"><span data-stu-id="ed96e-104">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="ed96e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed96e-105">Permissions</span></span>
<span data-ttu-id="ed96e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed96e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed96e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed96e-108">Permission type</span></span>      | <span data-ttu-id="ed96e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed96e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed96e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed96e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed96e-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed96e-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ed96e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed96e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed96e-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed96e-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ed96e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed96e-114">Application</span></span> | <span data-ttu-id="ed96e-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed96e-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed96e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed96e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ed96e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ed96e-117">Optional query parameters</span></span>
<span data-ttu-id="ed96e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ed96e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ed96e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed96e-119">Request headers</span></span>
| <span data-ttu-id="ed96e-120">名前</span><span class="sxs-lookup"><span data-stu-id="ed96e-120">Name</span></span>       | <span data-ttu-id="ed96e-121">種類</span><span class="sxs-lookup"><span data-stu-id="ed96e-121">Type</span></span> | <span data-ttu-id="ed96e-122">説明</span><span class="sxs-lookup"><span data-stu-id="ed96e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ed96e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed96e-123">Authorization</span></span>  | <span data-ttu-id="ed96e-124">string</span><span class="sxs-lookup"><span data-stu-id="ed96e-124">string</span></span>  | <span data-ttu-id="ed96e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed96e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed96e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed96e-127">Request body</span></span>
<span data-ttu-id="ed96e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ed96e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed96e-129">応答</span><span class="sxs-lookup"><span data-stu-id="ed96e-129">Response</span></span>

<span data-ttu-id="ed96e-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contact](../resources/contact.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ed96e-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed96e-131">例</span><span class="sxs-lookup"><span data-stu-id="ed96e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed96e-132">要求</span><span class="sxs-lookup"><span data-stu-id="ed96e-132">Request</span></span>
<span data-ttu-id="ed96e-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed96e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="ed96e-134">応答</span><span class="sxs-lookup"><span data-stu-id="ed96e-134">Response</span></span>
<span data-ttu-id="ed96e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed96e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
