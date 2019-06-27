---
title: 'セクション: copyToSectionGroup'
description: 指定したセクショングループにセクションをコピーします。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 34455921995768ba9d2faffac3319cb1d58b5d64
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279304"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="3a6e2-103">セクション: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="3a6e2-103">section: copyToSectionGroup</span></span>
<span data-ttu-id="3a6e2-104">指定したセクショングループにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="3a6e2-105">コピー操作では、非同期呼び出しパターンに従います。最初に Copy アクションを呼び出してから、結果の操作エンドポイントをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a6e2-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3a6e2-106">Permissions</span></span>
<span data-ttu-id="3a6e2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a6e2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a6e2-109">Permission type</span></span>      | <span data-ttu-id="3a6e2-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a6e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a6e2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a6e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3a6e2-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a6e2-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a6e2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a6e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a6e2-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a6e2-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3a6e2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a6e2-115">Application</span></span> | <span data-ttu-id="3a6e2-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a6e2-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a6e2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a6e2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="3a6e2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a6e2-118">Request headers</span></span>
| <span data-ttu-id="3a6e2-119">名前</span><span class="sxs-lookup"><span data-stu-id="3a6e2-119">Name</span></span>       | <span data-ttu-id="3a6e2-120">型</span><span class="sxs-lookup"><span data-stu-id="3a6e2-120">Type</span></span> | <span data-ttu-id="3a6e2-121">説明</span><span class="sxs-lookup"><span data-stu-id="3a6e2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3a6e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a6e2-122">Authorization</span></span>  | <span data-ttu-id="3a6e2-123">string</span><span class="sxs-lookup"><span data-stu-id="3a6e2-123">string</span></span>  | <span data-ttu-id="3a6e2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a6e2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a6e2-126">Content-Type</span></span> | <span data-ttu-id="3a6e2-127">string</span><span class="sxs-lookup"><span data-stu-id="3a6e2-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3a6e2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a6e2-128">Request body</span></span>
<span data-ttu-id="3a6e2-129">要求本文で、操作に必要なパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="3a6e2-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a6e2-130">Parameter</span></span>    | <span data-ttu-id="3a6e2-131">型</span><span class="sxs-lookup"><span data-stu-id="3a6e2-131">Type</span></span>   |<span data-ttu-id="3a6e2-132">説明</span><span class="sxs-lookup"><span data-stu-id="3a6e2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a6e2-133">groupId</span><span class="sxs-lookup"><span data-stu-id="3a6e2-133">groupId</span></span>|<span data-ttu-id="3a6e2-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3a6e2-134">String</span></span>|<span data-ttu-id="3a6e2-135">コピー先のグループの id。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-135">The id of the group to copy to.</span></span> <span data-ttu-id="3a6e2-136">Office 365 グループにコピーする場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-136">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="3a6e2-137">id</span><span class="sxs-lookup"><span data-stu-id="3a6e2-137">id</span></span>|<span data-ttu-id="3a6e2-138">String</span><span class="sxs-lookup"><span data-stu-id="3a6e2-138">String</span></span>|<span data-ttu-id="3a6e2-139">必須。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-139">Required.</span></span> <span data-ttu-id="3a6e2-140">コピー先のセクショングループの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-140">The id of the destination section group.</span></span> |
|<span data-ttu-id="3a6e2-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="3a6e2-141">renameAs</span></span>|<span data-ttu-id="3a6e2-142">String</span><span class="sxs-lookup"><span data-stu-id="3a6e2-142">String</span></span>|<span data-ttu-id="3a6e2-143">コピーするフィルターの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-143">The name of the copy.</span></span> <span data-ttu-id="3a6e2-144">Defaults to the name of the existing item.</span><span class="sxs-lookup"><span data-stu-id="3a6e2-144">Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="3a6e2-145">応答</span><span class="sxs-lookup"><span data-stu-id="3a6e2-145">Response</span></span>

<span data-ttu-id="3a6e2-146">成功した場合、このメソッド`202 Accepted`は応答コードと`Operation-Location`ヘッダーを返します。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-146">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="3a6e2-147">操作の場所のエンドポイントをポーリングして、[コピー操作の状態を取得](onenoteoperation-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-147">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="3a6e2-148">例</span><span class="sxs-lookup"><span data-stu-id="3a6e2-148">Example</span></span>
<span data-ttu-id="3a6e2-149">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a6e2-150">要求</span><span class="sxs-lookup"><span data-stu-id="3a6e2-150">Request</span></span>
<span data-ttu-id="3a6e2-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="3a6e2-152">応答</span><span class="sxs-lookup"><span data-stu-id="3a6e2-152">Response</span></span>
<span data-ttu-id="3a6e2-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3a6e2-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3a6e2-154">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="3a6e2-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3a6e2-155">C#</span><span class="sxs-lookup"><span data-stu-id="3a6e2-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a6e2-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="3a6e2-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3a6e2-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="3a6e2-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/section_copytosectiongroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/section-copytosectiongroup.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
