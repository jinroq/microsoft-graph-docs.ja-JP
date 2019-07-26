---
title: チャネルを一覧表示する
description: このチーム内のチャネルの一覧を取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: b4ed0fdeaa101a35bd68c421219b64f45529cc47
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882250"
---
# <a name="list-channels"></a><span data-ttu-id="db29c-103">チャネルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="db29c-103">List channels</span></span>



<span data-ttu-id="db29c-104">このチーム内の[チャネル](../resources/channel.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="db29c-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="db29c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="db29c-105">Permissions</span></span>
<span data-ttu-id="db29c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db29c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="db29c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db29c-108">Permission type</span></span>      | <span data-ttu-id="db29c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="db29c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db29c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db29c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db29c-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db29c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="db29c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db29c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db29c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db29c-113">Not supported.</span></span>    |
|<span data-ttu-id="db29c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db29c-114">Application</span></span> | <span data-ttu-id="db29c-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db29c-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="db29c-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="db29c-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="db29c-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="db29c-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="db29c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db29c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db29c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="db29c-119">Optional query parameters</span></span>
<span data-ttu-id="db29c-120">このメソッドは、応答をカスタマイズするための $filter、$select、および $expand [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="db29c-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db29c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db29c-121">Request headers</span></span>
| <span data-ttu-id="db29c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db29c-122">Header</span></span>       | <span data-ttu-id="db29c-123">値</span><span class="sxs-lookup"><span data-stu-id="db29c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="db29c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="db29c-124">Authorization</span></span>  | <span data-ttu-id="db29c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="db29c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db29c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="db29c-127">Request body</span></span>
<span data-ttu-id="db29c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="db29c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db29c-129">応答</span><span class="sxs-lookup"><span data-stu-id="db29c-129">Response</span></span>

<span data-ttu-id="db29c-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Channel](../resources/channel.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="db29c-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db29c-131">例</span><span class="sxs-lookup"><span data-stu-id="db29c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db29c-132">要求</span><span class="sxs-lookup"><span data-stu-id="db29c-132">Request</span></span>
<span data-ttu-id="db29c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="db29c-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db29c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="db29c-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db29c-135">C#</span><span class="sxs-lookup"><span data-stu-id="db29c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db29c-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="db29c-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db29c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db29c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db29c-138">Java</span><span class="sxs-lookup"><span data-stu-id="db29c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db29c-139">応答</span><span class="sxs-lookup"><span data-stu-id="db29c-139">Response</span></span>
<span data-ttu-id="db29c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="db29c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
