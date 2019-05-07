---
title: 同期テンプレートの更新
description: 特定のアプリケーションに関連付けられている同期テンプレートを更新 (上書き) します。
localization_priority: Normal
ms.openlocfilehash: 219a303b01198c3fb4ac4bb00e8a91564f8cf3b2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637928"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="e3cc9-103">同期テンプレートの更新</span><span class="sxs-lookup"><span data-stu-id="e3cc9-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3cc9-104">特定のアプリケーションに関連付けられている同期テンプレートを更新 (上書き) します。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3cc9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3cc9-105">Permissions</span></span>
<span data-ttu-id="e3cc9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3cc9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3cc9-108">Permission type</span></span>                        | <span data-ttu-id="e3cc9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3cc9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3cc9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3cc9-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="e3cc9-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3cc9-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e3cc9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3cc9-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e3cc9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-113">Not supported.</span></span>|
|<span data-ttu-id="e3cc9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3cc9-114">Application</span></span>                            |<span data-ttu-id="e3cc9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="e3cc9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3cc9-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="e3cc9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3cc9-117">Request headers</span></span>

| <span data-ttu-id="e3cc9-118">名前</span><span class="sxs-lookup"><span data-stu-id="e3cc9-118">Name</span></span>           | <span data-ttu-id="e3cc9-119">型</span><span class="sxs-lookup"><span data-stu-id="e3cc9-119">Type</span></span>    | <span data-ttu-id="e3cc9-120">説明</span><span class="sxs-lookup"><span data-stu-id="e3cc9-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e3cc9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3cc9-121">Authorization</span></span>  | <span data-ttu-id="e3cc9-122">string</span><span class="sxs-lookup"><span data-stu-id="e3cc9-122">string</span></span>  | <span data-ttu-id="e3cc9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3cc9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3cc9-125">Request body</span></span>

<span data-ttu-id="e3cc9-126">要求本文で、既存のテンプレートを置き換える[同期テンプレート](../resources/synchronization-synchronizationtemplate.md)オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="e3cc9-127">すべてのプロパティが指定されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-127">Make sure all properties are provided.</span></span> <span data-ttu-id="e3cc9-128">不足しているプロパティは消去されます。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="e3cc9-129">応答</span><span class="sxs-lookup"><span data-stu-id="e3cc9-129">Response</span></span>

<span data-ttu-id="e3cc9-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="e3cc9-132">例</span><span class="sxs-lookup"><span data-stu-id="e3cc9-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="e3cc9-133">要求</span><span class="sxs-lookup"><span data-stu-id="e3cc9-133">Request</span></span>
<span data-ttu-id="e3cc9-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-134">The following is an example of a request.</span></span> 

><span data-ttu-id="e3cc9-135">**注:** ここに示す要求オブジェクトは読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="e3cc9-136">実際の呼び出しですべてのプロパティを含めます。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-136">Include all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="e3cc9-137">応答</span><span class="sxs-lookup"><span data-stu-id="e3cc9-137">Response</span></span>
<span data-ttu-id="e3cc9-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3cc9-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e3cc9-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="e3cc9-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e3cc9-140">Visual</span><span class="sxs-lookup"><span data-stu-id="e3cc9-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_synchronizationtemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3cc9-141">Java</span><span class="sxs-lookup"><span data-stu-id="e3cc9-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_synchronizationtemplate-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
