---
title: 'servicePrincipals: リスト ownedObjects。'
description: ServicePrincipal によって所有されているオブジェクトの一覧を取得します。  これには、アプリケーションまたはグループが含まれることがあります。
localization_priority: Normal
ms.openlocfilehash: 9b99643eee693902bbdb10467463c2944f4b6fb0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269007"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="b4978-104">servicePrincipals: リスト ownedObjects。</span><span class="sxs-lookup"><span data-stu-id="b4978-104">servicePrincipals: List ownedObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4978-105">ServicePrincipal によって所有されているオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b4978-105">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="b4978-106">これには、アプリケーションまたはグループが含まれることがあります。</span><span class="sxs-lookup"><span data-stu-id="b4978-106">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4978-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b4978-107">Permissions</span></span>
<span data-ttu-id="b4978-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4978-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4978-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4978-110">Permission type</span></span>      | <span data-ttu-id="b4978-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4978-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4978-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4978-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b4978-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4978-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4978-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4978-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4978-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4978-115">Not supported.</span></span>    |
|<span data-ttu-id="b4978-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4978-116">Application</span></span> | <span data-ttu-id="b4978-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4978-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4978-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4978-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b4978-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b4978-119">Optional query parameters</span></span>
<span data-ttu-id="b4978-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b4978-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4978-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4978-121">Request headers</span></span>
| <span data-ttu-id="b4978-122">名前</span><span class="sxs-lookup"><span data-stu-id="b4978-122">Name</span></span>       | <span data-ttu-id="b4978-123">型</span><span class="sxs-lookup"><span data-stu-id="b4978-123">Type</span></span> | <span data-ttu-id="b4978-124">説明</span><span class="sxs-lookup"><span data-stu-id="b4978-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b4978-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4978-125">Authorization</span></span>  | <span data-ttu-id="b4978-126">string</span><span class="sxs-lookup"><span data-stu-id="b4978-126">string</span></span>  | <span data-ttu-id="b4978-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b4978-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4978-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4978-129">Request body</span></span>
<span data-ttu-id="b4978-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b4978-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4978-131">応答</span><span class="sxs-lookup"><span data-stu-id="b4978-131">Response</span></span>

<span data-ttu-id="b4978-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b4978-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4978-133">例</span><span class="sxs-lookup"><span data-stu-id="b4978-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4978-134">要求</span><span class="sxs-lookup"><span data-stu-id="b4978-134">Request</span></span>
<span data-ttu-id="b4978-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4978-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="b4978-136">応答</span><span class="sxs-lookup"><span data-stu-id="b4978-136">Response</span></span>
<span data-ttu-id="b4978-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b4978-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b4978-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="b4978-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b4978-141">C#</span><span class="sxs-lookup"><span data-stu-id="b4978-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_ownedobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4978-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="b4978-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_ownedobjects-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b4978-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="b4978-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_ownedobjects-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-ownedobjects.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/serviceprincipal-list-ownedobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list-ownedobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
