---
title: 契約書を作成します。
description: 契約の新しいオブジェクトを作成します。
ms.openlocfilehash: bfcab53b4233d133309c99a4825e184a42670458
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067704"
---
# <a name="create-agreement"></a><span data-ttu-id="24a10-103">契約書を作成します。</span><span class="sxs-lookup"><span data-stu-id="24a10-103">Create agreement</span></span>

> <span data-ttu-id="24a10-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24a10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24a10-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24a10-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24a10-106">[契約](../resources/agreement.md)の新しいオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="24a10-106">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="24a10-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="24a10-107">Permissions</span></span>
<span data-ttu-id="24a10-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24a10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24a10-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24a10-110">Permission type</span></span>                        | <span data-ttu-id="24a10-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="24a10-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="24a10-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24a10-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="24a10-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24a10-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="24a10-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24a10-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24a10-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24a10-115">Not supported.</span></span> |
|<span data-ttu-id="24a10-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24a10-116">Application</span></span>                            | <span data-ttu-id="24a10-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24a10-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24a10-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24a10-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="24a10-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24a10-119">Request headers</span></span>
| <span data-ttu-id="24a10-120">名前</span><span class="sxs-lookup"><span data-stu-id="24a10-120">Name</span></span>         | <span data-ttu-id="24a10-121">型</span><span class="sxs-lookup"><span data-stu-id="24a10-121">Type</span></span>        | <span data-ttu-id="24a10-122">説明</span><span class="sxs-lookup"><span data-stu-id="24a10-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="24a10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24a10-123">Authorization</span></span> | <span data-ttu-id="24a10-124">string</span><span class="sxs-lookup"><span data-stu-id="24a10-124">string</span></span> | <span data-ttu-id="24a10-125">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="24a10-125">Bearer \{token\}.</span></span> <span data-ttu-id="24a10-126">必須。</span><span class="sxs-lookup"><span data-stu-id="24a10-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24a10-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="24a10-127">Request body</span></span>
<span data-ttu-id="24a10-128">要求の本文には、[許可書](../resources/agreement.md)オブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="24a10-128">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="24a10-129">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="24a10-129">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="24a10-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a10-130">Property</span></span>     | <span data-ttu-id="24a10-131">型</span><span class="sxs-lookup"><span data-stu-id="24a10-131">Type</span></span>        | <span data-ttu-id="24a10-132">説明</span><span class="sxs-lookup"><span data-stu-id="24a10-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="24a10-133">displayName</span><span class="sxs-lookup"><span data-stu-id="24a10-133">displayName</span></span>|<span data-ttu-id="24a10-134">String</span><span class="sxs-lookup"><span data-stu-id="24a10-134">String</span></span>|<span data-ttu-id="24a10-135">契約書の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="24a10-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="24a10-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="24a10-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="24a10-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="24a10-137">Boolean</span></span>|<span data-ttu-id="24a10-138">ユーザーを展開し、受け入れる前に契約書を表示するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24a10-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="24a10-139">ファイルまたはファイル名</span><span class="sxs-lookup"><span data-stu-id="24a10-139">files/fileName</span></span>|<span data-ttu-id="24a10-140">String</span><span class="sxs-lookup"><span data-stu-id="24a10-140">String</span></span>|<span data-ttu-id="24a10-141">契約ファイル (TOU.pdf など) の名前です。</span><span class="sxs-lookup"><span data-stu-id="24a10-141">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="24a10-142">ファイル/isDefault</span><span class="sxs-lookup"><span data-stu-id="24a10-142">files/isDefault</span></span>|<span data-ttu-id="24a10-143">ブール値</span><span class="sxs-lookup"><span data-stu-id="24a10-143">Boolean</span></span>|<span data-ttu-id="24a10-144">クライアント基本設定と一致する、カルチャの場合、既定の契約書ファイルはかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24a10-144">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="24a10-145">ファイルの [なし] は、既定として設定された、1 つ目は既定値として扱われます。</span><span class="sxs-lookup"><span data-stu-id="24a10-145">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="24a10-146">ファイルと言語</span><span class="sxs-lookup"><span data-stu-id="24a10-146">files/language</span></span>|<span data-ttu-id="24a10-147">String</span><span class="sxs-lookup"><span data-stu-id="24a10-147">String</span></span>|<span data-ttu-id="24a10-148">形式 languagecode2 の国と regioncode2 の契約書ファイルのカルチャです。</span><span class="sxs-lookup"><span data-stu-id="24a10-148">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="24a10-149">languagecode2 は、小文字の ISO 639-1 から派生した 2 文字コードです。</span><span class="sxs-lookup"><span data-stu-id="24a10-149">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="24a10-150">国/regioncode2 では、ISO 3166 から派生し、通常は、2 つの大文字、または BCP 47 言語タグ (たとえば、EN-US)。</span><span class="sxs-lookup"><span data-stu-id="24a10-150">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="24a10-151">ファイル、構造体、データ fileData</span><span class="sxs-lookup"><span data-stu-id="24a10-151">files/fileData/data</span></span>|<span data-ttu-id="24a10-152">バイナリ</span><span class="sxs-lookup"><span data-stu-id="24a10-152">Binary</span></span>|<span data-ttu-id="24a10-153">PDF ドキュメントの使用条件を表すデータです。</span><span class="sxs-lookup"><span data-stu-id="24a10-153">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="24a10-154">応答</span><span class="sxs-lookup"><span data-stu-id="24a10-154">Response</span></span>
<span data-ttu-id="24a10-155">かどうかは成功すると、このメソッドが返されます、 `201, Created` 、応答の本体で応答コードおよび[契約](../resources/agreement.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="24a10-155">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24a10-156">例</span><span class="sxs-lookup"><span data-stu-id="24a10-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24a10-157">要求</span><span class="sxs-lookup"><span data-stu-id="24a10-157">Request</span></span>
<span data-ttu-id="24a10-158">要求の本文には、[許可書](../resources/agreement.md)オブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="24a10-158">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/agreements
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "files": [
    {
      "fileName": "TOU.pdf",
      "language": "en",
      "isDefault": true,
      "fileData": {
        "data": "SGVsbG8gd29ybGQ="
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="24a10-159">応答</span><span class="sxs-lookup"><span data-stu-id="24a10-159">Response</span></span>
><span data-ttu-id="24a10-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="24a10-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
