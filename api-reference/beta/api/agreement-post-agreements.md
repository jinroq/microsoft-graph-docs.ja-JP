---
title: 契約書を作成します。
description: 契約の新しいオブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: 5040651e032a4f5d0ef2340646f11eb51bfff5eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514426"
---
# <a name="create-agreement"></a><span data-ttu-id="f104f-103">契約書を作成します。</span><span class="sxs-lookup"><span data-stu-id="f104f-103">Create agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f104f-104">[契約](../resources/agreement.md)の新しいオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f104f-104">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f104f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f104f-105">Permissions</span></span>
<span data-ttu-id="f104f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f104f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f104f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f104f-108">Permission type</span></span>                        | <span data-ttu-id="f104f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f104f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f104f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f104f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f104f-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f104f-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="f104f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f104f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f104f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f104f-113">Not supported.</span></span> |
|<span data-ttu-id="f104f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f104f-114">Application</span></span>                            | <span data-ttu-id="f104f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f104f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f104f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f104f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="f104f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f104f-117">Request headers</span></span>
| <span data-ttu-id="f104f-118">名前</span><span class="sxs-lookup"><span data-stu-id="f104f-118">Name</span></span>         | <span data-ttu-id="f104f-119">型</span><span class="sxs-lookup"><span data-stu-id="f104f-119">Type</span></span>        | <span data-ttu-id="f104f-120">説明</span><span class="sxs-lookup"><span data-stu-id="f104f-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f104f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f104f-121">Authorization</span></span> | <span data-ttu-id="f104f-122">string</span><span class="sxs-lookup"><span data-stu-id="f104f-122">string</span></span> | <span data-ttu-id="f104f-123">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="f104f-123">Bearer \{token\}.</span></span> <span data-ttu-id="f104f-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="f104f-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f104f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f104f-125">Request body</span></span>
<span data-ttu-id="f104f-126">要求の本文には、[許可書](../resources/agreement.md)オブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="f104f-126">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="f104f-127">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f104f-127">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="f104f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f104f-128">Property</span></span>     | <span data-ttu-id="f104f-129">型</span><span class="sxs-lookup"><span data-stu-id="f104f-129">Type</span></span>        | <span data-ttu-id="f104f-130">説明</span><span class="sxs-lookup"><span data-stu-id="f104f-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f104f-131">displayName</span><span class="sxs-lookup"><span data-stu-id="f104f-131">displayName</span></span>|<span data-ttu-id="f104f-132">String</span><span class="sxs-lookup"><span data-stu-id="f104f-132">String</span></span>|<span data-ttu-id="f104f-133">契約書の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="f104f-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="f104f-134">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="f104f-134">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="f104f-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="f104f-135">Boolean</span></span>|<span data-ttu-id="f104f-136">ユーザーを展開し、受け入れる前に契約書を表示するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f104f-136">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="f104f-137">ファイルまたはファイル名</span><span class="sxs-lookup"><span data-stu-id="f104f-137">files/fileName</span></span>|<span data-ttu-id="f104f-138">String</span><span class="sxs-lookup"><span data-stu-id="f104f-138">String</span></span>|<span data-ttu-id="f104f-139">契約ファイル (TOU.pdf など) の名前です。</span><span class="sxs-lookup"><span data-stu-id="f104f-139">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="f104f-140">ファイル/isDefault</span><span class="sxs-lookup"><span data-stu-id="f104f-140">files/isDefault</span></span>|<span data-ttu-id="f104f-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="f104f-141">Boolean</span></span>|<span data-ttu-id="f104f-142">クライアント基本設定と一致する、カルチャの場合、既定の契約書ファイルはかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f104f-142">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="f104f-143">ファイルの [なし] は、既定として設定された、1 つ目は既定値として扱われます。</span><span class="sxs-lookup"><span data-stu-id="f104f-143">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="f104f-144">ファイルと言語</span><span class="sxs-lookup"><span data-stu-id="f104f-144">files/language</span></span>|<span data-ttu-id="f104f-145">String</span><span class="sxs-lookup"><span data-stu-id="f104f-145">String</span></span>|<span data-ttu-id="f104f-146">形式 languagecode2 の国と regioncode2 の契約書ファイルのカルチャです。</span><span class="sxs-lookup"><span data-stu-id="f104f-146">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="f104f-147">languagecode2 は、小文字の ISO 639-1 から派生した 2 文字コードです。</span><span class="sxs-lookup"><span data-stu-id="f104f-147">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="f104f-148">国/regioncode2 では、ISO 3166 から派生し、通常は、2 つの大文字、または BCP 47 言語タグ (たとえば、EN-US)。</span><span class="sxs-lookup"><span data-stu-id="f104f-148">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="f104f-149">ファイル、構造体、データ fileData</span><span class="sxs-lookup"><span data-stu-id="f104f-149">files/fileData/data</span></span>|<span data-ttu-id="f104f-150">Binary</span><span class="sxs-lookup"><span data-stu-id="f104f-150">Binary</span></span>|<span data-ttu-id="f104f-151">PDF ドキュメントの使用条件を表すデータです。</span><span class="sxs-lookup"><span data-stu-id="f104f-151">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="f104f-152">応答</span><span class="sxs-lookup"><span data-stu-id="f104f-152">Response</span></span>
<span data-ttu-id="f104f-153">かどうかは成功すると、このメソッドが返されます、 `201, Created` 、応答の本体で応答コードおよび[契約](../resources/agreement.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f104f-153">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f104f-154">例</span><span class="sxs-lookup"><span data-stu-id="f104f-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f104f-155">要求</span><span class="sxs-lookup"><span data-stu-id="f104f-155">Request</span></span>
<span data-ttu-id="f104f-156">要求の本文には、[許可書](../resources/agreement.md)オブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="f104f-156">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="f104f-157">応答</span><span class="sxs-lookup"><span data-stu-id="f104f-157">Response</span></span>
><span data-ttu-id="f104f-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f104f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-post-agreements.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
