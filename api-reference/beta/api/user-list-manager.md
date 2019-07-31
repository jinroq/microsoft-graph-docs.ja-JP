---
title: 上司を一覧表示する
description: ユーザーの上司を取得します。 ユーザーの上司として割り当てられているユーザーまたは連絡先を返します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 70e2baaec1e727f78a0cbde21e5149979ea4224a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996204"
---
# <a name="list-manager"></a><span data-ttu-id="83188-104">上司を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="83188-104">List manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83188-105">ユーザーの上司を取得します。</span><span class="sxs-lookup"><span data-stu-id="83188-105">Get user's manager.</span></span> <span data-ttu-id="83188-106">ユーザーの上司として割り当てられているユーザーまたは連絡先を返します。</span><span class="sxs-lookup"><span data-stu-id="83188-106">Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="83188-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83188-107">Permissions</span></span>
<span data-ttu-id="83188-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83188-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83188-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83188-110">Permission type</span></span>      | <span data-ttu-id="83188-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83188-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83188-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83188-112">Delegated (work or school account)</span></span> | <span data-ttu-id="83188-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83188-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83188-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83188-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83188-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83188-115">Not supported.</span></span>    |
|<span data-ttu-id="83188-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83188-116">Application</span></span> | <span data-ttu-id="83188-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83188-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83188-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83188-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83188-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="83188-119">Optional query parameters</span></span>
<span data-ttu-id="83188-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83188-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="83188-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83188-121">Request headers</span></span>
| <span data-ttu-id="83188-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83188-122">Header</span></span>       | <span data-ttu-id="83188-123">値</span><span class="sxs-lookup"><span data-stu-id="83188-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="83188-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="83188-124">Authorization</span></span>  | <span data-ttu-id="83188-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="83188-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="83188-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83188-127">Content-Type</span></span>   | <span data-ttu-id="83188-128">application/json</span><span class="sxs-lookup"><span data-stu-id="83188-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83188-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="83188-129">Request body</span></span>
<span data-ttu-id="83188-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83188-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83188-131">応答</span><span class="sxs-lookup"><span data-stu-id="83188-131">Response</span></span>

<span data-ttu-id="83188-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="83188-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83188-133">例</span><span class="sxs-lookup"><span data-stu-id="83188-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83188-134">要求</span><span class="sxs-lookup"><span data-stu-id="83188-134">Request</span></span>
<span data-ttu-id="83188-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83188-135">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="83188-136">応答</span><span class="sxs-lookup"><span data-stu-id="83188-136">Response</span></span>
<span data-ttu-id="83188-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="83188-137">Here is an example of the response.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
