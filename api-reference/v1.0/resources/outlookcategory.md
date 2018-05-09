# <a name="outlookcategory-resource-type"></a><span data-ttu-id="9b908-101">outlookCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b908-101">outlookCategory resource type</span></span>


<span data-ttu-id="9b908-102">ユーザーが Outlook アイテム (メッセージやイベントなど) をグループ化するために使用できるカテゴリを表します。</span><span class="sxs-lookup"><span data-stu-id="9b908-102">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="9b908-103">ユーザーはマスター リストにカテゴリを定義し、これらのユーザー定義カテゴリの 1 つ以上をアイテムに適用できます。</span><span class="sxs-lookup"><span data-stu-id="9b908-103">The user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="9b908-104">カテゴリを[作成](../api/outlookuser_post_mastercategories.md)してユーザーのマスター カテゴリ リストに定義するには、REST API を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="9b908-104">Using the REST API, you can [create](../api/outlookuser_post_mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="9b908-105">また、[このマスター カテゴリ リストの取得](../api/outlookuser_list_mastercategories.md)、[特定のカテゴリの取得](../api/outlookcategory_get.md)、カテゴリに関連付けられている色の[更新](../api/outlookcategory_update.md)、カテゴリの[削除](../api/outlookcategory_delete.md)などの操作を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="9b908-105">You can also [get this master list of categories](../api/outlookuser_list_mastercategories.md), [get a specific category](../api/outlookcategory_get.md), [update](../api/outlookcategory_update.md) the color associated with a category, or [delete](../api/outlookcategory_delete.md) a category.</span></span> <span data-ttu-id="9b908-106">カテゴリをアイテムに適用するには、適用対象とするアイテムの **categories** コレクションに、カテゴリの **displayName** プロパティを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="9b908-106">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="9b908-107">カテゴリを割り当てることができるリソースには、[contact](contact.md)、[event](event.md)、[message](message.md)、[post](post.md) があります。</span><span class="sxs-lookup"><span data-stu-id="9b908-107">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), and [post](post.md).</span></span>   

<span data-ttu-id="9b908-108">各カテゴリを特徴付けるプロパティには、**displayName** と **color** の 2 つがあります。</span><span class="sxs-lookup"><span data-stu-id="9b908-108">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="9b908-109">**displayName** の値は、ユーザーのマスター リスト内で一意でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="9b908-109">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="9b908-110">一方、**color** には一意の値を設定する必要はありません。マスター リストに含まれる複数のカテゴリに、同じ色をマッピングすることができます。</span><span class="sxs-lookup"><span data-stu-id="9b908-110">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="9b908-111">ユーザーのマスター リスト内のカテゴリには、最大 25 種類の色をマッピングできます。</span><span class="sxs-lookup"><span data-stu-id="9b908-111">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="9b908-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b908-112">Properties</span></span>
| <span data-ttu-id="9b908-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b908-113">Property</span></span>     | <span data-ttu-id="9b908-114">型</span><span class="sxs-lookup"><span data-stu-id="9b908-114">Type</span></span>   |<span data-ttu-id="9b908-115">説明</span><span class="sxs-lookup"><span data-stu-id="9b908-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b908-116">displayName</span><span class="sxs-lookup"><span data-stu-id="9b908-116">displayName</span></span>|<span data-ttu-id="9b908-117">String</span><span class="sxs-lookup"><span data-stu-id="9b908-117">String</span></span>|<span data-ttu-id="9b908-118">ユーザーのメールボックス内でカテゴリを識別する一意の名前。</span><span class="sxs-lookup"><span data-stu-id="9b908-118">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="9b908-119">カテゴリが作成された後に、この名前を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="9b908-119">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="9b908-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="9b908-120">Read-only.</span></span>|
|<span data-ttu-id="9b908-121">color</span><span class="sxs-lookup"><span data-stu-id="9b908-121">color</span></span>|<span data-ttu-id="9b908-122">String</span><span class="sxs-lookup"><span data-stu-id="9b908-122">String</span></span>|<span data-ttu-id="9b908-123">カテゴリを特徴付ける、あらかじめ設定された色の定数。定数は、事前定義された 25 種類の色のいずれか 1 つにマッピングされています。</span><span class="sxs-lookup"><span data-stu-id="9b908-123">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="9b908-124">次の注を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b908-124">See the note below.</span></span> |

