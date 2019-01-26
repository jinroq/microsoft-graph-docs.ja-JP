---
title: 'ユーザー: translateExchangeIds'
description: 形式との間、Outlook に関連するリソースの識別子を変換します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b09ae9bf6a1cbf1967a900770b07d8c9750ba21
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571290"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="52455-103">ユーザー: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="52455-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52455-104">形式との間、Outlook に関連するリソースの識別子を変換します。</span><span class="sxs-lookup"><span data-stu-id="52455-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="52455-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="52455-105">Permissions</span></span>

<span data-ttu-id="52455-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52455-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52455-108">Permission type</span></span> | <span data-ttu-id="52455-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52455-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="52455-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52455-110">Delegated (work or school account)</span></span> | <span data-ttu-id="52455-111">User.ReadBasic、User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52455-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="52455-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52455-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52455-113">User.ReadBasic、User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52455-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="52455-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52455-114">Application</span></span> | <span data-ttu-id="52455-115">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52455-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52455-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52455-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="52455-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52455-117">Request headers</span></span>

| <span data-ttu-id="52455-118">名前</span><span class="sxs-lookup"><span data-stu-id="52455-118">Name</span></span> | <span data-ttu-id="52455-119">値</span><span class="sxs-lookup"><span data-stu-id="52455-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="52455-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="52455-120">Authorization</span></span> | <span data-ttu-id="52455-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="52455-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52455-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="52455-123">Request body</span></span>

| <span data-ttu-id="52455-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="52455-124">Parameter</span></span> | <span data-ttu-id="52455-125">型</span><span class="sxs-lookup"><span data-stu-id="52455-125">Type</span></span> | <span data-ttu-id="52455-126">説明</span><span class="sxs-lookup"><span data-stu-id="52455-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="52455-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="52455-127">inputIds</span></span> | <span data-ttu-id="52455-128">Edm.String コレクション</span><span class="sxs-lookup"><span data-stu-id="52455-128">Edm.String collection</span></span> | <span data-ttu-id="52455-129">変換識別子のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="52455-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="52455-130">コレクション内のすべての識別子は、同じソース ID の種類を持つ必要があり、同じメールボックス内のアイテムにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="52455-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="52455-131">このコレクションの最大サイズは、1000 の文字列です。</span><span class="sxs-lookup"><span data-stu-id="52455-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="52455-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="52455-132">sourceIdType</span></span> | <span data-ttu-id="52455-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="52455-133">exchangeIdFormat</span></span> | <span data-ttu-id="52455-134">ID の種類の識別子の`InputIds`のパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="52455-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="52455-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="52455-135">targetIdType</span></span> | <span data-ttu-id="52455-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="52455-136">exchangeIdFormat</span></span> | <span data-ttu-id="52455-137">要求された ID の種類に変換します。</span><span class="sxs-lookup"><span data-stu-id="52455-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="52455-138">exchangeIdFormat 値</span><span class="sxs-lookup"><span data-stu-id="52455-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="52455-139">値</span><span class="sxs-lookup"><span data-stu-id="52455-139">Values</span></span> | <span data-ttu-id="52455-140">説明</span><span class="sxs-lookup"><span data-stu-id="52455-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="52455-141">エントリ Id</span><span class="sxs-lookup"><span data-stu-id="52455-141">entryId</span></span> | <span data-ttu-id="52455-142">MAPI クライアントによって使用されるバイナリのエントリ ID の形式です。</span><span class="sxs-lookup"><span data-stu-id="52455-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="52455-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="52455-143">ewsId</span></span> | <span data-ttu-id="52455-144">Exchange Web サービス クライアントによって使用される ID 形式です。</span><span class="sxs-lookup"><span data-stu-id="52455-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="52455-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="52455-145">immutableEntryId</span></span> | <span data-ttu-id="52455-146">バイナリ MAPI と互換性のある変更不可能な ID 形式です。</span><span class="sxs-lookup"><span data-stu-id="52455-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="52455-147">restId</span><span class="sxs-lookup"><span data-stu-id="52455-147">restId</span></span> | <span data-ttu-id="52455-148">Microsoft Graph で使用される既定の ID 形式です。</span><span class="sxs-lookup"><span data-stu-id="52455-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="52455-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="52455-149">restImmutableEntryId</span></span> | <span data-ttu-id="52455-150">Microsoft Graph で使用される ID の変更不可能な形式です。</span><span class="sxs-lookup"><span data-stu-id="52455-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="52455-151">バイナリ フォーマット (`entryId`と`immutableEntryId`) は、base64 でエンコードされた URL セーフであります。</span><span class="sxs-lookup"><span data-stu-id="52455-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="52455-152">URL safeness は、base64 エンコードのバイナリ データの次のように変更することによって実装されます。</span><span class="sxs-lookup"><span data-stu-id="52455-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="52455-153">交換`+`で`-`</span><span class="sxs-lookup"><span data-stu-id="52455-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="52455-154">交換`/`で`_`</span><span class="sxs-lookup"><span data-stu-id="52455-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="52455-155">末尾の埋め込み文字を削除する (`=`)</span><span class="sxs-lookup"><span data-stu-id="52455-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="52455-156">示す数のスペース文字は元の文字列の末尾に整数値を追加する (`0`、 `1`、または`2`)</span><span class="sxs-lookup"><span data-stu-id="52455-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="52455-157">応答</span><span class="sxs-lookup"><span data-stu-id="52455-157">Response</span></span>

<span data-ttu-id="52455-158">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[convertIdResult](../resources/convertidresult.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="52455-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52455-159">例</span><span class="sxs-lookup"><span data-stu-id="52455-159">Example</span></span>

<span data-ttu-id="52455-160">次の使用例は、REST API の通常の形式から、複数の識別子を変換する方法を示しています (`restId`) に残りの部分の変更不可能な形式 (`restImmutableEntryId`)。</span><span class="sxs-lookup"><span data-stu-id="52455-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="52455-161">要求</span><span class="sxs-lookup"><span data-stu-id="52455-161">Request</span></span>

<span data-ttu-id="52455-162">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52455-162">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="52455-163">応答</span><span class="sxs-lookup"><span data-stu-id="52455-163">Response</span></span>

<span data-ttu-id="52455-164">応答の例を次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="52455-164">Here is the example response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
