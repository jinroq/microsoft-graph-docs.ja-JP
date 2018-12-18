---
title: ルールを更新する
description: messageRule オブジェクトの書き込み可能なプロパティを変更し、変更を保存します。
author: angelgolfer-ms
ms.openlocfilehash: 9ecef5c23502065d0d9e6fc32850b1ce89a1508c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321785"
---
# <a name="update-rule"></a><span data-ttu-id="a912c-103">ルールを更新する</span><span class="sxs-lookup"><span data-stu-id="a912c-103">Update rule</span></span>

> <span data-ttu-id="a912c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a912c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a912c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a912c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a912c-106">[messageRule](../resources/messagerule.md) オブジェクトの書き込み可能なプロパティを変更し、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="a912c-106">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="a912c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a912c-107">Permissions</span></span>
<span data-ttu-id="a912c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a912c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a912c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a912c-110">Permission type</span></span>      | <span data-ttu-id="a912c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a912c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a912c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a912c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a912c-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a912c-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a912c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a912c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a912c-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a912c-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a912c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a912c-116">Application</span></span> | <span data-ttu-id="a912c-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a912c-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a912c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a912c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a912c-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a912c-119">Optional request headers</span></span>
| <span data-ttu-id="a912c-120">名前</span><span class="sxs-lookup"><span data-stu-id="a912c-120">Name</span></span>       | <span data-ttu-id="a912c-121">説明</span><span class="sxs-lookup"><span data-stu-id="a912c-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a912c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a912c-122">Authorization</span></span>  | <span data-ttu-id="a912c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a912c-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a912c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a912c-125">Request body</span></span>
<span data-ttu-id="a912c-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a912c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a912c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a912c-129">Property</span></span>     | <span data-ttu-id="a912c-130">種類</span><span class="sxs-lookup"><span data-stu-id="a912c-130">Type</span></span>   |<span data-ttu-id="a912c-131">説明</span><span class="sxs-lookup"><span data-stu-id="a912c-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a912c-132">actions</span><span class="sxs-lookup"><span data-stu-id="a912c-132">actions</span></span> | [<span data-ttu-id="a912c-133">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="a912c-133">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="a912c-134">該当する条件が満たされた場合にメッセージに対して実行されるアクション。</span><span class="sxs-lookup"><span data-stu-id="a912c-134">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="a912c-135">conditions</span><span class="sxs-lookup"><span data-stu-id="a912c-135">conditions</span></span> | [<span data-ttu-id="a912c-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="a912c-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="a912c-137">該当するルール アクションをトリガーするために満たす必要のある条件。</span><span class="sxs-lookup"><span data-stu-id="a912c-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="a912c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a912c-138">displayName</span></span> | <span data-ttu-id="a912c-139">String</span><span class="sxs-lookup"><span data-stu-id="a912c-139">String</span></span> | <span data-ttu-id="a912c-140">ルールの表示名。</span><span class="sxs-lookup"><span data-stu-id="a912c-140">The display name of the rule.</span></span> |
| <span data-ttu-id="a912c-141">exceptions</span><span class="sxs-lookup"><span data-stu-id="a912c-141">exceptions</span></span> | [<span data-ttu-id="a912c-142">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="a912c-142">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="a912c-143">ルールの例外条件。</span><span class="sxs-lookup"><span data-stu-id="a912c-143">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="a912c-144">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a912c-144">isEnabled</span></span> | <span data-ttu-id="a912c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a912c-145">Boolean</span></span> | <span data-ttu-id="a912c-146">メッセージに対するルールの適用が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a912c-146">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="a912c-147">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="a912c-147">isReadOnly</span></span> | <span data-ttu-id="a912c-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="a912c-148">Boolean</span></span> | <span data-ttu-id="a912c-149">ルールが読み取り専用のため、ルールの REST API による変更や削除ができないことを示します。</span><span class="sxs-lookup"><span data-stu-id="a912c-149">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="a912c-150">sequence</span><span class="sxs-lookup"><span data-stu-id="a912c-150">sequence</span></span> | <span data-ttu-id="a912c-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a912c-151">Int32</span></span> | <span data-ttu-id="a912c-152">他のルールもある中で、そのルールが実行される順序を示します。</span><span class="sxs-lookup"><span data-stu-id="a912c-152">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="a912c-153">応答</span><span class="sxs-lookup"><span data-stu-id="a912c-153">Response</span></span>
<span data-ttu-id="a912c-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に更新後の [messageRule](../resources/messagerule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a912c-154">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a912c-155">例</span><span class="sxs-lookup"><span data-stu-id="a912c-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a912c-156">要求</span><span class="sxs-lookup"><span data-stu-id="a912c-156">Request</span></span>
<span data-ttu-id="a912c-157">次の例では、ルールの名前、「[ルールを取得する](messagerule-get.md)」の[例](messagerule-get.md#example)のルールに対して実行するアクションを転送元からアドレスを変更し、その重要度を高くマークします。</span><span class="sxs-lookup"><span data-stu-id="a912c-157">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 
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
##### <a name="response"></a><span data-ttu-id="a912c-158">応答</span><span class="sxs-lookup"><span data-stu-id="a912c-158">Response</span></span>
<span data-ttu-id="a912c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a912c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->