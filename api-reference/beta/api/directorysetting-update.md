---
title: ディレクトリ設定を更新する
description: 特定のディレクトリ設定オブジェクトのプロパティを更新します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 35005bf047145a44d66777dbc947ef4fb7df5caa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417172"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="f1932-103">ディレクトリ設定を更新する</span><span class="sxs-lookup"><span data-stu-id="f1932-103">Update a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1932-104">特定のディレクトリ設定オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f1932-104">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="f1932-105">**注**: この API のベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="f1932-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="f1932-106">この API の/v1.0 バージョンが、 *groupSettings を更新*する名前に変更されました。</span><span class="sxs-lookup"><span data-stu-id="f1932-106">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1932-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1932-107">Permissions</span></span>
<span data-ttu-id="f1932-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1932-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1932-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1932-110">Permission type</span></span>      | <span data-ttu-id="f1932-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1932-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1932-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1932-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f1932-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1932-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f1932-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1932-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1932-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1932-115">Not supported.</span></span>    |
|<span data-ttu-id="f1932-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1932-116">Application</span></span> | <span data-ttu-id="f1932-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1932-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1932-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1932-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f1932-119">テナント全体またはグループ固有の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="f1932-119">Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f1932-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1932-120">Optional request headers</span></span>
| <span data-ttu-id="f1932-121">名前</span><span class="sxs-lookup"><span data-stu-id="f1932-121">Name</span></span>       | <span data-ttu-id="f1932-122">説明</span><span class="sxs-lookup"><span data-stu-id="f1932-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f1932-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1932-123">Authorization</span></span>  | <span data-ttu-id="f1932-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f1932-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1932-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1932-126">Request body</span></span>
<span data-ttu-id="f1932-127">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f1932-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="f1932-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1932-128">Property</span></span>     | <span data-ttu-id="f1932-129">型</span><span class="sxs-lookup"><span data-stu-id="f1932-129">Type</span></span>   |<span data-ttu-id="f1932-130">説明</span><span class="sxs-lookup"><span data-stu-id="f1932-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1932-131">values</span><span class="sxs-lookup"><span data-stu-id="f1932-131">values</span></span> | <span data-ttu-id="f1932-132">[Settingvalue](../resources/settingvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f1932-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="f1932-p104">更新された値のセットです。注:コレクション セット全体を指定する必要があります。単一の値のセットを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="f1932-p104">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="f1932-136">応答</span><span class="sxs-lookup"><span data-stu-id="f1932-136">Response</span></span>

<span data-ttu-id="f1932-137">成功した場合、このメソッドは `204 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f1932-137">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1932-138">例</span><span class="sxs-lookup"><span data-stu-id="f1932-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1932-139">要求</span><span class="sxs-lookup"><span data-stu-id="f1932-139">Request</span></span>
<span data-ttu-id="f1932-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1932-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f1932-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f1932-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f1932-142">C#</span><span class="sxs-lookup"><span data-stu-id="f1932-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1932-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1932-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f1932-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="f1932-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1932-145">応答</span><span class="sxs-lookup"><span data-stu-id="f1932-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```

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
  ]
}
-->
