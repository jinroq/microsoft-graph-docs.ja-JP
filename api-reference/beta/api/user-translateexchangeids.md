---
title: 'ユーザー: translateExchangeIds'
description: 形式との間、Outlook に関連するリソースの識別子を変換します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: b59cc33765586648432736df6067e6c089318729
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831907"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="a5b36-103">ユーザー: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="a5b36-103">user: translateExchangeIds</span></span>

> <span data-ttu-id="a5b36-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a5b36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5b36-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5b36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5b36-106">形式との間、Outlook に関連するリソースの識別子を変換します。</span><span class="sxs-lookup"><span data-stu-id="a5b36-106">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5b36-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a5b36-107">Permissions</span></span>

<span data-ttu-id="a5b36-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5b36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5b36-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5b36-110">Permission type</span></span> | <span data-ttu-id="a5b36-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5b36-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="a5b36-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5b36-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5b36-113">User.ReadBasic、User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5b36-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a5b36-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5b36-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5b36-115">User.ReadBasic、User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5b36-115">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="a5b36-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5b36-116">Application</span></span> | <span data-ttu-id="a5b36-117">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5b36-117">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5b36-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5b36-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="a5b36-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5b36-119">Request headers</span></span>

| <span data-ttu-id="a5b36-120">名前</span><span class="sxs-lookup"><span data-stu-id="a5b36-120">Name</span></span> | <span data-ttu-id="a5b36-121">値</span><span class="sxs-lookup"><span data-stu-id="a5b36-121">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="a5b36-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5b36-122">Authorization</span></span> | <span data-ttu-id="a5b36-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a5b36-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5b36-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5b36-125">Request body</span></span>

| <span data-ttu-id="a5b36-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="a5b36-126">Parameter</span></span> | <span data-ttu-id="a5b36-127">Type</span><span class="sxs-lookup"><span data-stu-id="a5b36-127">Type</span></span> | <span data-ttu-id="a5b36-128">説明</span><span class="sxs-lookup"><span data-stu-id="a5b36-128">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="a5b36-129">inputIds</span><span class="sxs-lookup"><span data-stu-id="a5b36-129">inputIds</span></span> | <span data-ttu-id="a5b36-130">Edm.String コレクション</span><span class="sxs-lookup"><span data-stu-id="a5b36-130">Edm.String collection</span></span> | <span data-ttu-id="a5b36-131">変換識別子のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a5b36-131">A collection of identifiers to convert.</span></span> <span data-ttu-id="a5b36-132">コレクション内のすべての識別子は、同じソース ID の種類を持つ必要があり、同じメールボックス内のアイテムにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5b36-132">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="a5b36-133">このコレクションの最大サイズは、1000 の文字列です。</span><span class="sxs-lookup"><span data-stu-id="a5b36-133">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="a5b36-134">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="a5b36-134">sourceIdType</span></span> | <span data-ttu-id="a5b36-135">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="a5b36-135">exchangeIdFormat</span></span> | <span data-ttu-id="a5b36-136">ID の種類の識別子の`InputIds`のパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="a5b36-136">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="a5b36-137">targetIdType</span><span class="sxs-lookup"><span data-stu-id="a5b36-137">targetIdType</span></span> | <span data-ttu-id="a5b36-138">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="a5b36-138">exchangeIdFormat</span></span> | <span data-ttu-id="a5b36-139">要求された ID の種類に変換します。</span><span class="sxs-lookup"><span data-stu-id="a5b36-139">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="a5b36-140">exchangeIdFormat 値</span><span class="sxs-lookup"><span data-stu-id="a5b36-140">exchangeIdFormat values</span></span>

| <span data-ttu-id="a5b36-141">値</span><span class="sxs-lookup"><span data-stu-id="a5b36-141">Values</span></span> | <span data-ttu-id="a5b36-142">説明</span><span class="sxs-lookup"><span data-stu-id="a5b36-142">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="a5b36-143">エントリ Id</span><span class="sxs-lookup"><span data-stu-id="a5b36-143">entryId</span></span> | <span data-ttu-id="a5b36-144">MAPI クライアントによって使用されるバイナリのエントリ ID の形式です。</span><span class="sxs-lookup"><span data-stu-id="a5b36-144">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="a5b36-145">ewsId</span><span class="sxs-lookup"><span data-stu-id="a5b36-145">ewsId</span></span> | <span data-ttu-id="a5b36-146">Exchange Web サービス クライアントによって使用される ID 形式です。</span><span class="sxs-lookup"><span data-stu-id="a5b36-146">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="a5b36-147">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="a5b36-147">immutableEntryId</span></span> | <span data-ttu-id="a5b36-148">バイナリ MAPI と互換性のある変更不可能な ID 形式です。</span><span class="sxs-lookup"><span data-stu-id="a5b36-148">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="a5b36-149">restId</span><span class="sxs-lookup"><span data-stu-id="a5b36-149">restId</span></span> | <span data-ttu-id="a5b36-150">Microsoft Graph で使用される既定の ID 形式です。</span><span class="sxs-lookup"><span data-stu-id="a5b36-150">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="a5b36-151">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="a5b36-151">restImmutableEntryId</span></span> | <span data-ttu-id="a5b36-152">Microsoft Graph で使用される ID の変更不可能な形式です。</span><span class="sxs-lookup"><span data-stu-id="a5b36-152">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="a5b36-153">バイナリ フォーマット (`entryId`と`immutableEntryId`) は、base64 でエンコードされた URL セーフであります。</span><span class="sxs-lookup"><span data-stu-id="a5b36-153">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="a5b36-154">URL safeness は、base64 エンコードのバイナリ データの次のように変更することによって実装されます。</span><span class="sxs-lookup"><span data-stu-id="a5b36-154">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="a5b36-155">交換`+`で`-`</span><span class="sxs-lookup"><span data-stu-id="a5b36-155">Replace `+` with `-`</span></span>
- <span data-ttu-id="a5b36-156">交換`/`で`_`</span><span class="sxs-lookup"><span data-stu-id="a5b36-156">Replace `/` with `_`</span></span>
- <span data-ttu-id="a5b36-157">末尾の埋め込み文字を削除する (`=`)</span><span class="sxs-lookup"><span data-stu-id="a5b36-157">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="a5b36-158">示す数のスペース文字は元の文字列の末尾に整数値を追加する (`0`、 `1`、または`2`)</span><span class="sxs-lookup"><span data-stu-id="a5b36-158">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="a5b36-159">応答</span><span class="sxs-lookup"><span data-stu-id="a5b36-159">Response</span></span>

<span data-ttu-id="a5b36-160">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[convertIdResult](../resources/convertidresult.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a5b36-160">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5b36-161">例</span><span class="sxs-lookup"><span data-stu-id="a5b36-161">Example</span></span>

<span data-ttu-id="a5b36-162">次の使用例は、REST API の通常の形式から、複数の識別子を変換する方法を示しています (`restId`) に残りの部分の変更不可能な形式 (`restImmutableEntryId`)。</span><span class="sxs-lookup"><span data-stu-id="a5b36-162">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="a5b36-163">要求</span><span class="sxs-lookup"><span data-stu-id="a5b36-163">Request</span></span>

<span data-ttu-id="a5b36-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a5b36-164">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5b36-165">応答</span><span class="sxs-lookup"><span data-stu-id="a5b36-165">Response</span></span>

<span data-ttu-id="a5b36-166">応答の例を次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="a5b36-166">Here is the example response</span></span>
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
      "sourceId": "{rest-formatted-id-1},
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2},
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
