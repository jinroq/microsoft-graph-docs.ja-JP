---
title: 'orgContact: getMemberObjects'
description: この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「アクセス許可」を参照してください。
ms.openlocfilehash: d68bd0d4d1ace57fa91b5874bf376fa0a3c4fef4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072699"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="e74db-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="e74db-104">orgContact: getMemberObjects</span></span>

> <span data-ttu-id="e74db-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e74db-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e74db-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e74db-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="e74db-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e74db-107">Permissions</span></span>
<span data-ttu-id="e74db-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e74db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e74db-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e74db-110">Permission type</span></span>      | <span data-ttu-id="e74db-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e74db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e74db-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e74db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e74db-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e74db-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e74db-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e74db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e74db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e74db-115">Not supported.</span></span>    |
|<span data-ttu-id="e74db-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e74db-116">Application</span></span> | <span data-ttu-id="e74db-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e74db-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e74db-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e74db-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="e74db-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e74db-119">Request headers</span></span>
| <span data-ttu-id="e74db-120">名前</span><span class="sxs-lookup"><span data-stu-id="e74db-120">Name</span></span>       | <span data-ttu-id="e74db-121">型</span><span class="sxs-lookup"><span data-stu-id="e74db-121">Type</span></span> | <span data-ttu-id="e74db-122">説明</span><span class="sxs-lookup"><span data-stu-id="e74db-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e74db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e74db-123">Authorization</span></span>  | <span data-ttu-id="e74db-124">string</span><span class="sxs-lookup"><span data-stu-id="e74db-124">string</span></span>  | <span data-ttu-id="e74db-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e74db-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e74db-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e74db-127">Request body</span></span>
<span data-ttu-id="e74db-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e74db-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e74db-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e74db-129">Parameter</span></span>    | <span data-ttu-id="e74db-130">型</span><span class="sxs-lookup"><span data-stu-id="e74db-130">Type</span></span>   |<span data-ttu-id="e74db-131">説明</span><span class="sxs-lookup"><span data-stu-id="e74db-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e74db-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e74db-132">securityEnabledOnly</span></span>|<span data-ttu-id="e74db-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="e74db-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="e74db-134">応答</span><span class="sxs-lookup"><span data-stu-id="e74db-134">Response</span></span>

<span data-ttu-id="e74db-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e74db-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e74db-136">例</span><span class="sxs-lookup"><span data-stu-id="e74db-136">Example</span></span>
<span data-ttu-id="e74db-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e74db-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e74db-138">要求</span><span class="sxs-lookup"><span data-stu-id="e74db-138">Request</span></span>
<span data-ttu-id="e74db-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e74db-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="e74db-140">応答</span><span class="sxs-lookup"><span data-stu-id="e74db-140">Response</span></span>
<span data-ttu-id="e74db-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e74db-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->