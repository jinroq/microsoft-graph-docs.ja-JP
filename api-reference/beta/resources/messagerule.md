---
title: messageRule リソースの種類
description: ユーザーの受信トレイ内のメッセージに適用されるルールです。
author: angelgolfer-ms
ms.openlocfilehash: 1824e9a8d840da824efb79eff4b98bac02a8c187
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307729"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="a4e85-103">messageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4e85-103">messageRule resource type</span></span>

> <span data-ttu-id="a4e85-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a4e85-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4e85-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4e85-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4e85-106">ユーザーの受信トレイ内のメッセージに適用されるルールです。</span><span class="sxs-lookup"><span data-stu-id="a4e85-106">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="a4e85-107">Outlook では、受信トレイ内の受信メッセージに対し、一定の条件に基づいて特定の操作を実行するルールを設定できます。</span><span class="sxs-lookup"><span data-stu-id="a4e85-107">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="a4e85-108">プログラムでこれらのルールにアクセスするには、受信トレイの [フォルダー](mailfolder.md)の **messageRules** ナビゲーション プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="a4e85-108">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="a4e85-109">各ルールは **messageRule** リソース、利用可能なルールの処理は [messageRuleActions](messageruleactions.md) 複合型、利用可能なルール条件および例外は [messageRulePredicates](messagerulepredicates.md) 複合型で表されます。</span><span class="sxs-lookup"><span data-stu-id="a4e85-109">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="a4e85-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4e85-110">Properties</span></span>
| <span data-ttu-id="a4e85-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4e85-111">Property</span></span>     | <span data-ttu-id="a4e85-112">種類</span><span class="sxs-lookup"><span data-stu-id="a4e85-112">Type</span></span>   |<span data-ttu-id="a4e85-113">説明</span><span class="sxs-lookup"><span data-stu-id="a4e85-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a4e85-114">actions</span><span class="sxs-lookup"><span data-stu-id="a4e85-114">actions</span></span> | [<span data-ttu-id="a4e85-115">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="a4e85-115">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="a4e85-116">該当する条件が満たされた場合にメッセージに対して実行されるアクション。</span><span class="sxs-lookup"><span data-stu-id="a4e85-116">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="a4e85-117">conditions</span><span class="sxs-lookup"><span data-stu-id="a4e85-117">conditions</span></span> | [<span data-ttu-id="a4e85-118">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="a4e85-118">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="a4e85-119">該当するルール アクションをトリガーするために満たす必要のある条件。</span><span class="sxs-lookup"><span data-stu-id="a4e85-119">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="a4e85-120">displayName</span><span class="sxs-lookup"><span data-stu-id="a4e85-120">displayName</span></span> | <span data-ttu-id="a4e85-121">String</span><span class="sxs-lookup"><span data-stu-id="a4e85-121">String</span></span> | <span data-ttu-id="a4e85-122">ルールの表示名。</span><span class="sxs-lookup"><span data-stu-id="a4e85-122">The display name of the rule.</span></span> |
| <span data-ttu-id="a4e85-123">exceptions</span><span class="sxs-lookup"><span data-stu-id="a4e85-123">exceptions</span></span> | [<span data-ttu-id="a4e85-124">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="a4e85-124">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="a4e85-125">ルールの例外条件。</span><span class="sxs-lookup"><span data-stu-id="a4e85-125">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="a4e85-126">hasError</span><span class="sxs-lookup"><span data-stu-id="a4e85-126">hasError</span></span> | <span data-ttu-id="a4e85-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4e85-127">Boolean</span></span> | <span data-ttu-id="a4e85-128">ルールがエラー状態かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a4e85-128">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="a4e85-129">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a4e85-129">Read-only.</span></span> |
| <span data-ttu-id="a4e85-130">id</span><span class="sxs-lookup"><span data-stu-id="a4e85-130">id</span></span> |<span data-ttu-id="a4e85-131">String</span><span class="sxs-lookup"><span data-stu-id="a4e85-131">String</span></span>|<span data-ttu-id="a4e85-132">ルールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a4e85-132">The unique identifier of the rule.</span></span> <span data-ttu-id="a4e85-133">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a4e85-133">Read-only.</span></span>|
| <span data-ttu-id="a4e85-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a4e85-134">isEnabled</span></span> | <span data-ttu-id="a4e85-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4e85-135">Boolean</span></span> | <span data-ttu-id="a4e85-136">メッセージに対するルールの適用が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a4e85-136">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="a4e85-137">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="a4e85-137">isReadOnly</span></span> | <span data-ttu-id="a4e85-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4e85-138">Boolean</span></span> | <span data-ttu-id="a4e85-139">ルールが読み取り専用のため、ルールの REST API による変更や削除ができないことを示します。</span><span class="sxs-lookup"><span data-stu-id="a4e85-139">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="a4e85-140">sequence</span><span class="sxs-lookup"><span data-stu-id="a4e85-140">sequence</span></span> | <span data-ttu-id="a4e85-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a4e85-141">Int32</span></span> | <span data-ttu-id="a4e85-142">他のルールもある中で、そのルールが実行される順序を示します。</span><span class="sxs-lookup"><span data-stu-id="a4e85-142">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a4e85-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4e85-143">JSON representation</span></span>
<span data-ttu-id="a4e85-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4e85-144">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="a4e85-145">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4e85-145">Methods</span></span>
| <span data-ttu-id="a4e85-146">メソッド</span><span class="sxs-lookup"><span data-stu-id="a4e85-146">Method</span></span>           | <span data-ttu-id="a4e85-147">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a4e85-147">Return Type</span></span>    |<span data-ttu-id="a4e85-148">説明</span><span class="sxs-lookup"><span data-stu-id="a4e85-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4e85-149">ルールの一覧表示</span><span class="sxs-lookup"><span data-stu-id="a4e85-149">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="a4e85-150">[messageRule](messagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a4e85-150">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="a4e85-151">ユーザーの受信トレイに定義されているすべての **messageRule** オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="a4e85-151">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="a4e85-152">ルールの取得</span><span class="sxs-lookup"><span data-stu-id="a4e85-152">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="a4e85-153">messageRule</span><span class="sxs-lookup"><span data-stu-id="a4e85-153">messageRule</span></span>](messagerule.md) |<span data-ttu-id="a4e85-154">**messageRule** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a4e85-154">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="a4e85-155">作成</span><span class="sxs-lookup"><span data-stu-id="a4e85-155">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="a4e85-156">messageRule</span><span class="sxs-lookup"><span data-stu-id="a4e85-156">messageRule</span></span>](messagerule.md) |<span data-ttu-id="a4e85-157">条件とアクションのセットを指定して **messageRule** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a4e85-157">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="a4e85-158">更新</span><span class="sxs-lookup"><span data-stu-id="a4e85-158">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="a4e85-159">messageRule</span><span class="sxs-lookup"><span data-stu-id="a4e85-159">messageRule</span></span>](messagerule.md) |<span data-ttu-id="a4e85-160">**messageRule** オブジェクトの書き込み可能なプロパティを変更し、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="a4e85-160">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="a4e85-161">削除</span><span class="sxs-lookup"><span data-stu-id="a4e85-161">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="a4e85-162">なし</span><span class="sxs-lookup"><span data-stu-id="a4e85-162">None</span></span> |<span data-ttu-id="a4e85-163">指定した **messageRule** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a4e85-163">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->