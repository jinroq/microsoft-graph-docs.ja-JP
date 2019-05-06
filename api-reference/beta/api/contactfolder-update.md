---
title: Update contactfolder
description: contactfolder オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 508a8ac6791eda1b854d95c3e08d693f77cc92cb
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591333"
---
# <a name="update-contactfolder"></a><span data-ttu-id="9b0d7-103">Update contactfolder</span><span class="sxs-lookup"><span data-stu-id="9b0d7-103">Update contactfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b0d7-104">contactfolder オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9b0d7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9b0d7-105">Permissions</span></span>
<span data-ttu-id="9b0d7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b0d7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b0d7-108">Permission type</span></span>      | <span data-ttu-id="9b0d7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b0d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b0d7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b0d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b0d7-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b0d7-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9b0d7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b0d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b0d7-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b0d7-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9b0d7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b0d7-114">Application</span></span> | <span data-ttu-id="9b0d7-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b0d7-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b0d7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b0d7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9b0d7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b0d7-117">Request headers</span></span>
| <span data-ttu-id="9b0d7-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b0d7-118">Header</span></span>       | <span data-ttu-id="9b0d7-119">値</span><span class="sxs-lookup"><span data-stu-id="9b0d7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9b0d7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b0d7-120">Authorization</span></span>  | <span data-ttu-id="9b0d7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9b0d7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b0d7-123">Content-Type</span></span>  | <span data-ttu-id="9b0d7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9b0d7-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9b0d7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b0d7-126">Request body</span></span>
<span data-ttu-id="9b0d7-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9b0d7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b0d7-130">Property</span></span>     | <span data-ttu-id="9b0d7-131">型</span><span class="sxs-lookup"><span data-stu-id="9b0d7-131">Type</span></span>   |<span data-ttu-id="9b0d7-132">説明</span><span class="sxs-lookup"><span data-stu-id="9b0d7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b0d7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9b0d7-133">displayName</span></span>|<span data-ttu-id="9b0d7-134">文字列</span><span class="sxs-lookup"><span data-stu-id="9b0d7-134">String</span></span>|<span data-ttu-id="9b0d7-135">フォルダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-135">The folder's display name.</span></span>|
|<span data-ttu-id="9b0d7-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="9b0d7-136">parentFolderId</span></span>|<span data-ttu-id="9b0d7-137">String</span><span class="sxs-lookup"><span data-stu-id="9b0d7-137">String</span></span>|<span data-ttu-id="9b0d7-138">フォルダーの親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-138">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="9b0d7-139">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="9b0d7-139">wellKnownName</span></span>|<span data-ttu-id="9b0d7-140">string</span><span class="sxs-lookup"><span data-stu-id="9b0d7-140">string</span></span>|<span data-ttu-id="9b0d7-141">フォルダーが認識されているフォルダーである場合、フォルダーの名前。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-141">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="9b0d7-142">現在、認識されている連絡先フォルダーは `contacts` のみです。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-142">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="9b0d7-143">応答</span><span class="sxs-lookup"><span data-stu-id="9b0d7-143">Response</span></span>

<span data-ttu-id="9b0d7-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [contactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-144">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9b0d7-145">例</span><span class="sxs-lookup"><span data-stu-id="9b0d7-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b0d7-146">要求</span><span class="sxs-lookup"><span data-stu-id="9b0d7-146">Request</span></span>
<span data-ttu-id="9b0d7-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="9b0d7-148">応答</span><span class="sxs-lookup"><span data-stu-id="9b0d7-148">Response</span></span>
<span data-ttu-id="9b0d7-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9b0d7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "wellKnownName": "wellKnownName-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9b0d7-152">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="9b0d7-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9b0d7-153">Visual</span><span class="sxs-lookup"><span data-stu-id="9b0d7-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b0d7-154">Java</span><span class="sxs-lookup"><span data-stu-id="9b0d7-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_contactfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
