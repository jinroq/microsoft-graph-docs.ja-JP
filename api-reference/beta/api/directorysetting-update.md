---
title: ディレクトリ設定を更新する
description: 特定のディレクトリ設定オブジェクトのプロパティを更新します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 65519a4bd4ae9e4640ec3d5b3abc604096bcd4b6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260537"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="aae4a-103">ディレクトリ設定を更新する</span><span class="sxs-lookup"><span data-stu-id="aae4a-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aae4a-104">特定のディレクトリ設定オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aae4a-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="aae4a-105">**注**: この API のベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="aae4a-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="aae4a-106">この API の/v1.0 バージョンが、 *groupSettings を更新*する名前に変更されました。</span><span class="sxs-lookup"><span data-stu-id="aae4a-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="aae4a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aae4a-107">Permissions</span></span>
<span data-ttu-id="aae4a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aae4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aae4a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aae4a-110">Permission type</span></span>      | <span data-ttu-id="aae4a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aae4a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aae4a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aae4a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aae4a-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aae4a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aae4a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aae4a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aae4a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aae4a-115">Not supported.</span></span>    |
|<span data-ttu-id="aae4a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aae4a-116">Application</span></span> | <span data-ttu-id="aae4a-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aae4a-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aae4a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aae4a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="aae4a-119">テナント全体またはグループ固有の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="aae4a-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="aae4a-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aae4a-120">Optional request headers</span></span>
| <span data-ttu-id="aae4a-121">名前</span><span class="sxs-lookup"><span data-stu-id="aae4a-121">Name</span></span>       | <span data-ttu-id="aae4a-122">説明</span><span class="sxs-lookup"><span data-stu-id="aae4a-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="aae4a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aae4a-123">Authorization</span></span>  | <span data-ttu-id="aae4a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aae4a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aae4a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="aae4a-126">Request body</span></span>
<span data-ttu-id="aae4a-127">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="aae4a-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="aae4a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aae4a-128">Property</span></span>     | <span data-ttu-id="aae4a-129">型</span><span class="sxs-lookup"><span data-stu-id="aae4a-129">Type</span></span>   |<span data-ttu-id="aae4a-130">説明</span><span class="sxs-lookup"><span data-stu-id="aae4a-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aae4a-131">values</span><span class="sxs-lookup"><span data-stu-id="aae4a-131">values</span></span> | <span data-ttu-id="aae4a-132">[Settingvalue](../resources/settingvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="aae4a-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="aae4a-p104">更新された値のセットです。注:コレクション セット全体を指定する必要があります。単一の値のセットを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="aae4a-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="aae4a-136">応答</span><span class="sxs-lookup"><span data-stu-id="aae4a-136">Response</span></span>

<span data-ttu-id="aae4a-137">成功した場合、このメソッドは `204 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="aae4a-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aae4a-138">例</span><span class="sxs-lookup"><span data-stu-id="aae4a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aae4a-139">要求</span><span class="sxs-lookup"><span data-stu-id="aae4a-139">Request</span></span>
<span data-ttu-id="aae4a-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aae4a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/settings/{id}
Content-type: application/json
Content-length: 178

{
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="aae4a-141">応答</span><span class="sxs-lookup"><span data-stu-id="aae4a-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aae4a-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="aae4a-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aae4a-143">C#</span><span class="sxs-lookup"><span data-stu-id="aae4a-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_directorysetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aae4a-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="aae4a-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_directorysetting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="aae4a-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="aae4a-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_directorysetting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
