---
title: 'servicePrincipal: getMemberGroups'
description: このサービスプリンシパルがメンバーになっているグループの一覧を取得します。  チェックは推移的です。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4a6f1fce9f5995762c120ad14597834b06d8b07a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410324"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="e2a18-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e2a18-104">servicePrincipal: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2a18-105">このサービスプリンシパルがメンバーになっているグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e2a18-105">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="e2a18-106">チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="e2a18-106">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2a18-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2a18-107">Permissions</span></span>
<span data-ttu-id="e2a18-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2a18-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e2a18-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2a18-110">Permission type</span></span>      | <span data-ttu-id="e2a18-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2a18-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2a18-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2a18-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2a18-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2a18-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e2a18-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2a18-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2a18-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2a18-115">Not supported.</span></span>    |
|<span data-ttu-id="e2a18-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2a18-116">Application</span></span> | <span data-ttu-id="e2a18-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2a18-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2a18-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2a18-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="e2a18-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2a18-119">Request headers</span></span>
| <span data-ttu-id="e2a18-120">名前</span><span class="sxs-lookup"><span data-stu-id="e2a18-120">Name</span></span>       | <span data-ttu-id="e2a18-121">型</span><span class="sxs-lookup"><span data-stu-id="e2a18-121">Type</span></span> | <span data-ttu-id="e2a18-122">説明</span><span class="sxs-lookup"><span data-stu-id="e2a18-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2a18-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2a18-123">Authorization</span></span>  | <span data-ttu-id="e2a18-124">string</span><span class="sxs-lookup"><span data-stu-id="e2a18-124">string</span></span>  | <span data-ttu-id="e2a18-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e2a18-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2a18-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2a18-127">Request body</span></span>
<span data-ttu-id="e2a18-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e2a18-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e2a18-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e2a18-129">Parameter</span></span>    | <span data-ttu-id="e2a18-130">型</span><span class="sxs-lookup"><span data-stu-id="e2a18-130">Type</span></span>   |<span data-ttu-id="e2a18-131">説明</span><span class="sxs-lookup"><span data-stu-id="e2a18-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2a18-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e2a18-132">securityEnabledOnly</span></span>|<span data-ttu-id="e2a18-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2a18-133">Boolean</span></span>|<span data-ttu-id="e2a18-p105">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="e2a18-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="e2a18-136">応答</span><span class="sxs-lookup"><span data-stu-id="e2a18-136">Response</span></span>

<span data-ttu-id="e2a18-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e2a18-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2a18-138">例</span><span class="sxs-lookup"><span data-stu-id="e2a18-138">Example</span></span>
<span data-ttu-id="e2a18-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e2a18-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e2a18-140">要求</span><span class="sxs-lookup"><span data-stu-id="e2a18-140">Request</span></span>
<span data-ttu-id="e2a18-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2a18-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e2a18-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e2a18-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2a18-143">C#</span><span class="sxs-lookup"><span data-stu-id="e2a18-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2a18-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2a18-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2a18-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="e2a18-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e2a18-146">応答</span><span class="sxs-lookup"><span data-stu-id="e2a18-146">Response</span></span>
<span data-ttu-id="e2a18-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e2a18-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
