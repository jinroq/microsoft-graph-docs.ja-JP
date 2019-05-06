---
title: inferenceClassificationOverride を作成する
description: 'SMTP アドレスによって識別される送信者の優先受信トレイの上書きを作成します。 その SMTP アドレスからの今後のメッセージは一貫して分類されます。 '
localization_priority: Normal
ms.openlocfilehash: 26524a50b56e49a7e28192124a94a52ad28ccd7c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592100"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="79b25-104">inferenceClassificationOverride を作成する</span><span class="sxs-lookup"><span data-stu-id="79b25-104">Create inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79b25-105">SMTP アドレスによって識別される送信者の[優先受信トレイ](../resources/manage-focused-inbox.md)の上書きを作成します。</span><span class="sxs-lookup"><span data-stu-id="79b25-105">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="79b25-106">この SMTP アドレスからの将来のメッセージは、オーバーライドで指定されたとおり一貫して分類されます。</span><span class="sxs-lookup"><span data-stu-id="79b25-106">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="79b25-107">**メモ**</span><span class="sxs-lookup"><span data-stu-id="79b25-107">**Note**</span></span>

- <span data-ttu-id="79b25-108">同じ STMP アドレスですでにオーバーライドがある場合は、そのオーバーライドの **ClassifyAs** および **Name** フィールドが指定の値で更新されます。</span><span class="sxs-lookup"><span data-stu-id="79b25-108">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="79b25-109">メールボックスでサポートされているオーバーライドは、一意の送信者 SMTP アドレスに基づき、最大 1000 件までです。</span><span class="sxs-lookup"><span data-stu-id="79b25-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="79b25-110">POST 操作では、同時に作成できるオーバーライドは 1 件です。</span><span class="sxs-lookup"><span data-stu-id="79b25-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="79b25-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79b25-111">Permissions</span></span>
<span data-ttu-id="79b25-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79b25-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79b25-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79b25-114">Permission type</span></span>      | <span data-ttu-id="79b25-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79b25-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79b25-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79b25-116">Delegated (work or school account)</span></span> | <span data-ttu-id="79b25-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b25-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="79b25-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79b25-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79b25-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b25-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="79b25-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79b25-120">Application</span></span> | <span data-ttu-id="79b25-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b25-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="79b25-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79b25-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="79b25-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79b25-123">Request headers</span></span>
| <span data-ttu-id="79b25-124">名前</span><span class="sxs-lookup"><span data-stu-id="79b25-124">Name</span></span>       | <span data-ttu-id="79b25-125">型</span><span class="sxs-lookup"><span data-stu-id="79b25-125">Type</span></span> | <span data-ttu-id="79b25-126">説明</span><span class="sxs-lookup"><span data-stu-id="79b25-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="79b25-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="79b25-127">Authorization</span></span>  | <span data-ttu-id="79b25-128">string</span><span class="sxs-lookup"><span data-stu-id="79b25-128">string</span></span>  | <span data-ttu-id="79b25-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="79b25-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79b25-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79b25-131">Content-Type</span></span> | <span data-ttu-id="79b25-132">string</span><span class="sxs-lookup"><span data-stu-id="79b25-132">string</span></span>  | <span data-ttu-id="79b25-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="79b25-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79b25-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="79b25-135">Request body</span></span>
<span data-ttu-id="79b25-136">要求の本文に、[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="79b25-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="79b25-137">応答</span><span class="sxs-lookup"><span data-stu-id="79b25-137">Response</span></span>

<span data-ttu-id="79b25-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79b25-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79b25-139">例</span><span class="sxs-lookup"><span data-stu-id="79b25-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79b25-140">要求</span><span class="sxs-lookup"><span data-stu-id="79b25-140">Request</span></span>
<span data-ttu-id="79b25-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79b25-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/beta/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```

##### <a name="response"></a><span data-ttu-id="79b25-142">応答</span><span class="sxs-lookup"><span data-stu-id="79b25-142">Response</span></span>
<span data-ttu-id="79b25-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79b25-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="79b25-146">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="79b25-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="79b25-147">Visual</span><span class="sxs-lookup"><span data-stu-id="79b25-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_inferenceclassificationoverride_from_inferenceclassification-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79b25-148">Java</span><span class="sxs-lookup"><span data-stu-id="79b25-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_inferenceclassificationoverride_from_inferenceclassification-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/inferenceclassification-post-overrides.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/inferenceclassification-post-overrides.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
