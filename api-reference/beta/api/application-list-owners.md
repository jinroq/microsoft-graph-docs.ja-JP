---
title: 所有者を一覧表示する
description: DirectoryObject オブジェクトのリストを取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 154d5350279107671b85fae5b072a538159b01e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945523"
---
# <a name="list-owners"></a><span data-ttu-id="b76ef-103">所有者を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b76ef-103">List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b76ef-104">DirectoryObject オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="b76ef-104">Retrieve a list of directoryObject objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b76ef-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b76ef-105">Permissions</span></span>
<span data-ttu-id="b76ef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b76ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b76ef-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b76ef-108">Permission type</span></span>      | <span data-ttu-id="b76ef-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b76ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b76ef-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b76ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b76ef-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b76ef-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b76ef-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b76ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b76ef-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b76ef-113">Not supported.</span></span>    |
|<span data-ttu-id="b76ef-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b76ef-114">Application</span></span> | <span data-ttu-id="b76ef-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b76ef-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b76ef-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b76ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b76ef-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b76ef-117">Optional query parameters</span></span>
<span data-ttu-id="b76ef-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b76ef-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b76ef-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b76ef-119">Request headers</span></span>
| <span data-ttu-id="b76ef-120">名前</span><span class="sxs-lookup"><span data-stu-id="b76ef-120">Name</span></span>       | <span data-ttu-id="b76ef-121">型</span><span class="sxs-lookup"><span data-stu-id="b76ef-121">Type</span></span> | <span data-ttu-id="b76ef-122">説明</span><span class="sxs-lookup"><span data-stu-id="b76ef-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b76ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b76ef-123">Authorization</span></span>  | <span data-ttu-id="b76ef-124">string</span><span class="sxs-lookup"><span data-stu-id="b76ef-124">string</span></span>  | <span data-ttu-id="b76ef-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b76ef-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b76ef-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b76ef-127">Request body</span></span>
<span data-ttu-id="b76ef-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b76ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b76ef-129">応答</span><span class="sxs-lookup"><span data-stu-id="b76ef-129">Response</span></span>

<span data-ttu-id="b76ef-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b76ef-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b76ef-131">例</span><span class="sxs-lookup"><span data-stu-id="b76ef-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b76ef-132">要求</span><span class="sxs-lookup"><span data-stu-id="b76ef-132">Request</span></span>
<span data-ttu-id="b76ef-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b76ef-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b76ef-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b76ef-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b76ef-135">C#</span><span class="sxs-lookup"><span data-stu-id="b76ef-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b76ef-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b76ef-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b76ef-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="b76ef-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b76ef-138">Java</span><span class="sxs-lookup"><span data-stu-id="b76ef-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b76ef-139">応答</span><span class="sxs-lookup"><span data-stu-id="b76ef-139">Response</span></span>
<span data-ttu-id="b76ef-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b76ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
