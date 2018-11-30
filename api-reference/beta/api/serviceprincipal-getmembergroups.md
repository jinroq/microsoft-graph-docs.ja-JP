---
title: 'servicePrincipal: getMemberGroups'
description: このサービス主体のメンバーであるグループの一覧を取得します。  チェック、推移的です。
ms.openlocfilehash: 3ea35e86269f370a3f4fc500555ae04705c038fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066748"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="f4a90-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f4a90-104">servicePrincipal: getMemberGroups</span></span>

> <span data-ttu-id="f4a90-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f4a90-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4a90-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4a90-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f4a90-107">このサービス主体のメンバーであるグループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f4a90-107">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="f4a90-108">チェック、推移的です。</span><span class="sxs-lookup"><span data-stu-id="f4a90-108">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4a90-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4a90-109">Permissions</span></span>
<span data-ttu-id="f4a90-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4a90-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f4a90-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4a90-112">Permission type</span></span>      | <span data-ttu-id="f4a90-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4a90-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4a90-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4a90-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f4a90-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4a90-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f4a90-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4a90-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4a90-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4a90-117">Not supported.</span></span>    |
|<span data-ttu-id="f4a90-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4a90-118">Application</span></span> | <span data-ttu-id="f4a90-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a90-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4a90-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4a90-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="f4a90-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4a90-121">Request headers</span></span>
| <span data-ttu-id="f4a90-122">名前</span><span class="sxs-lookup"><span data-stu-id="f4a90-122">Name</span></span>       | <span data-ttu-id="f4a90-123">型</span><span class="sxs-lookup"><span data-stu-id="f4a90-123">Type</span></span> | <span data-ttu-id="f4a90-124">説明</span><span class="sxs-lookup"><span data-stu-id="f4a90-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4a90-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4a90-125">Authorization</span></span>  | <span data-ttu-id="f4a90-126">string</span><span class="sxs-lookup"><span data-stu-id="f4a90-126">string</span></span>  | <span data-ttu-id="f4a90-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f4a90-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4a90-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4a90-129">Request body</span></span>
<span data-ttu-id="f4a90-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f4a90-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4a90-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4a90-131">Parameter</span></span>    | <span data-ttu-id="f4a90-132">型</span><span class="sxs-lookup"><span data-stu-id="f4a90-132">Type</span></span>   |<span data-ttu-id="f4a90-133">説明</span><span class="sxs-lookup"><span data-stu-id="f4a90-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4a90-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="f4a90-134">securityEnabledOnly</span></span>|<span data-ttu-id="f4a90-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="f4a90-135">Boolean</span></span>|<span data-ttu-id="f4a90-p106">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="f4a90-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="f4a90-138">応答</span><span class="sxs-lookup"><span data-stu-id="f4a90-138">Response</span></span>

<span data-ttu-id="f4a90-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f4a90-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4a90-140">例</span><span class="sxs-lookup"><span data-stu-id="f4a90-140">Example</span></span>
<span data-ttu-id="f4a90-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f4a90-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f4a90-142">要求</span><span class="sxs-lookup"><span data-stu-id="f4a90-142">Request</span></span>
<span data-ttu-id="f4a90-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4a90-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f4a90-144">応答</span><span class="sxs-lookup"><span data-stu-id="f4a90-144">Response</span></span>
<span data-ttu-id="f4a90-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f4a90-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->