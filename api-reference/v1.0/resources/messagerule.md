# <a name="messagerule-resource-type"></a><span data-ttu-id="e663b-101">messageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e663b-101">messageRule resource type</span></span>


<span data-ttu-id="e663b-102">ユーザーの受信トレイ内のメッセージに適用されるルールです。</span><span class="sxs-lookup"><span data-stu-id="e663b-102">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="e663b-103">Outlook では、受信トレイ内の受信メッセージに対し、一定の条件に基づいて特定の操作を実行するルールを設定できます。</span><span class="sxs-lookup"><span data-stu-id="e663b-103">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions if certain conditions are met.</span></span> 

<span data-ttu-id="e663b-104">プログラムでこれらのルールにアクセスするには、受信トレイの [フォルダー](mailfolder.md)の **messageRules** ナビゲーション プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="e663b-104">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="e663b-105">各ルールは **messageRule** リソース、利用可能なルールの処理は [messageRuleActions](messageruleactions.md) 複合型、利用可能なルール条件および例外は [messageRulePredicates](messagerulepredicates.md) 複合型で表されます。</span><span class="sxs-lookup"><span data-stu-id="e663b-105">Programmatically, you can access rules through the MessageRules navigation property of the Inbox folder. Each rule is represented by the **MessageRule** resource, available rule actions are represented by the [MessageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [MessageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="e663b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e663b-106">Properties</span></span>
| <span data-ttu-id="e663b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e663b-107">Property</span></span>     | <span data-ttu-id="e663b-108">型</span><span class="sxs-lookup"><span data-stu-id="e663b-108">Type</span></span>   |<span data-ttu-id="e663b-109">説明</span><span class="sxs-lookup"><span data-stu-id="e663b-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e663b-110">actions</span><span class="sxs-lookup"><span data-stu-id="e663b-110">Actions</span></span> | [<span data-ttu-id="e663b-111">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="e663b-111">MessageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="e663b-112">該当する条件が満たされた場合にメッセージに対して実行されるアクション。</span><span class="sxs-lookup"><span data-stu-id="e663b-112">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="e663b-113">conditions</span><span class="sxs-lookup"><span data-stu-id="e663b-113">Conditions</span></span> | [<span data-ttu-id="e663b-114">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e663b-114">MessageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="e663b-115">該当するルール アクションをトリガーするために満たす必要のある条件。</span><span class="sxs-lookup"><span data-stu-id="e663b-115">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="e663b-116">displayName</span><span class="sxs-lookup"><span data-stu-id="e663b-116">displayName</span></span> | <span data-ttu-id="e663b-117">String</span><span class="sxs-lookup"><span data-stu-id="e663b-117">String</span></span> | <span data-ttu-id="e663b-118">ルールの表示名。</span><span class="sxs-lookup"><span data-stu-id="e663b-118">The display name of the rule.</span></span> |
| <span data-ttu-id="e663b-119">exceptions</span><span class="sxs-lookup"><span data-stu-id="e663b-119">exceptions</span></span> | [<span data-ttu-id="e663b-120">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e663b-120">MessageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="e663b-121">ルールの例外条件。</span><span class="sxs-lookup"><span data-stu-id="e663b-121">Represents exception conditions for the rule.</span></span> |
| <span data-ttu-id="e663b-122">hasError</span><span class="sxs-lookup"><span data-stu-id="e663b-122">HasError</span></span> | <span data-ttu-id="e663b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="e663b-123">Boolean</span></span> | <span data-ttu-id="e663b-124">ルールがエラー状態かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e663b-124">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="e663b-125">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e663b-125">Read-only.</span></span> |
| <span data-ttu-id="e663b-126">id</span><span class="sxs-lookup"><span data-stu-id="e663b-126">id</span></span> |<span data-ttu-id="e663b-127">String</span><span class="sxs-lookup"><span data-stu-id="e663b-127">String</span></span>|<span data-ttu-id="e663b-128">ルールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e663b-128">The unique identifier of the rule.</span></span> <span data-ttu-id="e663b-129">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e663b-129">Read-only.</span></span>|
| <span data-ttu-id="e663b-130">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e663b-130">IsEnabled</span></span> | <span data-ttu-id="e663b-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="e663b-131">Boolean</span></span> | <span data-ttu-id="e663b-132">メッセージに対するルールの適用が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e663b-132">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="e663b-133">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="e663b-133">IsReadOnly</span></span> | <span data-ttu-id="e663b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="e663b-134">Boolean</span></span> | <span data-ttu-id="e663b-135">ルールが読み取り専用のため、ルールの REST API による変更や削除ができないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e663b-135">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="e663b-136">sequence</span><span class="sxs-lookup"><span data-stu-id="e663b-136">Sequence</span></span> | <span data-ttu-id="e663b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e663b-137">Int32</span></span> | <span data-ttu-id="e663b-138">他のルールもある中で、そのルールが実行される順序を示します。</span><span class="sxs-lookup"><span data-stu-id="e663b-138">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e663b-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e663b-139">JSON representation</span></span>
<span data-ttu-id="e663b-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e663b-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="e663b-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="e663b-141">Methods</span></span>
| <span data-ttu-id="e663b-142">メソッド</span><span class="sxs-lookup"><span data-stu-id="e663b-142">Method</span></span>           | <span data-ttu-id="e663b-143">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e663b-143">Return Type</span></span>    |<span data-ttu-id="e663b-144">説明</span><span class="sxs-lookup"><span data-stu-id="e663b-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e663b-145">ルールの一覧表示</span><span class="sxs-lookup"><span data-stu-id="e663b-145">List rules</span></span>](../api/mailfolder_list_messagerules.md) | <span data-ttu-id="e663b-146">[messageRule](messagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e663b-146">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="e663b-147">ユーザーの受信トレイに定義されているすべての **messageRule** オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="e663b-147">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="e663b-148">ルールの取得</span><span class="sxs-lookup"><span data-stu-id="e663b-148">Get a specific rule</span></span>](../api/messagerule_get.md) | [<span data-ttu-id="e663b-149">messageRule</span><span class="sxs-lookup"><span data-stu-id="e663b-149">messageRule</span></span>](messagerule.md) |<span data-ttu-id="e663b-150">**messageRule** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e663b-150">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="e663b-151">作成</span><span class="sxs-lookup"><span data-stu-id="e663b-151">Create</span></span>](../api/mailfolder_post_messagerules.md) | [<span data-ttu-id="e663b-152">messageRule</span><span class="sxs-lookup"><span data-stu-id="e663b-152">messageRule</span></span>](messagerule.md) |<span data-ttu-id="e663b-153">条件とアクションのセットを指定して **messageRule** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e663b-153">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="e663b-154">更新</span><span class="sxs-lookup"><span data-stu-id="e663b-154">Update</span></span>](../api/messagerule_update.md) | [<span data-ttu-id="e663b-155">messageRule</span><span class="sxs-lookup"><span data-stu-id="e663b-155">messageRule</span></span>](messagerule.md) |<span data-ttu-id="e663b-156">**messageRule** オブジェクトの書き込み可能なプロパティを変更し、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="e663b-156">Change writable properties on a rule and save the changes.</span></span> |
|[<span data-ttu-id="e663b-157">削除</span><span class="sxs-lookup"><span data-stu-id="e663b-157">Delete</span></span>](../api/messagerule_delete.md) | <span data-ttu-id="e663b-158">なし</span><span class="sxs-lookup"><span data-stu-id="e663b-158">None</span></span> |<span data-ttu-id="e663b-159">指定した **messageRule** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e663b-159">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->