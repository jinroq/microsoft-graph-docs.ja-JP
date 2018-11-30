---
title: messageRule リソースの種類
description: ユーザーの受信トレイ内のメッセージに適用されるルールです。
ms.openlocfilehash: 3189ca11f00d5f298e4de29531f20e9da52c8c6e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073553"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="6808c-103">messageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6808c-103">messageRule resource type</span></span>

> <span data-ttu-id="6808c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6808c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6808c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6808c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6808c-106">ユーザーの受信トレイ内のメッセージに適用されるルールです。</span><span class="sxs-lookup"><span data-stu-id="6808c-106">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="6808c-107">Outlook では、受信トレイ内の受信メッセージに対し、一定の条件に基づいて特定の操作を実行するルールを設定できます。</span><span class="sxs-lookup"><span data-stu-id="6808c-107">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="6808c-108">プログラムでこれらのルールにアクセスするには、受信トレイの [フォルダー](mailfolder.md)の **messageRules** ナビゲーション プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="6808c-108">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="6808c-109">各ルールは **messageRule** リソース、利用可能なルールの処理は [messageRuleActions](messageruleactions.md) 複合型、利用可能なルール条件および例外は [messageRulePredicates](messagerulepredicates.md) 複合型で表されます。</span><span class="sxs-lookup"><span data-stu-id="6808c-109">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="6808c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6808c-110">Properties</span></span>
| <span data-ttu-id="6808c-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6808c-111">Property</span></span>     | <span data-ttu-id="6808c-112">型</span><span class="sxs-lookup"><span data-stu-id="6808c-112">Type</span></span>   |<span data-ttu-id="6808c-113">説明</span><span class="sxs-lookup"><span data-stu-id="6808c-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6808c-114">actions</span><span class="sxs-lookup"><span data-stu-id="6808c-114">actions</span></span> | [<span data-ttu-id="6808c-115">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="6808c-115">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="6808c-116">該当する条件が満たされた場合にメッセージに対して実行されるアクション。</span><span class="sxs-lookup"><span data-stu-id="6808c-116">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="6808c-117">conditions</span><span class="sxs-lookup"><span data-stu-id="6808c-117">conditions</span></span> | [<span data-ttu-id="6808c-118">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="6808c-118">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="6808c-119">該当するルール アクションをトリガーするために満たす必要のある条件。</span><span class="sxs-lookup"><span data-stu-id="6808c-119">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="6808c-120">displayName</span><span class="sxs-lookup"><span data-stu-id="6808c-120">displayName</span></span> | <span data-ttu-id="6808c-121">String</span><span class="sxs-lookup"><span data-stu-id="6808c-121">String</span></span> | <span data-ttu-id="6808c-122">ルールの表示名。</span><span class="sxs-lookup"><span data-stu-id="6808c-122">The display name of the rule.</span></span> |
| <span data-ttu-id="6808c-123">exceptions</span><span class="sxs-lookup"><span data-stu-id="6808c-123">exceptions</span></span> | [<span data-ttu-id="6808c-124">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="6808c-124">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="6808c-125">ルールの例外条件。</span><span class="sxs-lookup"><span data-stu-id="6808c-125">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="6808c-126">hasError</span><span class="sxs-lookup"><span data-stu-id="6808c-126">hasError</span></span> | <span data-ttu-id="6808c-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="6808c-127">Boolean</span></span> | <span data-ttu-id="6808c-128">ルールがエラー状態かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6808c-128">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="6808c-129">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6808c-129">Read-only.</span></span> |
| <span data-ttu-id="6808c-130">id</span><span class="sxs-lookup"><span data-stu-id="6808c-130">id</span></span> |<span data-ttu-id="6808c-131">String</span><span class="sxs-lookup"><span data-stu-id="6808c-131">String</span></span>|<span data-ttu-id="6808c-132">ルールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6808c-132">The unique identifier of the rule.</span></span> <span data-ttu-id="6808c-133">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6808c-133">Read-only.</span></span>|
| <span data-ttu-id="6808c-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6808c-134">isEnabled</span></span> | <span data-ttu-id="6808c-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="6808c-135">Boolean</span></span> | <span data-ttu-id="6808c-136">メッセージに対するルールの適用が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6808c-136">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="6808c-137">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="6808c-137">isReadOnly</span></span> | <span data-ttu-id="6808c-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="6808c-138">Boolean</span></span> | <span data-ttu-id="6808c-139">ルールが読み取り専用のため、ルールの REST API による変更や削除ができないことを示します。</span><span class="sxs-lookup"><span data-stu-id="6808c-139">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="6808c-140">sequence</span><span class="sxs-lookup"><span data-stu-id="6808c-140">sequence</span></span> | <span data-ttu-id="6808c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6808c-141">Int32</span></span> | <span data-ttu-id="6808c-142">他のルールもある中で、そのルールが実行される順序を示します。</span><span class="sxs-lookup"><span data-stu-id="6808c-142">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6808c-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6808c-143">JSON representation</span></span>
<span data-ttu-id="6808c-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6808c-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRule"
}-->

```json
{
  "actions": {"@odata.type": "microsoft.graph.messageRuleActions"},
  "conditions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "displayName": "String",
  "exceptions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "hasError": "Boolean",
  "id": "String",
  "isEnabled": "Boolean",
  "isReadOnly": "Boolean",
  "sequence": "Int32"
}

```

## <a name="methods"></a><span data-ttu-id="6808c-145">メソッド</span><span class="sxs-lookup"><span data-stu-id="6808c-145">Methods</span></span>
| <span data-ttu-id="6808c-146">メソッド</span><span class="sxs-lookup"><span data-stu-id="6808c-146">Method</span></span>           | <span data-ttu-id="6808c-147">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6808c-147">Return Type</span></span>    |<span data-ttu-id="6808c-148">説明</span><span class="sxs-lookup"><span data-stu-id="6808c-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6808c-149">ルールの一覧表示</span><span class="sxs-lookup"><span data-stu-id="6808c-149">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="6808c-150">[messageRule](messagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6808c-150">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="6808c-151">ユーザーの受信トレイに定義されているすべての **messageRule** オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="6808c-151">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="6808c-152">ルールの取得</span><span class="sxs-lookup"><span data-stu-id="6808c-152">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="6808c-153">messageRule</span><span class="sxs-lookup"><span data-stu-id="6808c-153">messageRule</span></span>](messagerule.md) |<span data-ttu-id="6808c-154">**messageRule** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6808c-154">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="6808c-155">作成</span><span class="sxs-lookup"><span data-stu-id="6808c-155">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="6808c-156">messageRule</span><span class="sxs-lookup"><span data-stu-id="6808c-156">messageRule</span></span>](messagerule.md) |<span data-ttu-id="6808c-157">条件とアクションのセットを指定して **messageRule** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6808c-157">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="6808c-158">更新</span><span class="sxs-lookup"><span data-stu-id="6808c-158">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="6808c-159">messageRule</span><span class="sxs-lookup"><span data-stu-id="6808c-159">messageRule</span></span>](messagerule.md) |<span data-ttu-id="6808c-160">**messageRule** オブジェクトの書き込み可能なプロパティを変更し、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="6808c-160">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="6808c-161">削除</span><span class="sxs-lookup"><span data-stu-id="6808c-161">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="6808c-162">なし</span><span class="sxs-lookup"><span data-stu-id="6808c-162">None</span></span> |<span data-ttu-id="6808c-163">指定した **messageRule** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="6808c-163">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->