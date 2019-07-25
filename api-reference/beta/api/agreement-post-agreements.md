---
title: 契約を作成する
description: 新しいアグリーメントオブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: a9f0dd682ca09ea9723409193447c07f845e27da
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855467"
---
# <a name="create-agreement"></a><span data-ttu-id="eb1f0-103">契約を作成する</span><span class="sxs-lookup"><span data-stu-id="eb1f0-103">Create agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb1f0-104">新しい[アグリーメント](../resources/agreement.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-104">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb1f0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eb1f0-105">Permissions</span></span>
<span data-ttu-id="eb1f0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb1f0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb1f0-108">Permission type</span></span>                        | <span data-ttu-id="eb1f0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb1f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb1f0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb1f0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb1f0-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb1f0-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="eb1f0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb1f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb1f0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-113">Not supported.</span></span> |
|<span data-ttu-id="eb1f0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb1f0-114">Application</span></span>                            | <span data-ttu-id="eb1f0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb1f0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb1f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="eb1f0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb1f0-117">Request headers</span></span>
| <span data-ttu-id="eb1f0-118">名前</span><span class="sxs-lookup"><span data-stu-id="eb1f0-118">Name</span></span>         | <span data-ttu-id="eb1f0-119">型</span><span class="sxs-lookup"><span data-stu-id="eb1f0-119">Type</span></span>        | <span data-ttu-id="eb1f0-120">説明</span><span class="sxs-lookup"><span data-stu-id="eb1f0-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eb1f0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb1f0-121">Authorization</span></span> | <span data-ttu-id="eb1f0-122">string</span><span class="sxs-lookup"><span data-stu-id="eb1f0-122">string</span></span> | <span data-ttu-id="eb1f0-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb1f0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="eb1f0-125">Request body</span></span>
<span data-ttu-id="eb1f0-126">要求本文で、[アグリーメント](../resources/agreement.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-126">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="eb1f0-127">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-127">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="eb1f0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb1f0-128">Property</span></span>     | <span data-ttu-id="eb1f0-129">型</span><span class="sxs-lookup"><span data-stu-id="eb1f0-129">Type</span></span>        | <span data-ttu-id="eb1f0-130">説明</span><span class="sxs-lookup"><span data-stu-id="eb1f0-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb1f0-131">displayName</span><span class="sxs-lookup"><span data-stu-id="eb1f0-131">displayName</span></span>|<span data-ttu-id="eb1f0-132">String</span><span class="sxs-lookup"><span data-stu-id="eb1f0-132">String</span></span>|<span data-ttu-id="eb1f0-133">アグリーメントの表示名。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="eb1f0-134">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="eb1f0-134">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="eb1f0-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb1f0-135">Boolean</span></span>|<span data-ttu-id="eb1f0-136">ユーザーが同意する前に、契約を展開して表示する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-136">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="eb1f0-137">ファイル/ファイル名</span><span class="sxs-lookup"><span data-stu-id="eb1f0-137">files/fileName</span></span>|<span data-ttu-id="eb1f0-138">String</span><span class="sxs-lookup"><span data-stu-id="eb1f0-138">String</span></span>|<span data-ttu-id="eb1f0-139">アグリーメントファイルの名前 (たとえば、「お持ちの形式」)。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-139">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="eb1f0-140">ファイル/isDefault</span><span class="sxs-lookup"><span data-stu-id="eb1f0-140">files/isDefault</span></span>|<span data-ttu-id="eb1f0-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb1f0-141">Boolean</span></span>|<span data-ttu-id="eb1f0-142">クライアントの優先度に一致するカルチャがない場合に、これが既定のアグリーメントファイルであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-142">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="eb1f0-143">ファイルが既定として設定されていない場合は、最初のファイルが既定として扱われます。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-143">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="eb1f0-144">ファイル/言語</span><span class="sxs-lookup"><span data-stu-id="eb1f0-144">files/language</span></span>|<span data-ttu-id="eb1f0-145">String</span><span class="sxs-lookup"><span data-stu-id="eb1f0-145">String</span></span>|<span data-ttu-id="eb1f0-146">Languagecode2-country/regioncode2 という形式の、アグリーメントファイルのカルチャ。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-146">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="eb1f0-147">languagecode2 は、ISO 639-1 から派生した、小文字の2文字のコードです。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-147">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="eb1f0-148">country/regioncode2 は ISO 3166 から派生し、通常は2つの大文字または BCP-47 language タグ (例: en-us) で構成されます。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-148">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="eb1f0-149">ファイル/fileData/データ</span><span class="sxs-lookup"><span data-stu-id="eb1f0-149">files/fileData/data</span></span>|<span data-ttu-id="eb1f0-150">Binary</span><span class="sxs-lookup"><span data-stu-id="eb1f0-150">Binary</span></span>|<span data-ttu-id="eb1f0-151">PDF ドキュメントの使用条件を表すデータ。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-151">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="eb1f0-152">応答</span><span class="sxs-lookup"><span data-stu-id="eb1f0-152">Response</span></span>
<span data-ttu-id="eb1f0-153">成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[アグリーメント](../resources/agreement.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-153">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb1f0-154">例</span><span class="sxs-lookup"><span data-stu-id="eb1f0-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb1f0-155">要求</span><span class="sxs-lookup"><span data-stu-id="eb1f0-155">Request</span></span>
<span data-ttu-id="eb1f0-156">要求本文で、[アグリーメント](../resources/agreement.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-156">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eb1f0-157">プロトコル</span><span class="sxs-lookup"><span data-stu-id="eb1f0-157">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="eb1f0-158">C#</span><span class="sxs-lookup"><span data-stu-id="eb1f0-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb1f0-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb1f0-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eb1f0-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="eb1f0-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eb1f0-161">Java</span><span class="sxs-lookup"><span data-stu-id="eb1f0-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eb1f0-162">応答</span><span class="sxs-lookup"><span data-stu-id="eb1f0-162">Response</span></span>
><span data-ttu-id="eb1f0-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="eb1f0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
