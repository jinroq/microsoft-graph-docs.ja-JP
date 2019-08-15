---
title: 'servicePrincipal: getMemberObjects'
description: このサービスプリンシパルがメンバーになっているグループとディレクトリロールの一覧を取得します。  このチェックは推移的です。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 23e223d2ce621217911b478b464d10a8c6392350
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410311"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="ac5c8-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="ac5c8-104">servicePrincipal: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac5c8-105">このサービスプリンシパルがメンバーになっているグループとディレクトリロールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ac5c8-105">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="ac5c8-106">このチェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="ac5c8-106">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac5c8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ac5c8-107">Permissions</span></span>
<span data-ttu-id="ac5c8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac5c8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac5c8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac5c8-110">Permission type</span></span>      | <span data-ttu-id="ac5c8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac5c8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac5c8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac5c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ac5c8-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac5c8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ac5c8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac5c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac5c8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac5c8-115">Not supported.</span></span>    |
|<span data-ttu-id="ac5c8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac5c8-116">Application</span></span> | <span data-ttu-id="ac5c8-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac5c8-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac5c8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac5c8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="ac5c8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac5c8-119">Request headers</span></span>
| <span data-ttu-id="ac5c8-120">名前</span><span class="sxs-lookup"><span data-stu-id="ac5c8-120">Name</span></span>       | <span data-ttu-id="ac5c8-121">型</span><span class="sxs-lookup"><span data-stu-id="ac5c8-121">Type</span></span> | <span data-ttu-id="ac5c8-122">説明</span><span class="sxs-lookup"><span data-stu-id="ac5c8-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ac5c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac5c8-123">Authorization</span></span>  | <span data-ttu-id="ac5c8-124">string</span><span class="sxs-lookup"><span data-stu-id="ac5c8-124">string</span></span>  | <span data-ttu-id="ac5c8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ac5c8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac5c8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac5c8-127">Request body</span></span>
<span data-ttu-id="ac5c8-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ac5c8-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ac5c8-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ac5c8-129">Parameter</span></span>    | <span data-ttu-id="ac5c8-130">型</span><span class="sxs-lookup"><span data-stu-id="ac5c8-130">Type</span></span>   |<span data-ttu-id="ac5c8-131">説明</span><span class="sxs-lookup"><span data-stu-id="ac5c8-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac5c8-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ac5c8-132">securityEnabledOnly</span></span>|<span data-ttu-id="ac5c8-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac5c8-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="ac5c8-134">応答</span><span class="sxs-lookup"><span data-stu-id="ac5c8-134">Response</span></span>

<span data-ttu-id="ac5c8-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ac5c8-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac5c8-136">例</span><span class="sxs-lookup"><span data-stu-id="ac5c8-136">Example</span></span>
<span data-ttu-id="ac5c8-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ac5c8-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ac5c8-138">要求</span><span class="sxs-lookup"><span data-stu-id="ac5c8-138">Request</span></span>
<span data-ttu-id="ac5c8-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ac5c8-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ac5c8-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ac5c8-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ac5c8-141">C#</span><span class="sxs-lookup"><span data-stu-id="ac5c8-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac5c8-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac5c8-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ac5c8-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="ac5c8-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ac5c8-144">応答</span><span class="sxs-lookup"><span data-stu-id="ac5c8-144">Response</span></span>
<span data-ttu-id="ac5c8-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ac5c8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
