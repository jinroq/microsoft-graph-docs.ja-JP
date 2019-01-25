---
title: リストの操作
description: ユーザーが使用されているユーザーのリストの計算の把握。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ca5fdd4602d109d98002c0ef54fde5ad341e1903
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521622"
---
# <a name="list-workingwith"></a><span data-ttu-id="68890-103">リストの操作</span><span class="sxs-lookup"><span data-stu-id="68890-103">List workingWith</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68890-104">ユーザーが使用されているユーザーのリストの計算の把握。</span><span class="sxs-lookup"><span data-stu-id="68890-104">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="68890-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="68890-105">Permissions</span></span>
<span data-ttu-id="68890-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68890-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="68890-108">Permission type</span></span>      | <span data-ttu-id="68890-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="68890-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68890-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="68890-110">Delegated (work or school account)</span></span> | <span data-ttu-id="68890-111">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="68890-111">User.Read.All</span></span>    |
|<span data-ttu-id="68890-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="68890-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68890-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68890-113">Not supported.</span></span>    |
|<span data-ttu-id="68890-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="68890-114">Application</span></span> | <span data-ttu-id="68890-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="68890-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68890-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="68890-116">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="68890-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="68890-117">Optional query parameters</span></span>
<span data-ttu-id="68890-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="68890-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68890-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68890-119">Request headers</span></span>
| <span data-ttu-id="68890-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68890-120">Header</span></span>         | <span data-ttu-id="68890-121">値</span><span class="sxs-lookup"><span data-stu-id="68890-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="68890-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="68890-122">Authorization</span></span>  | <span data-ttu-id="68890-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="68890-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="68890-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68890-125">Content-Type</span></span>   | <span data-ttu-id="68890-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68890-126">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="68890-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="68890-127">Request body</span></span>
<span data-ttu-id="68890-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="68890-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68890-129">応答</span><span class="sxs-lookup"><span data-stu-id="68890-129">Response</span></span>

<span data-ttu-id="68890-130">成功した場合、このメソッドは、応答の本体で、200 OK 応答コードと[ユーザー](../resources/user.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="68890-130">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68890-131">例</span><span class="sxs-lookup"><span data-stu-id="68890-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68890-132">要求</span><span class="sxs-lookup"><span data-stu-id="68890-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="68890-133">応答</span><span class="sxs-lookup"><span data-stu-id="68890-133">Response</span></span>
<span data-ttu-id="68890-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="68890-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-workingwith.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
