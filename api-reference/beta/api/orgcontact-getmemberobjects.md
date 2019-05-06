---
title: 'orgContact: getMemberObjects'
description: この API を呼び出すには、次のいずれかのアクセス許可が必要です。 アクセス許可の選択方法などの詳細については、「アクセス許可」を参照してください。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5866793654095e54cba96147ab5489ab92eef3dd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596762"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="135a8-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="135a8-104">orgContact: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="135a8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="135a8-105">Permissions</span></span>
<span data-ttu-id="135a8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="135a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="135a8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="135a8-108">Permission type</span></span>      | <span data-ttu-id="135a8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="135a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="135a8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="135a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="135a8-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="135a8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="135a8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="135a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="135a8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="135a8-113">Not supported.</span></span>    |
|<span data-ttu-id="135a8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="135a8-114">Application</span></span> | <span data-ttu-id="135a8-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="135a8-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="135a8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="135a8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="135a8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="135a8-117">Request headers</span></span>
| <span data-ttu-id="135a8-118">名前</span><span class="sxs-lookup"><span data-stu-id="135a8-118">Name</span></span>       | <span data-ttu-id="135a8-119">型</span><span class="sxs-lookup"><span data-stu-id="135a8-119">Type</span></span> | <span data-ttu-id="135a8-120">説明</span><span class="sxs-lookup"><span data-stu-id="135a8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="135a8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="135a8-121">Authorization</span></span>  | <span data-ttu-id="135a8-122">string</span><span class="sxs-lookup"><span data-stu-id="135a8-122">string</span></span>  | <span data-ttu-id="135a8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="135a8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="135a8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="135a8-125">Request body</span></span>
<span data-ttu-id="135a8-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="135a8-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="135a8-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="135a8-127">Parameter</span></span>    | <span data-ttu-id="135a8-128">型</span><span class="sxs-lookup"><span data-stu-id="135a8-128">Type</span></span>   |<span data-ttu-id="135a8-129">説明</span><span class="sxs-lookup"><span data-stu-id="135a8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="135a8-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="135a8-130">securityEnabledOnly</span></span>|<span data-ttu-id="135a8-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="135a8-131">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="135a8-132">応答</span><span class="sxs-lookup"><span data-stu-id="135a8-132">Response</span></span>

<span data-ttu-id="135a8-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="135a8-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="135a8-134">例</span><span class="sxs-lookup"><span data-stu-id="135a8-134">Example</span></span>
<span data-ttu-id="135a8-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="135a8-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="135a8-136">要求</span><span class="sxs-lookup"><span data-stu-id="135a8-136">Request</span></span>
<span data-ttu-id="135a8-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="135a8-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="135a8-138">応答</span><span class="sxs-lookup"><span data-stu-id="135a8-138">Response</span></span>
<span data-ttu-id="135a8-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="135a8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="135a8-142">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="135a8-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="135a8-143">Visual</span><span class="sxs-lookup"><span data-stu-id="135a8-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/orgcontact_getmemberobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="135a8-144">Java</span><span class="sxs-lookup"><span data-stu-id="135a8-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/orgcontact_getmemberobjects-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
