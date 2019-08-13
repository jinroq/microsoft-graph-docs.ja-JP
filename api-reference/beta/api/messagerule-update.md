---
title: ルールを更新する
description: messageRule オブジェクトの書き込み可能なプロパティを変更し、変更を保存します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8983550dd1c9dd04eb11331805b63c9161f5186e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342776"
---
# <a name="update-rule"></a><span data-ttu-id="44500-103">ルールを更新する</span><span class="sxs-lookup"><span data-stu-id="44500-103">Update rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44500-104">[messageRule](../resources/messagerule.md) オブジェクトの書き込み可能なプロパティを変更し、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="44500-104">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="44500-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44500-105">Permissions</span></span>
<span data-ttu-id="44500-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44500-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44500-108">Permission type</span></span>      | <span data-ttu-id="44500-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44500-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44500-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44500-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44500-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44500-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="44500-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44500-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44500-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44500-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="44500-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44500-114">Application</span></span> | <span data-ttu-id="44500-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44500-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="44500-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44500-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="44500-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44500-117">Optional request headers</span></span>
| <span data-ttu-id="44500-118">名前</span><span class="sxs-lookup"><span data-stu-id="44500-118">Name</span></span>       | <span data-ttu-id="44500-119">説明</span><span class="sxs-lookup"><span data-stu-id="44500-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="44500-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="44500-120">Authorization</span></span>  | <span data-ttu-id="44500-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="44500-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="44500-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="44500-123">Request body</span></span>
<span data-ttu-id="44500-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="44500-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="44500-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44500-127">Property</span></span>     | <span data-ttu-id="44500-128">型</span><span class="sxs-lookup"><span data-stu-id="44500-128">Type</span></span>   |<span data-ttu-id="44500-129">説明</span><span class="sxs-lookup"><span data-stu-id="44500-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="44500-130">actions</span><span class="sxs-lookup"><span data-stu-id="44500-130">actions</span></span> | [<span data-ttu-id="44500-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="44500-131">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="44500-132">該当する条件が満たされた場合にメッセージに対して実行されるアクション。</span><span class="sxs-lookup"><span data-stu-id="44500-132">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="44500-133">conditions</span><span class="sxs-lookup"><span data-stu-id="44500-133">conditions</span></span> | [<span data-ttu-id="44500-134">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="44500-134">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="44500-135">該当するルール アクションをトリガーするために満たす必要のある条件。</span><span class="sxs-lookup"><span data-stu-id="44500-135">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="44500-136">displayName</span><span class="sxs-lookup"><span data-stu-id="44500-136">displayName</span></span> | <span data-ttu-id="44500-137">String</span><span class="sxs-lookup"><span data-stu-id="44500-137">String</span></span> | <span data-ttu-id="44500-138">ルールの表示名。</span><span class="sxs-lookup"><span data-stu-id="44500-138">The display name of the rule.</span></span> |
| <span data-ttu-id="44500-139">exceptions</span><span class="sxs-lookup"><span data-stu-id="44500-139">exceptions</span></span> | [<span data-ttu-id="44500-140">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="44500-140">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="44500-141">ルールの例外条件。</span><span class="sxs-lookup"><span data-stu-id="44500-141">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="44500-142">isEnabled</span><span class="sxs-lookup"><span data-stu-id="44500-142">isEnabled</span></span> | <span data-ttu-id="44500-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="44500-143">Boolean</span></span> | <span data-ttu-id="44500-144">メッセージに対するルールの適用が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="44500-144">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="44500-145">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="44500-145">isReadOnly</span></span> | <span data-ttu-id="44500-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="44500-146">Boolean</span></span> | <span data-ttu-id="44500-147">ルールが読み取り専用のため、ルールの REST API による変更や削除ができないことを示します。</span><span class="sxs-lookup"><span data-stu-id="44500-147">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="44500-148">sequence</span><span class="sxs-lookup"><span data-stu-id="44500-148">sequence</span></span> | <span data-ttu-id="44500-149">Int32</span><span class="sxs-lookup"><span data-stu-id="44500-149">Int32</span></span> | <span data-ttu-id="44500-150">他のルールもある中で、そのルールが実行される順序を示します。</span><span class="sxs-lookup"><span data-stu-id="44500-150">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="44500-151">応答</span><span class="sxs-lookup"><span data-stu-id="44500-151">Response</span></span>
<span data-ttu-id="44500-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に更新後の [messageRule](../resources/messagerule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="44500-152">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44500-153">例</span><span class="sxs-lookup"><span data-stu-id="44500-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44500-154">要求</span><span class="sxs-lookup"><span data-stu-id="44500-154">Request</span></span>
<span data-ttu-id="44500-155">次の例では、ルールの名前、「[ルールを取得する](messagerule-get.md)」の[例](messagerule-get.md#example)のルールに対して実行するアクションを転送元からアドレスを変更し、その重要度を高くマークします。</span><span class="sxs-lookup"><span data-stu-id="44500-155">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="44500-156">プロトコル</span><span class="sxs-lookup"><span data-stu-id="44500-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44500-157">C#</span><span class="sxs-lookup"><span data-stu-id="44500-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44500-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44500-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44500-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="44500-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="44500-160">Java</span><span class="sxs-lookup"><span data-stu-id="44500-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="44500-161">応答</span><span class="sxs-lookup"><span data-stu-id="44500-161">Response</span></span>
<span data-ttu-id="44500-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44500-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"Important from partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "markImportance": "high"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
