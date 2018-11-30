---
title: リストの操作
description: ユーザーが使用されているユーザーのリストの計算の把握。
ms.openlocfilehash: ce464667c66a430f20c60485712c649120dac4a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068131"
---
# <a name="list-workingwith"></a><span data-ttu-id="e2460-103">リストの操作</span><span class="sxs-lookup"><span data-stu-id="e2460-103">List workingWith</span></span>

> <span data-ttu-id="e2460-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e2460-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2460-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2460-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2460-106">ユーザーが使用されているユーザーのリストの計算の把握。</span><span class="sxs-lookup"><span data-stu-id="e2460-106">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2460-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2460-107">Permissions</span></span>
<span data-ttu-id="e2460-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2460-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2460-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2460-110">Permission type</span></span>      | <span data-ttu-id="e2460-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2460-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2460-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2460-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2460-113">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2460-113">User.Read.All</span></span>    |
|<span data-ttu-id="e2460-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2460-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2460-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2460-115">Not supported.</span></span>    |
|<span data-ttu-id="e2460-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2460-116">Application</span></span> | <span data-ttu-id="e2460-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2460-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2460-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2460-118">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2460-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e2460-119">Optional query parameters</span></span>
<span data-ttu-id="e2460-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e2460-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2460-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2460-121">Request headers</span></span>
| <span data-ttu-id="e2460-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2460-122">Header</span></span>         | <span data-ttu-id="e2460-123">値</span><span class="sxs-lookup"><span data-stu-id="e2460-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="e2460-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2460-124">Authorization</span></span>  | <span data-ttu-id="e2460-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e2460-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e2460-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2460-127">Content-Type</span></span>   | <span data-ttu-id="e2460-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e2460-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="e2460-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2460-129">Request body</span></span>
<span data-ttu-id="e2460-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e2460-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2460-131">応答</span><span class="sxs-lookup"><span data-stu-id="e2460-131">Response</span></span>

<span data-ttu-id="e2460-132">成功した場合、このメソッドは、応答の本体で、200 OK 応答コードと[ユーザー](../resources/user.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e2460-132">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2460-133">例</span><span class="sxs-lookup"><span data-stu-id="e2460-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2460-134">要求</span><span class="sxs-lookup"><span data-stu-id="e2460-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="e2460-135">応答</span><span class="sxs-lookup"><span data-stu-id="e2460-135">Response</span></span>
<span data-ttu-id="e2460-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e2460-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "id": "id-value",
  "preferredName": "preferredName-value",
  "Email": "Email-value",
}
```