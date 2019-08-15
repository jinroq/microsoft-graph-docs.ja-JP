---
title: 'orgContact: getMemberGroups'
description: この API を呼び出すには、次のいずれかのアクセス許可が必要です。 アクセス許可の選択方法などの詳細については、「アクセス許可」を参照してください。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2a560d6274c6bc61a263988c981ac3ff311645b5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414302"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="56157-104">orgContact: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="56157-104">orgContact: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="56157-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="56157-105">Permissions</span></span>
<span data-ttu-id="56157-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56157-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56157-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56157-108">Permission type</span></span>      | <span data-ttu-id="56157-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="56157-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56157-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56157-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56157-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56157-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56157-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56157-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56157-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56157-113">Not supported.</span></span>    |
|<span data-ttu-id="56157-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56157-114">Application</span></span> | <span data-ttu-id="56157-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56157-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56157-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56157-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="56157-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56157-117">Request headers</span></span>
| <span data-ttu-id="56157-118">名前</span><span class="sxs-lookup"><span data-stu-id="56157-118">Name</span></span>       | <span data-ttu-id="56157-119">型</span><span class="sxs-lookup"><span data-stu-id="56157-119">Type</span></span> | <span data-ttu-id="56157-120">説明</span><span class="sxs-lookup"><span data-stu-id="56157-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="56157-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56157-121">Authorization</span></span>  | <span data-ttu-id="56157-122">string</span><span class="sxs-lookup"><span data-stu-id="56157-122">string</span></span>  | <span data-ttu-id="56157-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="56157-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56157-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="56157-125">Request body</span></span>
<span data-ttu-id="56157-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="56157-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56157-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="56157-127">Parameter</span></span>    | <span data-ttu-id="56157-128">型</span><span class="sxs-lookup"><span data-stu-id="56157-128">Type</span></span>   |<span data-ttu-id="56157-129">説明</span><span class="sxs-lookup"><span data-stu-id="56157-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56157-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="56157-130">securityEnabledOnly</span></span>|<span data-ttu-id="56157-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="56157-131">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="56157-132">応答</span><span class="sxs-lookup"><span data-stu-id="56157-132">Response</span></span>

<span data-ttu-id="56157-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="56157-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56157-134">例</span><span class="sxs-lookup"><span data-stu-id="56157-134">Example</span></span>
<span data-ttu-id="56157-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="56157-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="56157-136">要求</span><span class="sxs-lookup"><span data-stu-id="56157-136">Request</span></span>
<span data-ttu-id="56157-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56157-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="56157-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="56157-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="56157-139">C#</span><span class="sxs-lookup"><span data-stu-id="56157-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56157-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56157-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56157-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="56157-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="56157-142">応答</span><span class="sxs-lookup"><span data-stu-id="56157-142">Response</span></span>
<span data-ttu-id="56157-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56157-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
