---
title: 上司を一覧表示する
description: ユーザーの上司を取得します。ユーザーの上司として割り当てられているユーザーまたは連絡先を返します。
ms.openlocfilehash: 3601b7c13eb97b288cc65e927432bd420105970a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069128"
---
# <a name="list-manager"></a><span data-ttu-id="4be21-104">上司を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4be21-104">List manager</span></span>

> <span data-ttu-id="4be21-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4be21-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4be21-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4be21-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4be21-p103">ユーザーの上司を取得します。ユーザーの上司として割り当てられているユーザーまたは連絡先を返します。</span><span class="sxs-lookup"><span data-stu-id="4be21-p103">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="4be21-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4be21-109">Permissions</span></span>
<span data-ttu-id="4be21-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4be21-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4be21-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4be21-112">Permission type</span></span>      | <span data-ttu-id="4be21-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4be21-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4be21-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4be21-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4be21-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4be21-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4be21-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4be21-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4be21-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4be21-117">Not supported.</span></span>    |
|<span data-ttu-id="4be21-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4be21-118">Application</span></span> | <span data-ttu-id="4be21-119">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be21-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4be21-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4be21-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4be21-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4be21-121">Optional query parameters</span></span>
<span data-ttu-id="4be21-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4be21-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4be21-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4be21-123">Request headers</span></span>
| <span data-ttu-id="4be21-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4be21-124">Header</span></span>       | <span data-ttu-id="4be21-125">値</span><span class="sxs-lookup"><span data-stu-id="4be21-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4be21-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4be21-126">Authorization</span></span>  | <span data-ttu-id="4be21-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4be21-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4be21-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4be21-129">Content-Type</span></span>   | <span data-ttu-id="4be21-130">application/json</span><span class="sxs-lookup"><span data-stu-id="4be21-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4be21-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="4be21-131">Request body</span></span>
<span data-ttu-id="4be21-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4be21-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4be21-133">応答</span><span class="sxs-lookup"><span data-stu-id="4be21-133">Response</span></span>

<span data-ttu-id="4be21-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4be21-134">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4be21-135">例</span><span class="sxs-lookup"><span data-stu-id="4be21-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4be21-136">要求</span><span class="sxs-lookup"><span data-stu-id="4be21-136">Request</span></span>
<span data-ttu-id="4be21-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4be21-137">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="4be21-138">応答</span><span class="sxs-lookup"><span data-stu-id="4be21-138">Response</span></span>
<span data-ttu-id="4be21-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4be21-139">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->