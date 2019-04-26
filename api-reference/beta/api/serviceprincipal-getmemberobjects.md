---
title: 'serviceprincipal: getmemberobjects'
description: このサービスプリンシパルがメンバーになっているグループとディレクトリロールの一覧を取得します。  このチェックは推移的です。
localization_priority: Normal
ms.openlocfilehash: 6fd1a9b977eeed9eea56af19c2a7093795b45f15
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335847"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="3a929-104">serviceprincipal: getmemberobjects</span><span class="sxs-lookup"><span data-stu-id="3a929-104">servicePrincipal: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a929-105">このサービスプリンシパルがメンバーになっているグループとディレクトリロールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="3a929-105">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="3a929-106">このチェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="3a929-106">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a929-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3a929-107">Permissions</span></span>
<span data-ttu-id="3a929-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a929-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a929-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a929-110">Permission type</span></span>      | <span data-ttu-id="3a929-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a929-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a929-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a929-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a929-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a929-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3a929-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a929-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a929-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a929-115">Not supported.</span></span>    |
|<span data-ttu-id="3a929-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a929-116">Application</span></span> | <span data-ttu-id="3a929-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a929-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a929-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a929-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="3a929-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a929-119">Request headers</span></span>
| <span data-ttu-id="3a929-120">名前</span><span class="sxs-lookup"><span data-stu-id="3a929-120">Name</span></span>       | <span data-ttu-id="3a929-121">型</span><span class="sxs-lookup"><span data-stu-id="3a929-121">Type</span></span> | <span data-ttu-id="3a929-122">説明</span><span class="sxs-lookup"><span data-stu-id="3a929-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3a929-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a929-123">Authorization</span></span>  | <span data-ttu-id="3a929-124">string</span><span class="sxs-lookup"><span data-stu-id="3a929-124">string</span></span>  | <span data-ttu-id="3a929-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3a929-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a929-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a929-127">Request body</span></span>
<span data-ttu-id="3a929-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3a929-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a929-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a929-129">Parameter</span></span>    | <span data-ttu-id="3a929-130">型</span><span class="sxs-lookup"><span data-stu-id="3a929-130">Type</span></span>   |<span data-ttu-id="3a929-131">説明</span><span class="sxs-lookup"><span data-stu-id="3a929-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a929-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="3a929-132">securityEnabledOnly</span></span>|<span data-ttu-id="3a929-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a929-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="3a929-134">応答</span><span class="sxs-lookup"><span data-stu-id="3a929-134">Response</span></span>

<span data-ttu-id="3a929-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3a929-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a929-136">例</span><span class="sxs-lookup"><span data-stu-id="3a929-136">Example</span></span>
<span data-ttu-id="3a929-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3a929-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a929-138">要求</span><span class="sxs-lookup"><span data-stu-id="3a929-138">Request</span></span>
<span data-ttu-id="3a929-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a929-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3a929-140">応答</span><span class="sxs-lookup"><span data-stu-id="3a929-140">Response</span></span>
<span data-ttu-id="3a929-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3a929-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
