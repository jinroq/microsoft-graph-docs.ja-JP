---
title: 同期テンプレートの更新
description: 特定のアプリケーションに関連付けられている同期テンプレートを更新 (上書き) します。
localization_priority: Normal
ms.openlocfilehash: 155e8c15abd8cac9b017bdaa0276561272cbbf15
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458137"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="6a0cd-103">同期テンプレートの更新</span><span class="sxs-lookup"><span data-stu-id="6a0cd-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a0cd-104">特定のアプリケーションに関連付けられている同期テンプレートを更新 (上書き) します。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a0cd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a0cd-105">Permissions</span></span>
<span data-ttu-id="6a0cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a0cd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a0cd-108">Permission type</span></span>                        | <span data-ttu-id="6a0cd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a0cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a0cd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a0cd-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="6a0cd-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a0cd-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="6a0cd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a0cd-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="6a0cd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-113">Not supported.</span></span>|
|<span data-ttu-id="6a0cd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a0cd-114">Application</span></span>                            |<span data-ttu-id="6a0cd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="6a0cd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a0cd-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="6a0cd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a0cd-117">Request headers</span></span>

| <span data-ttu-id="6a0cd-118">名前</span><span class="sxs-lookup"><span data-stu-id="6a0cd-118">Name</span></span>           | <span data-ttu-id="6a0cd-119">型</span><span class="sxs-lookup"><span data-stu-id="6a0cd-119">Type</span></span>    | <span data-ttu-id="6a0cd-120">説明</span><span class="sxs-lookup"><span data-stu-id="6a0cd-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="6a0cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a0cd-121">Authorization</span></span>  | <span data-ttu-id="6a0cd-122">string</span><span class="sxs-lookup"><span data-stu-id="6a0cd-122">string</span></span>  | <span data-ttu-id="6a0cd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a0cd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a0cd-125">Request body</span></span>

<span data-ttu-id="6a0cd-126">要求本文で、既存のテンプレートを置き換える[同期テンプレート](../resources/synchronization-synchronizationtemplate.md)オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="6a0cd-127">すべてのプロパティが指定されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-127">Make sure all properties are provided.</span></span> <span data-ttu-id="6a0cd-128">不足しているプロパティは消去されます。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="6a0cd-129">応答</span><span class="sxs-lookup"><span data-stu-id="6a0cd-129">Response</span></span>

<span data-ttu-id="6a0cd-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="6a0cd-132">例</span><span class="sxs-lookup"><span data-stu-id="6a0cd-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="6a0cd-133">要求</span><span class="sxs-lookup"><span data-stu-id="6a0cd-133">Request</span></span>
<span data-ttu-id="6a0cd-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-134">The following is an example of a request.</span></span> 

><span data-ttu-id="6a0cd-135">**注:** ここに示す要求オブジェクトは読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="6a0cd-136">実際の呼び出しですべてのプロパティを含めます。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-136">Include all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a0cd-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6a0cd-137">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a0cd-138">C#</span><span class="sxs-lookup"><span data-stu-id="6a0cd-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a0cd-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a0cd-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a0cd-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="6a0cd-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6a0cd-141">応答</span><span class="sxs-lookup"><span data-stu-id="6a0cd-141">Response</span></span>
<span data-ttu-id="6a0cd-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a0cd-142">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
