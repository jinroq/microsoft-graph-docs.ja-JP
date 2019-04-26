---
title: messageRule リソースの種類
description: ユーザーの受信トレイ内のメッセージに適用されるルールです。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d74d4c6a5121355113a883c5c8096420986b6549
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342260"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="69dad-103">messageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="69dad-103">messageRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69dad-104">ユーザーの受信トレイ内のメッセージに適用されるルールです。</span><span class="sxs-lookup"><span data-stu-id="69dad-104">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="69dad-105">Outlook では、受信トレイ内の受信メッセージに対し、一定の条件に基づいて特定の操作を実行するルールを設定できます。</span><span class="sxs-lookup"><span data-stu-id="69dad-105">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="69dad-106">プログラムでこれらのルールにアクセスするには、受信トレイの [フォルダー](mailfolder.md)の **messageRules** ナビゲーション プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="69dad-106">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="69dad-107">各ルールは **messageRule** リソース、利用可能なルールの処理は [messageRuleActions](messageruleactions.md) 複合型、利用可能なルール条件および例外は [messageRulePredicates](messagerulepredicates.md) 複合型で表されます。</span><span class="sxs-lookup"><span data-stu-id="69dad-107">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="69dad-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69dad-108">Properties</span></span>
| <span data-ttu-id="69dad-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69dad-109">Property</span></span>     | <span data-ttu-id="69dad-110">型</span><span class="sxs-lookup"><span data-stu-id="69dad-110">Type</span></span>   |<span data-ttu-id="69dad-111">説明</span><span class="sxs-lookup"><span data-stu-id="69dad-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="69dad-112">actions</span><span class="sxs-lookup"><span data-stu-id="69dad-112">actions</span></span> | [<span data-ttu-id="69dad-113">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="69dad-113">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="69dad-114">該当する条件が満たされた場合にメッセージに対して実行されるアクション。</span><span class="sxs-lookup"><span data-stu-id="69dad-114">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="69dad-115">conditions</span><span class="sxs-lookup"><span data-stu-id="69dad-115">conditions</span></span> | [<span data-ttu-id="69dad-116">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="69dad-116">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="69dad-117">該当するルール アクションをトリガーするために満たす必要のある条件。</span><span class="sxs-lookup"><span data-stu-id="69dad-117">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="69dad-118">displayName</span><span class="sxs-lookup"><span data-stu-id="69dad-118">displayName</span></span> | <span data-ttu-id="69dad-119">String</span><span class="sxs-lookup"><span data-stu-id="69dad-119">String</span></span> | <span data-ttu-id="69dad-120">ルールの表示名。</span><span class="sxs-lookup"><span data-stu-id="69dad-120">The display name of the rule.</span></span> |
| <span data-ttu-id="69dad-121">exceptions</span><span class="sxs-lookup"><span data-stu-id="69dad-121">exceptions</span></span> | [<span data-ttu-id="69dad-122">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="69dad-122">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="69dad-123">ルールの例外条件。</span><span class="sxs-lookup"><span data-stu-id="69dad-123">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="69dad-124">hasError</span><span class="sxs-lookup"><span data-stu-id="69dad-124">hasError</span></span> | <span data-ttu-id="69dad-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="69dad-125">Boolean</span></span> | <span data-ttu-id="69dad-126">ルールがエラー状態かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="69dad-126">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="69dad-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="69dad-127">Read-only.</span></span> |
| <span data-ttu-id="69dad-128">id</span><span class="sxs-lookup"><span data-stu-id="69dad-128">id</span></span> |<span data-ttu-id="69dad-129">String</span><span class="sxs-lookup"><span data-stu-id="69dad-129">String</span></span>|<span data-ttu-id="69dad-130">ルールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="69dad-130">The unique identifier of the rule.</span></span> <span data-ttu-id="69dad-131">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="69dad-131">Read-only.</span></span>|
| <span data-ttu-id="69dad-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="69dad-132">isEnabled</span></span> | <span data-ttu-id="69dad-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="69dad-133">Boolean</span></span> | <span data-ttu-id="69dad-134">メッセージに対するルールの適用が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="69dad-134">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="69dad-135">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="69dad-135">isReadOnly</span></span> | <span data-ttu-id="69dad-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="69dad-136">Boolean</span></span> | <span data-ttu-id="69dad-137">ルールが読み取り専用のため、ルールの REST API による変更や削除ができないことを示します。</span><span class="sxs-lookup"><span data-stu-id="69dad-137">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="69dad-138">sequence</span><span class="sxs-lookup"><span data-stu-id="69dad-138">sequence</span></span> | <span data-ttu-id="69dad-139">Int32</span><span class="sxs-lookup"><span data-stu-id="69dad-139">Int32</span></span> | <span data-ttu-id="69dad-140">他のルールもある中で、そのルールが実行される順序を示します。</span><span class="sxs-lookup"><span data-stu-id="69dad-140">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="69dad-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69dad-141">JSON representation</span></span>
<span data-ttu-id="69dad-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="69dad-142">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="69dad-143">メソッド</span><span class="sxs-lookup"><span data-stu-id="69dad-143">Methods</span></span>
| <span data-ttu-id="69dad-144">メソッド</span><span class="sxs-lookup"><span data-stu-id="69dad-144">Method</span></span>           | <span data-ttu-id="69dad-145">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="69dad-145">Return Type</span></span>    |<span data-ttu-id="69dad-146">説明</span><span class="sxs-lookup"><span data-stu-id="69dad-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69dad-147">ルールの一覧表示</span><span class="sxs-lookup"><span data-stu-id="69dad-147">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="69dad-148">[messageRule](messagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="69dad-148">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="69dad-149">ユーザーの受信トレイに定義されているすべての **messageRule** オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="69dad-149">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="69dad-150">ルールの取得</span><span class="sxs-lookup"><span data-stu-id="69dad-150">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="69dad-151">messageRule</span><span class="sxs-lookup"><span data-stu-id="69dad-151">messageRule</span></span>](messagerule.md) |<span data-ttu-id="69dad-152">**messageRule** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="69dad-152">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="69dad-153">作成</span><span class="sxs-lookup"><span data-stu-id="69dad-153">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="69dad-154">messageRule</span><span class="sxs-lookup"><span data-stu-id="69dad-154">messageRule</span></span>](messagerule.md) |<span data-ttu-id="69dad-155">条件とアクションのセットを指定して **messageRule** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="69dad-155">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="69dad-156">更新</span><span class="sxs-lookup"><span data-stu-id="69dad-156">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="69dad-157">messageRule</span><span class="sxs-lookup"><span data-stu-id="69dad-157">messageRule</span></span>](messagerule.md) |<span data-ttu-id="69dad-158">**messageRule** オブジェクトの書き込み可能なプロパティを変更し、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="69dad-158">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="69dad-159">削除</span><span class="sxs-lookup"><span data-stu-id="69dad-159">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="69dad-160">なし</span><span class="sxs-lookup"><span data-stu-id="69dad-160">None</span></span> |<span data-ttu-id="69dad-161">指定した **messageRule** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="69dad-161">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
