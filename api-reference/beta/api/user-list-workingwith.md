---
title: リスト workingWith
description: ユーザーが作業しているユーザーのリストについて、計算された洞察。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 587a9e34db293a738e1242b3d41406bb15990834
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987482"
---
# <a name="list-workingwith"></a><span data-ttu-id="40c5e-103">リスト workingWith</span><span class="sxs-lookup"><span data-stu-id="40c5e-103">List workingWith</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40c5e-104">ユーザーが作業しているユーザーのリストについて、計算された洞察。</span><span class="sxs-lookup"><span data-stu-id="40c5e-104">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="40c5e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="40c5e-105">Permissions</span></span>
<span data-ttu-id="40c5e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40c5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40c5e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40c5e-108">Permission type</span></span>      | <span data-ttu-id="40c5e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="40c5e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40c5e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40c5e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40c5e-111">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="40c5e-111">User.Read.All</span></span>    |
|<span data-ttu-id="40c5e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40c5e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40c5e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40c5e-113">Not supported.</span></span>    |
|<span data-ttu-id="40c5e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40c5e-114">Application</span></span> | <span data-ttu-id="40c5e-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="40c5e-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40c5e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40c5e-116">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40c5e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="40c5e-117">Optional query parameters</span></span>
<span data-ttu-id="40c5e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="40c5e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40c5e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40c5e-119">Request headers</span></span>
| <span data-ttu-id="40c5e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40c5e-120">Header</span></span>         | <span data-ttu-id="40c5e-121">値</span><span class="sxs-lookup"><span data-stu-id="40c5e-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="40c5e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40c5e-122">Authorization</span></span>  | <span data-ttu-id="40c5e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="40c5e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40c5e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40c5e-125">Content-Type</span></span>   | <span data-ttu-id="40c5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40c5e-126">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="40c5e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="40c5e-127">Request body</span></span>
<span data-ttu-id="40c5e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="40c5e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40c5e-129">応答</span><span class="sxs-lookup"><span data-stu-id="40c5e-129">Response</span></span>

<span data-ttu-id="40c5e-130">成功した場合、このメソッドは 200 OK 応答コードと、応答本文で[User](../resources/user.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="40c5e-130">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40c5e-131">例</span><span class="sxs-lookup"><span data-stu-id="40c5e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40c5e-132">要求</span><span class="sxs-lookup"><span data-stu-id="40c5e-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="40c5e-133">応答</span><span class="sxs-lookup"><span data-stu-id="40c5e-133">Response</span></span>
<span data-ttu-id="40c5e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40c5e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