> <span data-ttu-id="9b908-125">**注:** **color** に使用できる値は、あらかじめ設定されている `None`、`preset0`、`preset1` などの定数です。</span><span class="sxs-lookup"><span data-stu-id="9b908-125">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="9b908-126">設定済みの定数は、それぞれ 1 つの色にマッピングされています。ただし、実際の色は、カテゴリを表示する Outloook クライアントに依存します。</span><span class="sxs-lookup"><span data-stu-id="9b908-126">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="9b908-127">次の表に、設定済みの各定数に Outlook (デスクトップ クライアント) でマッピングされている色を記載します。</span><span class="sxs-lookup"><span data-stu-id="9b908-127">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="9b908-128">設定済みの定数</span><span class="sxs-lookup"><span data-stu-id="9b908-128">Pre-set constant</span></span>  | <span data-ttu-id="9b908-129">Outlook でマッピングされている色</span><span class="sxs-lookup"><span data-stu-id="9b908-129">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9b908-130">None</span><span class="sxs-lookup"><span data-stu-id="9b908-130">None</span></span> | <span data-ttu-id="9b908-131">マッピングされている色なし</span><span class="sxs-lookup"><span data-stu-id="9b908-131">No color mapped</span></span> |
| <span data-ttu-id="9b908-132">Preset0</span><span class="sxs-lookup"><span data-stu-id="9b908-132">Preset0</span></span> | <span data-ttu-id="9b908-133">赤</span><span class="sxs-lookup"><span data-stu-id="9b908-133">Red</span></span> |
| <span data-ttu-id="9b908-134">Preset1</span><span class="sxs-lookup"><span data-stu-id="9b908-134">Preset1</span></span> | <span data-ttu-id="9b908-135">オレンジ</span><span class="sxs-lookup"><span data-stu-id="9b908-135">Orange</span></span> |
| <span data-ttu-id="9b908-136">Preset2</span><span class="sxs-lookup"><span data-stu-id="9b908-136">Preset2</span></span> | <span data-ttu-id="9b908-137">茶</span><span class="sxs-lookup"><span data-stu-id="9b908-137">Brown</span></span> |
| <span data-ttu-id="9b908-138">Preset3</span><span class="sxs-lookup"><span data-stu-id="9b908-138">Preset3</span></span> | <span data-ttu-id="9b908-139">黄</span><span class="sxs-lookup"><span data-stu-id="9b908-139">Yellow</span></span> |
| <span data-ttu-id="9b908-140">Preset4</span><span class="sxs-lookup"><span data-stu-id="9b908-140">Preset4</span></span> | <span data-ttu-id="9b908-141">緑</span><span class="sxs-lookup"><span data-stu-id="9b908-141">Green</span></span> |
| <span data-ttu-id="9b908-142">Preset5</span><span class="sxs-lookup"><span data-stu-id="9b908-142">Preset5</span></span> | <span data-ttu-id="9b908-143">青緑</span><span class="sxs-lookup"><span data-stu-id="9b908-143">Teal</span></span> |
| <span data-ttu-id="9b908-144">Preset6</span><span class="sxs-lookup"><span data-stu-id="9b908-144">Preset6</span></span> | <span data-ttu-id="9b908-145">オリーブ</span><span class="sxs-lookup"><span data-stu-id="9b908-145">Olive</span></span> |
| <span data-ttu-id="9b908-146">Preset7</span><span class="sxs-lookup"><span data-stu-id="9b908-146">Preset7</span></span> | <span data-ttu-id="9b908-147">青</span><span class="sxs-lookup"><span data-stu-id="9b908-147">Blue</span></span> |
| <span data-ttu-id="9b908-148">Preset8</span><span class="sxs-lookup"><span data-stu-id="9b908-148">Preset8</span></span> | <span data-ttu-id="9b908-149">紫</span><span class="sxs-lookup"><span data-stu-id="9b908-149">Purple</span></span> |
| <span data-ttu-id="9b908-150">Preset9</span><span class="sxs-lookup"><span data-stu-id="9b908-150">Preset9</span></span> | <span data-ttu-id="9b908-151">深紅</span><span class="sxs-lookup"><span data-stu-id="9b908-151">Cranberry</span></span> |
| <span data-ttu-id="9b908-152">Preset10</span><span class="sxs-lookup"><span data-stu-id="9b908-152">Preset10</span></span> | <span data-ttu-id="9b908-153">鋼色</span><span class="sxs-lookup"><span data-stu-id="9b908-153">Steel</span></span> |
| <span data-ttu-id="9b908-154">Preset11</span><span class="sxs-lookup"><span data-stu-id="9b908-154">Preset11</span></span> | <span data-ttu-id="9b908-155">DarkSteel</span><span class="sxs-lookup"><span data-stu-id="9b908-155">DarkSteel</span></span> |
| <span data-ttu-id="9b908-156">Preset12</span><span class="sxs-lookup"><span data-stu-id="9b908-156">Preset12</span></span> | <span data-ttu-id="9b908-157">灰色</span><span class="sxs-lookup"><span data-stu-id="9b908-157">Gray</span></span> |
| <span data-ttu-id="9b908-158">Preset13</span><span class="sxs-lookup"><span data-stu-id="9b908-158">Preset13</span></span> | <span data-ttu-id="9b908-159">DarkGray</span><span class="sxs-lookup"><span data-stu-id="9b908-159">DarkGray</span></span> |
| <span data-ttu-id="9b908-160">Preset14</span><span class="sxs-lookup"><span data-stu-id="9b908-160">Preset14</span></span> | <span data-ttu-id="9b908-161">黒</span><span class="sxs-lookup"><span data-stu-id="9b908-161">Black</span></span> |
| <span data-ttu-id="9b908-162">Preset15</span><span class="sxs-lookup"><span data-stu-id="9b908-162">Preset15</span></span> | <span data-ttu-id="9b908-163">DarkRed</span><span class="sxs-lookup"><span data-stu-id="9b908-163">DarkRed</span></span> |
| <span data-ttu-id="9b908-164">Preset16</span><span class="sxs-lookup"><span data-stu-id="9b908-164">Preset16</span></span> | <span data-ttu-id="9b908-165">DarkOrange</span><span class="sxs-lookup"><span data-stu-id="9b908-165">DarkOrange</span></span> |
| <span data-ttu-id="9b908-166">Preset17</span><span class="sxs-lookup"><span data-stu-id="9b908-166">Preset17</span></span> | <span data-ttu-id="9b908-167">DarkBrown</span><span class="sxs-lookup"><span data-stu-id="9b908-167">DarkBrown</span></span> |
| <span data-ttu-id="9b908-168">Preset18</span><span class="sxs-lookup"><span data-stu-id="9b908-168">Preset18</span></span> | <span data-ttu-id="9b908-169">DarkYellow</span><span class="sxs-lookup"><span data-stu-id="9b908-169">DarkYellow</span></span> |
| <span data-ttu-id="9b908-170">Preset19</span><span class="sxs-lookup"><span data-stu-id="9b908-170">Preset19</span></span> | <span data-ttu-id="9b908-171">DarkGreen</span><span class="sxs-lookup"><span data-stu-id="9b908-171">DarkGreen</span></span> |
| <span data-ttu-id="9b908-172">Preset20</span><span class="sxs-lookup"><span data-stu-id="9b908-172">Preset20</span></span> | <span data-ttu-id="9b908-173">DarkTeal</span><span class="sxs-lookup"><span data-stu-id="9b908-173">DarkTeal</span></span> |
| <span data-ttu-id="9b908-174">Preset21</span><span class="sxs-lookup"><span data-stu-id="9b908-174">Preset21</span></span> | <span data-ttu-id="9b908-175">DarkOlive</span><span class="sxs-lookup"><span data-stu-id="9b908-175">DarkOlive</span></span> |
| <span data-ttu-id="9b908-176">Preset22</span><span class="sxs-lookup"><span data-stu-id="9b908-176">Preset22</span></span> | <span data-ttu-id="9b908-177">DarkBlue</span><span class="sxs-lookup"><span data-stu-id="9b908-177">DarkBlue</span></span> |
| <span data-ttu-id="9b908-178">Preset23</span><span class="sxs-lookup"><span data-stu-id="9b908-178">Preset23</span></span> | <span data-ttu-id="9b908-179">DarkPurple</span><span class="sxs-lookup"><span data-stu-id="9b908-179">DarkPurple</span></span> |
| <span data-ttu-id="9b908-180">Preset24</span><span class="sxs-lookup"><span data-stu-id="9b908-180">Preset24</span></span> | <span data-ttu-id="9b908-181">DarkCranberry</span><span class="sxs-lookup"><span data-stu-id="9b908-181">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9b908-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b908-182">JSON representation</span></span>
<span data-ttu-id="9b908-183">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b908-183">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a><span data-ttu-id="9b908-184">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b908-184">Methods</span></span>
| <span data-ttu-id="9b908-185">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b908-185">Method</span></span>           | <span data-ttu-id="9b908-186">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9b908-186">Return Type</span></span>    |<span data-ttu-id="9b908-187">説明</span><span class="sxs-lookup"><span data-stu-id="9b908-187">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b908-188">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="9b908-188">List categories</span></span>](../api/outlookuser_list_mastercategories.md) | <span data-ttu-id="9b908-189">[outlookCategory](../resources/outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9b908-189">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="9b908-190">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="9b908-190">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="9b908-191">カテゴリの取得</span><span class="sxs-lookup"><span data-stu-id="9b908-191">Get category</span></span>](../api/outlookcategory_get.md) | [<span data-ttu-id="9b908-192">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="9b908-192">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="9b908-193">指定した **outlookCategory** オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="9b908-193">Get the properties and relationships of the specified **event** object.</span></span>|
|[<span data-ttu-id="9b908-194">作成</span><span class="sxs-lookup"><span data-stu-id="9b908-194">Create</span></span>](../api/outlookuser_post_mastercategories.md) | [<span data-ttu-id="9b908-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="9b908-195">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="9b908-196">ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9b908-196">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="9b908-197">更新</span><span class="sxs-lookup"><span data-stu-id="9b908-197">Update</span></span>](../api/outlookcategory_update.md) | [<span data-ttu-id="9b908-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="9b908-198">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="9b908-199">指定した **outlookCategory** オブジェクトの書き込み可能な **color** プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9b908-199">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="9b908-200">削除</span><span class="sxs-lookup"><span data-stu-id="9b908-200">Delete</span></span>](../api/outlookcategory_delete.md) | <span data-ttu-id="9b908-201">None</span><span class="sxs-lookup"><span data-stu-id="9b908-201">None</span></span> |<span data-ttu-id="9b908-202">指定した **outlookCategory** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="9b908-202">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
 