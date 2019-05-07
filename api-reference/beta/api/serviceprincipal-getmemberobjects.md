---
title: 'servicePrincipal: getMemberObjects'
description: このサービスプリンシパルがメンバーになっているグループとディレクトリロールの一覧を取得します。  このチェックは推移的です。
localization_priority: Normal
ms.openlocfilehash: 00f49c3b33133dcabeaf08bab1740fe50ea6b662
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638712"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="80e7b-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="80e7b-104">servicePrincipal: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80e7b-105">このサービスプリンシパルがメンバーになっているグループとディレクトリロールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="80e7b-105">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="80e7b-106">このチェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="80e7b-106">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="80e7b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="80e7b-107">Permissions</span></span>
<span data-ttu-id="80e7b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80e7b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80e7b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80e7b-110">Permission type</span></span>      | <span data-ttu-id="80e7b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="80e7b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80e7b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80e7b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="80e7b-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="80e7b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80e7b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80e7b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80e7b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80e7b-115">Not supported.</span></span>    |
|<span data-ttu-id="80e7b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80e7b-116">Application</span></span> | <span data-ttu-id="80e7b-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80e7b-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80e7b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80e7b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="80e7b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80e7b-119">Request headers</span></span>
| <span data-ttu-id="80e7b-120">名前</span><span class="sxs-lookup"><span data-stu-id="80e7b-120">Name</span></span>       | <span data-ttu-id="80e7b-121">型</span><span class="sxs-lookup"><span data-stu-id="80e7b-121">Type</span></span> | <span data-ttu-id="80e7b-122">説明</span><span class="sxs-lookup"><span data-stu-id="80e7b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80e7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80e7b-123">Authorization</span></span>  | <span data-ttu-id="80e7b-124">string</span><span class="sxs-lookup"><span data-stu-id="80e7b-124">string</span></span>  | <span data-ttu-id="80e7b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="80e7b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80e7b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="80e7b-127">Request body</span></span>
<span data-ttu-id="80e7b-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="80e7b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="80e7b-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="80e7b-129">Parameter</span></span>    | <span data-ttu-id="80e7b-130">型</span><span class="sxs-lookup"><span data-stu-id="80e7b-130">Type</span></span>   |<span data-ttu-id="80e7b-131">説明</span><span class="sxs-lookup"><span data-stu-id="80e7b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80e7b-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="80e7b-132">securityEnabledOnly</span></span>|<span data-ttu-id="80e7b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="80e7b-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="80e7b-134">応答</span><span class="sxs-lookup"><span data-stu-id="80e7b-134">Response</span></span>

<span data-ttu-id="80e7b-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="80e7b-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80e7b-136">例</span><span class="sxs-lookup"><span data-stu-id="80e7b-136">Example</span></span>
<span data-ttu-id="80e7b-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="80e7b-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80e7b-138">要求</span><span class="sxs-lookup"><span data-stu-id="80e7b-138">Request</span></span>
<span data-ttu-id="80e7b-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80e7b-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="80e7b-140">応答</span><span class="sxs-lookup"><span data-stu-id="80e7b-140">Response</span></span>
<span data-ttu-id="80e7b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80e7b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="80e7b-144">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="80e7b-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="80e7b-145">Visual</span><span class="sxs-lookup"><span data-stu-id="80e7b-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/serviceprincipal_getmemberobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80e7b-146">Java</span><span class="sxs-lookup"><span data-stu-id="80e7b-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/serviceprincipal_getmemberobjects-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/serviceprincipal-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
