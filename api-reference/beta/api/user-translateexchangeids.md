---
title: 'ユーザー: translateExchangeIds'
description: Outlook 関連リソースの ID の形式を変換します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1015ae12f5ecfd63b29efe38f7172321b06386ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33961230"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="91d54-103">ユーザー: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="91d54-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91d54-104">Outlook 関連リソースの ID の形式を変換します。</span><span class="sxs-lookup"><span data-stu-id="91d54-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="91d54-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91d54-105">Permissions</span></span>

<span data-ttu-id="91d54-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91d54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91d54-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91d54-108">Permission type</span></span> | <span data-ttu-id="91d54-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="91d54-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="91d54-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91d54-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91d54-111">ユーザー. ReadBasic、user. 読み取り、ユーザー. 読み取り/書き込み。すべてのユーザー。すべてのユーザーに対して。</span><span class="sxs-lookup"><span data-stu-id="91d54-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="91d54-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91d54-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91d54-113">ユーザー. ReadBasic、User. 読み取り/書き込み</span><span class="sxs-lookup"><span data-stu-id="91d54-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="91d54-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91d54-114">Application</span></span> | <span data-ttu-id="91d54-115">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91d54-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91d54-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91d54-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="91d54-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91d54-117">Request headers</span></span>

| <span data-ttu-id="91d54-118">名前</span><span class="sxs-lookup"><span data-stu-id="91d54-118">Name</span></span> | <span data-ttu-id="91d54-119">値</span><span class="sxs-lookup"><span data-stu-id="91d54-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="91d54-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="91d54-120">Authorization</span></span> | <span data-ttu-id="91d54-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="91d54-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91d54-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="91d54-123">Request body</span></span>

| <span data-ttu-id="91d54-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="91d54-124">Parameter</span></span> | <span data-ttu-id="91d54-125">型</span><span class="sxs-lookup"><span data-stu-id="91d54-125">Type</span></span> | <span data-ttu-id="91d54-126">説明</span><span class="sxs-lookup"><span data-stu-id="91d54-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="91d54-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="91d54-127">inputIds</span></span> | <span data-ttu-id="91d54-128">String collection</span><span class="sxs-lookup"><span data-stu-id="91d54-128">String collection</span></span> | <span data-ttu-id="91d54-129">変換する識別子のコレクション。</span><span class="sxs-lookup"><span data-stu-id="91d54-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="91d54-130">コレクション内のすべての識別子のソース ID の種類は同じである必要があり、同じメールボックス内のアイテムである必要があります。</span><span class="sxs-lookup"><span data-stu-id="91d54-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="91d54-131">このコレクションの最大サイズは1000文字列です。</span><span class="sxs-lookup"><span data-stu-id="91d54-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="91d54-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="91d54-132">sourceIdType</span></span> | <span data-ttu-id="91d54-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="91d54-133">exchangeIdFormat</span></span> | <span data-ttu-id="91d54-134">`InputIds`パラメーターの識別子の id の種類。</span><span class="sxs-lookup"><span data-stu-id="91d54-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="91d54-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="91d54-135">targetIdType</span></span> | <span data-ttu-id="91d54-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="91d54-136">exchangeIdFormat</span></span> | <span data-ttu-id="91d54-137">変換先となる要求された ID の種類。</span><span class="sxs-lookup"><span data-stu-id="91d54-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="91d54-138">exchangeIdFormat の値</span><span class="sxs-lookup"><span data-stu-id="91d54-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="91d54-139">値</span><span class="sxs-lookup"><span data-stu-id="91d54-139">Values</span></span> | <span data-ttu-id="91d54-140">説明</span><span class="sxs-lookup"><span data-stu-id="91d54-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="91d54-141">entryId</span><span class="sxs-lookup"><span data-stu-id="91d54-141">entryId</span></span> | <span data-ttu-id="91d54-142">MAPI クライアントによって使用されるバイナリエントリ ID 形式。</span><span class="sxs-lookup"><span data-stu-id="91d54-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="91d54-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="91d54-143">ewsId</span></span> | <span data-ttu-id="91d54-144">Exchange Web サービスクライアントによって使用される ID 形式。</span><span class="sxs-lookup"><span data-stu-id="91d54-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="91d54-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="91d54-145">immutableEntryId</span></span> | <span data-ttu-id="91d54-146">バイナリ MAPI 互換の不変 ID 形式。</span><span class="sxs-lookup"><span data-stu-id="91d54-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="91d54-147">restId</span><span class="sxs-lookup"><span data-stu-id="91d54-147">restId</span></span> | <span data-ttu-id="91d54-148">Microsoft Graph で使用される既定の ID 形式。</span><span class="sxs-lookup"><span data-stu-id="91d54-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="91d54-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="91d54-149">restImmutableEntryId</span></span> | <span data-ttu-id="91d54-150">Microsoft Graph で使用される不変の ID 形式。</span><span class="sxs-lookup"><span data-stu-id="91d54-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="91d54-151">バイナリ形式 (`entryId`および`immutableEntryId`) は、URL セーフな base64 でエンコードされます。</span><span class="sxs-lookup"><span data-stu-id="91d54-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="91d54-152">URL-safeness は、バイナリデータの base64 エンコードを次のように変更することによって実装されます。</span><span class="sxs-lookup"><span data-stu-id="91d54-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="91d54-153">置換`+`後`-`</span><span class="sxs-lookup"><span data-stu-id="91d54-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="91d54-154">置換`/`後`_`</span><span class="sxs-lookup"><span data-stu-id="91d54-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="91d54-155">末尾のパディング文字を削除`=`する ()</span><span class="sxs-lookup"><span data-stu-id="91d54-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="91d54-156">文字列の末尾に、元の文字の数 (`0`、 `1`、、または`2`) を示す整数を追加します。</span><span class="sxs-lookup"><span data-stu-id="91d54-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="91d54-157">応答</span><span class="sxs-lookup"><span data-stu-id="91d54-157">Response</span></span>

<span data-ttu-id="91d54-158">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[convertIdResult](../resources/convertidresult.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="91d54-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91d54-159">例</span><span class="sxs-lookup"><span data-stu-id="91d54-159">Example</span></span>

<span data-ttu-id="91d54-160">次の例は、複数の識別子を標準の REST API 形式 (`restId`) から不変形式 (`restImmutableEntryId`) に変換する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="91d54-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="91d54-161">要求</span><span class="sxs-lookup"><span data-stu-id="91d54-161">Request</span></span>

<span data-ttu-id="91d54-162">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91d54-162">Here is the example request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds
Content-Type: application/json

{
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  "sourceIdType": "restId",
  "targetIdType": "restImmutableEntryId"
}
```

### <a name="response"></a><span data-ttu-id="91d54-163">応答</span><span class="sxs-lookup"><span data-stu-id="91d54-163">Response</span></span>

<span data-ttu-id="91d54-164">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="91d54-164">Here is the example response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/testexchangebeta/$metadata#Collection(microsoft.graph.convertIdResult)",
  "value": [
    {
      "sourceId": "{rest-formatted-id-1}",
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2}",
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="91d54-165">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="91d54-165">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91d54-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="91d54-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="91d54-167">C#</span><span class="sxs-lookup"><span data-stu-id="91d54-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
