---
title: 'servicePrincipal: getMemberObjects'
description: このサービス主体のメンバーであるグループおよびディレクトリの役割の一覧を取得します。  このチェックは、推移的です。
ms.openlocfilehash: 82fd1791b32c54a4670977e7ca5a66bdd92c1c14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071242"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="d4633-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="d4633-104">servicePrincipal: getMemberObjects</span></span>

> <span data-ttu-id="d4633-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d4633-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4633-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4633-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4633-107">このサービス主体のメンバーであるグループおよびディレクトリの役割の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d4633-107">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="d4633-108">このチェックは、推移的です。</span><span class="sxs-lookup"><span data-stu-id="d4633-108">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4633-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d4633-109">Permissions</span></span>
<span data-ttu-id="d4633-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4633-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4633-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4633-112">Permission type</span></span>      | <span data-ttu-id="d4633-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4633-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4633-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4633-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d4633-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4633-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4633-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4633-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4633-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4633-117">Not supported.</span></span>    |
|<span data-ttu-id="d4633-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4633-118">Application</span></span> | <span data-ttu-id="d4633-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4633-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4633-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4633-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="d4633-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4633-121">Request headers</span></span>
| <span data-ttu-id="d4633-122">名前</span><span class="sxs-lookup"><span data-stu-id="d4633-122">Name</span></span>       | <span data-ttu-id="d4633-123">型</span><span class="sxs-lookup"><span data-stu-id="d4633-123">Type</span></span> | <span data-ttu-id="d4633-124">説明</span><span class="sxs-lookup"><span data-stu-id="d4633-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d4633-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4633-125">Authorization</span></span>  | <span data-ttu-id="d4633-126">string</span><span class="sxs-lookup"><span data-stu-id="d4633-126">string</span></span>  | <span data-ttu-id="d4633-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d4633-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4633-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4633-129">Request body</span></span>
<span data-ttu-id="d4633-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d4633-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d4633-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d4633-131">Parameter</span></span>    | <span data-ttu-id="d4633-132">型</span><span class="sxs-lookup"><span data-stu-id="d4633-132">Type</span></span>   |<span data-ttu-id="d4633-133">説明</span><span class="sxs-lookup"><span data-stu-id="d4633-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4633-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d4633-134">securityEnabledOnly</span></span>|<span data-ttu-id="d4633-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="d4633-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="d4633-136">応答</span><span class="sxs-lookup"><span data-stu-id="d4633-136">Response</span></span>

<span data-ttu-id="d4633-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d4633-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4633-138">例</span><span class="sxs-lookup"><span data-stu-id="d4633-138">Example</span></span>
<span data-ttu-id="d4633-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d4633-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d4633-140">要求</span><span class="sxs-lookup"><span data-stu-id="d4633-140">Request</span></span>
<span data-ttu-id="d4633-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4633-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d4633-142">応答</span><span class="sxs-lookup"><span data-stu-id="d4633-142">Response</span></span>
<span data-ttu-id="d4633-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4633-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->