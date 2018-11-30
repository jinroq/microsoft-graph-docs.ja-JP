---
title: 'servicePrincipal: checkMemberGroups'
description: この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「アクセス許可」を参照してください。
ms.openlocfilehash: bf16206e9029ddcf687738c3a7db5a0a27a43903
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066233"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="1d72b-104">servicePrincipal: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="1d72b-104">servicePrincipal: checkMemberGroups</span></span>

> <span data-ttu-id="1d72b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d72b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d72b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d72b-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d72b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d72b-107">Permissions</span></span>
<span data-ttu-id="1d72b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d72b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d72b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d72b-110">Permission type</span></span>      | <span data-ttu-id="1d72b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d72b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d72b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d72b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d72b-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d72b-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d72b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d72b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d72b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d72b-115">Not supported.</span></span>    |
|<span data-ttu-id="1d72b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d72b-116">Application</span></span> | <span data-ttu-id="1d72b-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d72b-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d72b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d72b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="1d72b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d72b-119">Request headers</span></span>
| <span data-ttu-id="1d72b-120">名前</span><span class="sxs-lookup"><span data-stu-id="1d72b-120">Name</span></span>       | <span data-ttu-id="1d72b-121">型</span><span class="sxs-lookup"><span data-stu-id="1d72b-121">Type</span></span> | <span data-ttu-id="1d72b-122">説明</span><span class="sxs-lookup"><span data-stu-id="1d72b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d72b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d72b-123">Authorization</span></span>  | <span data-ttu-id="1d72b-124">string</span><span class="sxs-lookup"><span data-stu-id="1d72b-124">string</span></span>  | <span data-ttu-id="1d72b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1d72b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d72b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d72b-127">Request body</span></span>
<span data-ttu-id="1d72b-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1d72b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1d72b-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1d72b-129">Parameter</span></span>    | <span data-ttu-id="1d72b-130">型</span><span class="sxs-lookup"><span data-stu-id="1d72b-130">Type</span></span>   |<span data-ttu-id="1d72b-131">説明</span><span class="sxs-lookup"><span data-stu-id="1d72b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d72b-132">groupIds</span><span class="sxs-lookup"><span data-stu-id="1d72b-132">groupIds</span></span>|<span data-ttu-id="1d72b-133">String</span><span class="sxs-lookup"><span data-stu-id="1d72b-133">String</span></span>||

## <a name="response"></a><span data-ttu-id="1d72b-134">応答</span><span class="sxs-lookup"><span data-stu-id="1d72b-134">Response</span></span>

<span data-ttu-id="1d72b-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1d72b-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d72b-136">例</span><span class="sxs-lookup"><span data-stu-id="1d72b-136">Example</span></span>
<span data-ttu-id="1d72b-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1d72b-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1d72b-138">要求</span><span class="sxs-lookup"><span data-stu-id="1d72b-138">Request</span></span>
<span data-ttu-id="1d72b-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d72b-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="1d72b-140">応答</span><span class="sxs-lookup"><span data-stu-id="1d72b-140">Response</span></span>
<span data-ttu-id="1d72b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d72b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->