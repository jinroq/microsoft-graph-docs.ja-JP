---
title: inferenceClassificationOverride を作成する
description: 'SMTP アドレスで示される送信者のオーバーライドを作成します。 その SMTP アドレスからの今後のメッセージは一貫して分類されます。 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: bd9c86e3a283ec63c81eeac9bc19f3968d45d5d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014390"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="1e123-104">inferenceClassificationOverride を作成する</span><span class="sxs-lookup"><span data-stu-id="1e123-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="1e123-p102">SMTP アドレスで示される送信者のオーバーライドを作成します。この SMTP アドレスからの将来のメッセージは、オーバーライドで指定されたとおり一貫して分類されます。</span><span class="sxs-lookup"><span data-stu-id="1e123-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="1e123-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="1e123-107">**Note**</span></span>

- <span data-ttu-id="1e123-108">同じ SMTP アドレスを持つオーバーライドが既に存在する場合は\*\*\*\* 、そのオーバーライドの [フィールド名] フィールドと [**名前**] フィールドが、指定された値で更新されます。</span><span class="sxs-lookup"><span data-stu-id="1e123-108">If an override already exists with the same SMTP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="1e123-109">メールボックスでサポートされているオーバーライドは、一意の送信者 SMTP アドレスに基づき、最大 1000 件までです。</span><span class="sxs-lookup"><span data-stu-id="1e123-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="1e123-110">POST 操作では、同時に作成できるオーバーライドは 1 件です。</span><span class="sxs-lookup"><span data-stu-id="1e123-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e123-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e123-111">Permissions</span></span>
<span data-ttu-id="1e123-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e123-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e123-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e123-114">Permission type</span></span>      | <span data-ttu-id="1e123-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e123-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e123-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e123-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1e123-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e123-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1e123-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e123-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e123-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e123-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1e123-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e123-120">Application</span></span> | <span data-ttu-id="1e123-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e123-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e123-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e123-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="1e123-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e123-123">Request headers</span></span>
| <span data-ttu-id="1e123-124">名前</span><span class="sxs-lookup"><span data-stu-id="1e123-124">Name</span></span>       | <span data-ttu-id="1e123-125">型</span><span class="sxs-lookup"><span data-stu-id="1e123-125">Type</span></span> | <span data-ttu-id="1e123-126">説明</span><span class="sxs-lookup"><span data-stu-id="1e123-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e123-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e123-127">Authorization</span></span>  | <span data-ttu-id="1e123-128">string</span><span class="sxs-lookup"><span data-stu-id="1e123-128">string</span></span>  | <span data-ttu-id="1e123-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e123-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e123-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1e123-131">Content-Type</span></span> | <span data-ttu-id="1e123-132">string</span><span class="sxs-lookup"><span data-stu-id="1e123-132">string</span></span>  | <span data-ttu-id="1e123-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="1e123-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e123-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e123-135">Request body</span></span>
<span data-ttu-id="1e123-136">要求の本文に、[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e123-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1e123-137">応答</span><span class="sxs-lookup"><span data-stu-id="1e123-137">Response</span></span>

<span data-ttu-id="1e123-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1e123-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e123-139">例</span><span class="sxs-lookup"><span data-stu-id="1e123-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e123-140">要求</span><span class="sxs-lookup"><span data-stu-id="1e123-140">Request</span></span>
<span data-ttu-id="1e123-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e123-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1e123-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1e123-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e123-143">C#</span><span class="sxs-lookup"><span data-stu-id="1e123-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-inferenceclassificationoverride-from-inferenceclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e123-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e123-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-inferenceclassificationoverride-from-inferenceclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e123-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="1e123-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-inferenceclassificationoverride-from-inferenceclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1e123-146">Java</span><span class="sxs-lookup"><span data-stu-id="1e123-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-inferenceclassificationoverride-from-inferenceclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1e123-147">応答</span><span class="sxs-lookup"><span data-stu-id="1e123-147">Response</span></span>
<span data-ttu-id="1e123-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1e123-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
