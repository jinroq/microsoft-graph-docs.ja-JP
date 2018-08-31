# <a name="messagerule-resource-type"></a><span data-ttu-id="03ae4-101">messageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03ae4-101">messageRule resource type</span></span>


<span data-ttu-id="03ae4-102">ユーザーの受信トレイ内のメッセージに適用されるルールです。</span><span class="sxs-lookup"><span data-stu-id="03ae4-102">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="03ae4-103">Outlook では、受信トレイ内の受信メッセージに対し、一定の条件に基づいて特定の操作を実行するルールを設定できます。</span><span class="sxs-lookup"><span data-stu-id="03ae4-103">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="03ae4-104">プログラムでこれらのルールにアクセスするには、受信トレイの [フォルダー](mailfolder.md)の **messageRules** ナビゲーション プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="03ae4-104">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="03ae4-105">各ルールは **messageRule** リソース、利用可能なルールの処理は [messageRuleActions](messageruleactions.md) 複合型、利用可能なルール条件および例外は [messageRulePredicates](messagerulepredicates.md) 複合型で表されます。</span><span class="sxs-lookup"><span data-stu-id="03ae4-105">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="03ae4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03ae4-106">Properties</span></span>
| <span data-ttu-id="03ae4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03ae4-107">Property</span></span>     | <span data-ttu-id="03ae4-108">タイプ</span><span class="sxs-lookup"><span data-stu-id="03ae4-108">Type</span></span>   |<span data-ttu-id="03ae4-109">説明</span><span class="sxs-lookup"><span data-stu-id="03ae4-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="03ae4-110">actions</span><span class="sxs-lookup"><span data-stu-id="03ae4-110">actions</span></span> | [<span data-ttu-id="03ae4-111">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="03ae4-111">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="03ae4-112">該当する条件が満たされた場合にメッセージに対して実行されるアクション。</span><span class="sxs-lookup"><span data-stu-id="03ae4-112">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="03ae4-113">conditions</span><span class="sxs-lookup"><span data-stu-id="03ae4-113">conditions</span></span> | [<span data-ttu-id="03ae4-114">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="03ae4-114">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="03ae4-115">該当するルール アクションをトリガーするために満たす必要のある条件。</span><span class="sxs-lookup"><span data-stu-id="03ae4-115">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="03ae4-116">displayName</span><span class="sxs-lookup"><span data-stu-id="03ae4-116">displayName</span></span> | <span data-ttu-id="03ae4-117">String</span><span class="sxs-lookup"><span data-stu-id="03ae4-117">String</span></span> | <span data-ttu-id="03ae4-118">ルールの表示名。</span><span class="sxs-lookup"><span data-stu-id="03ae4-118">The display name of the rule.</span></span> |
| <span data-ttu-id="03ae4-119">exceptions</span><span class="sxs-lookup"><span data-stu-id="03ae4-119">exceptions</span></span> | [<span data-ttu-id="03ae4-120">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="03ae4-120">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="03ae4-121">ルールの例外条件。</span><span class="sxs-lookup"><span data-stu-id="03ae4-121">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="03ae4-122">hasError</span><span class="sxs-lookup"><span data-stu-id="03ae4-122">hasError</span></span> | <span data-ttu-id="03ae4-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="03ae4-123">Boolean</span></span> | <span data-ttu-id="03ae4-124">ルールがエラー状態かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="03ae4-124">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="03ae4-125">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="03ae4-125">Read-only.</span></span> |
| <span data-ttu-id="03ae4-126">id</span><span class="sxs-lookup"><span data-stu-id="03ae4-126">id</span></span> |<span data-ttu-id="03ae4-127">String</span><span class="sxs-lookup"><span data-stu-id="03ae4-127">String</span></span>|<span data-ttu-id="03ae4-128">ルールの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="03ae4-128">The unique identifier of the rule.</span></span> <span data-ttu-id="03ae4-129">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="03ae4-129">Read-only.</span></span>|
| <span data-ttu-id="03ae4-130">isEnabled</span><span class="sxs-lookup"><span data-stu-id="03ae4-130">isEnabled</span></span> | <span data-ttu-id="03ae4-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="03ae4-131">Boolean</span></span> | <span data-ttu-id="03ae4-132">メッセージに対するルールの適用が有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="03ae4-132">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="03ae4-133">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="03ae4-133">isReadOnly</span></span> | <span data-ttu-id="03ae4-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="03ae4-134">Boolean</span></span> | <span data-ttu-id="03ae4-135">ルールが読み取り専用のため、ルールの REST API による変更や削除ができないことを示します。</span><span class="sxs-lookup"><span data-stu-id="03ae4-135">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="03ae4-136">sequence</span><span class="sxs-lookup"><span data-stu-id="03ae4-136">sequence</span></span> | <span data-ttu-id="03ae4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="03ae4-137">Int32</span></span> | <span data-ttu-id="03ae4-138">他のルールもある中で、そのルールが実行される順序を示します。</span><span class="sxs-lookup"><span data-stu-id="03ae4-138">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="03ae4-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03ae4-139">JSON representation</span></span>
<span data-ttu-id="03ae4-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="03ae4-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
   "baseType": "microsoft.graph.entity",
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

## <a name="methods"></a><span data-ttu-id="03ae4-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="03ae4-141">Methods</span></span>
| <span data-ttu-id="03ae4-142">メソッド</span><span class="sxs-lookup"><span data-stu-id="03ae4-142">Method</span></span>           | <span data-ttu-id="03ae4-143">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="03ae4-143">Return Type</span></span>    |<span data-ttu-id="03ae4-144">説明</span><span class="sxs-lookup"><span data-stu-id="03ae4-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03ae4-145">ルールの一覧表示</span><span class="sxs-lookup"><span data-stu-id="03ae4-145">List rules</span></span>](../api/mailfolder_list_messagerules.md) | <span data-ttu-id="03ae4-146">[messageRule](messagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="03ae4-146">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="03ae4-147">ユーザーの受信トレイに定義されているすべての **messageRule** オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="03ae4-147">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="03ae4-148">ルールの取得</span><span class="sxs-lookup"><span data-stu-id="03ae4-148">Get rule</span></span>](../api/messagerule_get.md) | [<span data-ttu-id="03ae4-149">messageRule</span><span class="sxs-lookup"><span data-stu-id="03ae4-149">messageRule</span></span>](messagerule.md) |<span data-ttu-id="03ae4-150">**messageRule** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="03ae4-150">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="03ae4-151">作成</span><span class="sxs-lookup"><span data-stu-id="03ae4-151">Create</span></span>](../api/mailfolder_post_messagerules.md) | [<span data-ttu-id="03ae4-152">messageRule</span><span class="sxs-lookup"><span data-stu-id="03ae4-152">messageRule</span></span>](messagerule.md) |<span data-ttu-id="03ae4-153">条件とアクションのセットを指定して **messageRule** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="03ae4-153">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="03ae4-154">更新</span><span class="sxs-lookup"><span data-stu-id="03ae4-154">Update</span></span>](../api/messagerule_update.md) | [<span data-ttu-id="03ae4-155">messageRule</span><span class="sxs-lookup"><span data-stu-id="03ae4-155">messageRule</span></span>](messagerule.md) |<span data-ttu-id="03ae4-156">**messageRule** オブジェクトの書き込み可能なプロパティを変更し、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="03ae4-156">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="03ae4-157">削除</span><span class="sxs-lookup"><span data-stu-id="03ae4-157">Delete</span></span>](../api/messagerule_delete.md) | <span data-ttu-id="03ae4-158">なし</span><span class="sxs-lookup"><span data-stu-id="03ae4-158">None</span></span> |<span data-ttu-id="03ae4-159">指定した **messageRule** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="03ae4-159">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->