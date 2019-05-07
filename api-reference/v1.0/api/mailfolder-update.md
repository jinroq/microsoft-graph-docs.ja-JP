---
title: MailFolder を更新する
description: mailfolder オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: daa089d51af768e8ab07b6cedb0c88e0030ab435
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612584"
---
# <a name="update-mailfolder"></a><span data-ttu-id="1d36e-103">MailFolder を更新する</span><span class="sxs-lookup"><span data-stu-id="1d36e-103">Update mailfolder</span></span>

<span data-ttu-id="1d36e-104">mailfolder オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1d36e-104">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d36e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d36e-105">Permissions</span></span>
<span data-ttu-id="1d36e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d36e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d36e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d36e-108">Permission type</span></span>      | <span data-ttu-id="1d36e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d36e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d36e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d36e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d36e-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d36e-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1d36e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d36e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d36e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d36e-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1d36e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d36e-114">Application</span></span> | <span data-ttu-id="1d36e-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d36e-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d36e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d36e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1d36e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d36e-117">Request headers</span></span>
| <span data-ttu-id="1d36e-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d36e-118">Header</span></span>       | <span data-ttu-id="1d36e-119">値</span><span class="sxs-lookup"><span data-stu-id="1d36e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d36e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d36e-120">Authorization</span></span>  | <span data-ttu-id="1d36e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1d36e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1d36e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d36e-123">Content-Type</span></span>  | <span data-ttu-id="1d36e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1d36e-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d36e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d36e-126">Request body</span></span>
<span data-ttu-id="1d36e-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1d36e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1d36e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d36e-130">Property</span></span>     | <span data-ttu-id="1d36e-131">型</span><span class="sxs-lookup"><span data-stu-id="1d36e-131">Type</span></span>   |<span data-ttu-id="1d36e-132">説明</span><span class="sxs-lookup"><span data-stu-id="1d36e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d36e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1d36e-133">displayName</span></span>|<span data-ttu-id="1d36e-134">String</span><span class="sxs-lookup"><span data-stu-id="1d36e-134">String</span></span>|<span data-ttu-id="1d36e-135">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="1d36e-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="1d36e-136">応答</span><span class="sxs-lookup"><span data-stu-id="1d36e-136">Response</span></span>

<span data-ttu-id="1d36e-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1d36e-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d36e-138">例</span><span class="sxs-lookup"><span data-stu-id="1d36e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d36e-139">要求</span><span class="sxs-lookup"><span data-stu-id="1d36e-139">Request</span></span>
<span data-ttu-id="1d36e-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d36e-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
##### <a name="response"></a><span data-ttu-id="1d36e-141">応答</span><span class="sxs-lookup"><span data-stu-id="1d36e-141">Response</span></span>
<span data-ttu-id="1d36e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d36e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1d36e-145">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1d36e-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1d36e-146">Visual</span><span class="sxs-lookup"><span data-stu-id="1d36e-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d36e-147">Java</span><span class="sxs-lookup"><span data-stu-id="1d36e-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
