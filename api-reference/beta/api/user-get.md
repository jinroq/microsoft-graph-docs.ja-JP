---
title: ユーザーの取得
description: ユーザー オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b0a05ee2e2bd2b4f5d2e66f5c2e0efcf27efb59
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523947"
---
# <a name="get-a-user"></a><span data-ttu-id="19d8c-103">ユーザーの取得</span><span class="sxs-lookup"><span data-stu-id="19d8c-103">Get a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19d8c-104">ユーザー オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="19d8c-104">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="19d8c-105">**ユーザー** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**ユーザー** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="19d8c-105">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="19d8c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19d8c-106">Permissions</span></span>
<span data-ttu-id="19d8c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19d8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19d8c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19d8c-109">Permission type</span></span>      | <span data-ttu-id="19d8c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19d8c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19d8c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19d8c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="19d8c-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19d8c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19d8c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19d8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19d8c-114">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19d8c-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="19d8c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19d8c-115">Application</span></span> | <span data-ttu-id="19d8c-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19d8c-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19d8c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19d8c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="19d8c-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="19d8c-118">Optional query parameters</span></span>
<span data-ttu-id="19d8c-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="19d8c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="19d8c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19d8c-120">Request headers</span></span>
| <span data-ttu-id="19d8c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19d8c-121">Header</span></span>       | <span data-ttu-id="19d8c-122">値</span><span class="sxs-lookup"><span data-stu-id="19d8c-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="19d8c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19d8c-123">Authorization</span></span>  | <span data-ttu-id="19d8c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19d8c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="19d8c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19d8c-126">Content-Type</span></span>   | <span data-ttu-id="19d8c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="19d8c-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19d8c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="19d8c-128">Request body</span></span>
<span data-ttu-id="19d8c-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="19d8c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19d8c-130">応答</span><span class="sxs-lookup"><span data-stu-id="19d8c-130">Response</span></span>

<span data-ttu-id="19d8c-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="19d8c-131">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19d8c-132">例</span><span class="sxs-lookup"><span data-stu-id="19d8c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19d8c-133">要求</span><span class="sxs-lookup"><span data-stu-id="19d8c-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
##### <a name="response"></a><span data-ttu-id="19d8c-134">応答</span><span class="sxs-lookup"><span data-stu-id="19d8c-134">Response</span></span>
<span data-ttu-id="19d8c-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="19d8c-135">Here is an example of the response.</span></span> <span data-ttu-id="19d8c-136">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="19d8c-136">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="19d8c-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="19d8c-137">See also</span></span>

- [<span data-ttu-id="19d8c-138">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="19d8c-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="19d8c-139">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="19d8c-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="19d8c-140">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="19d8c-140">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
