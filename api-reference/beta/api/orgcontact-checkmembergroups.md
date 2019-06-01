---
title: 'orgContact: checkMemberGroups'
description: この API を呼び出すには、次のいずれかのアクセス許可が必要です。 アクセス許可の選択方法などの詳細については、「アクセス許可」を参照してください。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 057d2a76d18db261b7ff1a4de238a3fe7006839a
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657281"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="e1280-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e1280-104">orgContact: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="e1280-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1280-105">Permissions</span></span>
<span data-ttu-id="e1280-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1280-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1280-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1280-108">Permission type</span></span>      | <span data-ttu-id="e1280-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1280-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1280-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1280-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1280-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1280-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e1280-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1280-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1280-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1280-113">Not supported.</span></span>    |
|<span data-ttu-id="e1280-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1280-114">Application</span></span> | <span data-ttu-id="e1280-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1280-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1280-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1280-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="e1280-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1280-117">Request headers</span></span>
| <span data-ttu-id="e1280-118">名前</span><span class="sxs-lookup"><span data-stu-id="e1280-118">Name</span></span>       | <span data-ttu-id="e1280-119">型</span><span class="sxs-lookup"><span data-stu-id="e1280-119">Type</span></span> | <span data-ttu-id="e1280-120">説明</span><span class="sxs-lookup"><span data-stu-id="e1280-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e1280-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1280-121">Authorization</span></span>  | <span data-ttu-id="e1280-122">string</span><span class="sxs-lookup"><span data-stu-id="e1280-122">string</span></span>  | <span data-ttu-id="e1280-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1280-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1280-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1280-125">Request body</span></span>
<span data-ttu-id="e1280-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e1280-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e1280-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e1280-127">Parameter</span></span>    | <span data-ttu-id="e1280-128">型</span><span class="sxs-lookup"><span data-stu-id="e1280-128">Type</span></span>   |<span data-ttu-id="e1280-129">説明</span><span class="sxs-lookup"><span data-stu-id="e1280-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1280-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="e1280-130">groupIds</span></span>|<span data-ttu-id="e1280-131">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="e1280-131">String collection</span></span> ||

## <a name="response"></a><span data-ttu-id="e1280-132">応答</span><span class="sxs-lookup"><span data-stu-id="e1280-132">Response</span></span>

<span data-ttu-id="e1280-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1280-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1280-134">例</span><span class="sxs-lookup"><span data-stu-id="e1280-134">Example</span></span>
<span data-ttu-id="e1280-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e1280-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e1280-136">要求</span><span class="sxs-lookup"><span data-stu-id="e1280-136">Request</span></span>
<span data-ttu-id="e1280-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1280-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="e1280-138">応答</span><span class="sxs-lookup"><span data-stu-id="e1280-138">Response</span></span>
<span data-ttu-id="e1280-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1280-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1280-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e1280-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1280-143">C#</span><span class="sxs-lookup"><span data-stu-id="e1280-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/orgcontact_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1280-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1280-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/orgcontact_checkmembergroups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
