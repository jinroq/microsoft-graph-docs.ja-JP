---
title: outlookCategory リソースの種類
description: ユーザーが Outlook アイテム (メッセージやイベントなど) をグループ化するために使用できるカテゴリを表します。 Outlook では、ユーザーが、マスター] ボックスの一覧でカテゴリを定義し、これらのユーザー定義の 1 つ以上を適用することができます。
ms.openlocfilehash: 073441894989ee4193018a404b0472a5f1562e4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067226"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="a8a87-104">outlookCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a8a87-104">outlookCategory resource type</span></span>

> <span data-ttu-id="a8a87-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a8a87-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8a87-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8a87-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8a87-107">ユーザーが Outlook アイテム (メッセージやイベントなど) をグループ化するために使用できるカテゴリを表します。</span><span class="sxs-lookup"><span data-stu-id="a8a87-107">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="a8a87-108">Outlook では、ユーザーは、マスター] ボックスの一覧でカテゴリを定義し、アイテムを 1 つまたは複数のユーザー定義カテゴリを適用できます。</span><span class="sxs-lookup"><span data-stu-id="a8a87-108">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="a8a87-109">カテゴリを[作成](../api/outlookuser-post-mastercategories.md)してユーザーのマスター カテゴリ リストに定義するには、REST API を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="a8a87-109">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="a8a87-110">また、[このマスター カテゴリ リストの取得](../api/outlookuser-list-mastercategories.md)、[特定のカテゴリの取得](../api/outlookcategory-get.md)、カテゴリに関連付けられている色の[更新](../api/outlookcategory-update.md)、カテゴリの[削除](../api/outlookcategory-delete.md)などの操作を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="a8a87-110">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="a8a87-111">カテゴリをアイテムに適用するには、適用対象とするアイテムの **categories** コレクションに、カテゴリの **displayName** プロパティを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="a8a87-111">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="a8a87-112">カテゴリを割り当てることができるリソースには、[連絡先](contact.md)、[イベント](event.md)、[メッセージ](message.md)、 [outlookTask](outlooktask.md)、および[投稿](post.md)が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a8a87-112">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="a8a87-113">各カテゴリを特徴付けるプロパティには、**displayName** と **color** の 2 つがあります。</span><span class="sxs-lookup"><span data-stu-id="a8a87-113">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="a8a87-114">**displayName** の値は、ユーザーのマスター リスト内で一意でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="a8a87-114">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="a8a87-115">一方、**color** には一意の値を設定する必要はありません。マスター リストに含まれる複数のカテゴリに、同じ色をマッピングすることができます。</span><span class="sxs-lookup"><span data-stu-id="a8a87-115">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="a8a87-116">ユーザーのマスター リスト内のカテゴリには、最大 25 種類の色をマッピングできます。</span><span class="sxs-lookup"><span data-stu-id="a8a87-116">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="a8a87-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8a87-117">Properties</span></span>
| <span data-ttu-id="a8a87-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8a87-118">Property</span></span>     | <span data-ttu-id="a8a87-119">型</span><span class="sxs-lookup"><span data-stu-id="a8a87-119">Type</span></span>   |<span data-ttu-id="a8a87-120">説明</span><span class="sxs-lookup"><span data-stu-id="a8a87-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8a87-121">displayName</span><span class="sxs-lookup"><span data-stu-id="a8a87-121">displayName</span></span>|<span data-ttu-id="a8a87-122">String</span><span class="sxs-lookup"><span data-stu-id="a8a87-122">String</span></span>|<span data-ttu-id="a8a87-123">ユーザーのメールボックス内でカテゴリを識別する一意の名前。</span><span class="sxs-lookup"><span data-stu-id="a8a87-123">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="a8a87-124">カテゴリが作成された後に、この名前を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="a8a87-124">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="a8a87-125">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a8a87-125">Read-only.</span></span>|
|<span data-ttu-id="a8a87-126">color</span><span class="sxs-lookup"><span data-stu-id="a8a87-126">color</span></span>|<span data-ttu-id="a8a87-127">String</span><span class="sxs-lookup"><span data-stu-id="a8a87-127">String</span></span>|<span data-ttu-id="a8a87-128">カテゴリを特徴付ける、あらかじめ設定された色の定数。定数は、事前定義された 25 種類の色のいずれか 1 つにマッピングされています。</span><span class="sxs-lookup"><span data-stu-id="a8a87-128">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="a8a87-129">次の注を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8a87-129">See the note below.</span></span> |

> <span data-ttu-id="a8a87-130">**注:** **color** に使用できる値は、あらかじめ設定されている `None`、`preset0`、`preset1` などの定数です。</span><span class="sxs-lookup"><span data-stu-id="a8a87-130">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="a8a87-131">設定済みの定数は、それぞれ 1 つの色にマッピングされています。ただし、実際の色は、カテゴリを表示する Outloook クライアントに依存します。</span><span class="sxs-lookup"><span data-stu-id="a8a87-131">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="a8a87-132">次の表に、設定済みの各定数に Outlook (デスクトップ クライアント) でマッピングされている色を記載します。</span><span class="sxs-lookup"><span data-stu-id="a8a87-132">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="a8a87-133">設定済みの定数</span><span class="sxs-lookup"><span data-stu-id="a8a87-133">Pre-set constant</span></span>  | <span data-ttu-id="a8a87-134">Outlook でマッピングされている色</span><span class="sxs-lookup"><span data-stu-id="a8a87-134">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8a87-135">None</span><span class="sxs-lookup"><span data-stu-id="a8a87-135">None</span></span> | <span data-ttu-id="a8a87-136">マッピングされている色なし</span><span class="sxs-lookup"><span data-stu-id="a8a87-136">No color mapped</span></span> |
| <span data-ttu-id="a8a87-137">Preset0</span><span class="sxs-lookup"><span data-stu-id="a8a87-137">Preset0</span></span> | <span data-ttu-id="a8a87-138">赤</span><span class="sxs-lookup"><span data-stu-id="a8a87-138">Red</span></span> |
| <span data-ttu-id="a8a87-139">Preset1</span><span class="sxs-lookup"><span data-stu-id="a8a87-139">Preset1</span></span> | <span data-ttu-id="a8a87-140">オレンジ</span><span class="sxs-lookup"><span data-stu-id="a8a87-140">Orange</span></span> |
| <span data-ttu-id="a8a87-141">Preset2</span><span class="sxs-lookup"><span data-stu-id="a8a87-141">Preset2</span></span> | <span data-ttu-id="a8a87-142">茶</span><span class="sxs-lookup"><span data-stu-id="a8a87-142">Brown</span></span> |
| <span data-ttu-id="a8a87-143">Preset3</span><span class="sxs-lookup"><span data-stu-id="a8a87-143">Preset3</span></span> | <span data-ttu-id="a8a87-144">黄</span><span class="sxs-lookup"><span data-stu-id="a8a87-144">Yellow</span></span> |
| <span data-ttu-id="a8a87-145">Preset4</span><span class="sxs-lookup"><span data-stu-id="a8a87-145">Preset4</span></span> | <span data-ttu-id="a8a87-146">緑</span><span class="sxs-lookup"><span data-stu-id="a8a87-146">Green</span></span> |
| <span data-ttu-id="a8a87-147">Preset5</span><span class="sxs-lookup"><span data-stu-id="a8a87-147">Preset5</span></span> | <span data-ttu-id="a8a87-148">青緑</span><span class="sxs-lookup"><span data-stu-id="a8a87-148">Teal</span></span> |
| <span data-ttu-id="a8a87-149">Preset6</span><span class="sxs-lookup"><span data-stu-id="a8a87-149">Preset6</span></span> | <span data-ttu-id="a8a87-150">オリーブ</span><span class="sxs-lookup"><span data-stu-id="a8a87-150">Olive</span></span> |
| <span data-ttu-id="a8a87-151">Preset7</span><span class="sxs-lookup"><span data-stu-id="a8a87-151">Preset7</span></span> | <span data-ttu-id="a8a87-152">青</span><span class="sxs-lookup"><span data-stu-id="a8a87-152">Blue</span></span> |
| <span data-ttu-id="a8a87-153">Preset8</span><span class="sxs-lookup"><span data-stu-id="a8a87-153">Preset8</span></span> | <span data-ttu-id="a8a87-154">紫</span><span class="sxs-lookup"><span data-stu-id="a8a87-154">Purple</span></span> |
| <span data-ttu-id="a8a87-155">Preset9</span><span class="sxs-lookup"><span data-stu-id="a8a87-155">Preset9</span></span> | <span data-ttu-id="a8a87-156">深紅</span><span class="sxs-lookup"><span data-stu-id="a8a87-156">Cranberry</span></span> |
| <span data-ttu-id="a8a87-157">Preset10</span><span class="sxs-lookup"><span data-stu-id="a8a87-157">Preset10</span></span> | <span data-ttu-id="a8a87-158">鋼色</span><span class="sxs-lookup"><span data-stu-id="a8a87-158">Steel</span></span> |
| <span data-ttu-id="a8a87-159">Preset11</span><span class="sxs-lookup"><span data-stu-id="a8a87-159">Preset11</span></span> | <span data-ttu-id="a8a87-160">DarkSteel</span><span class="sxs-lookup"><span data-stu-id="a8a87-160">DarkSteel</span></span> |
| <span data-ttu-id="a8a87-161">Preset12</span><span class="sxs-lookup"><span data-stu-id="a8a87-161">Preset12</span></span> | <span data-ttu-id="a8a87-162">灰色</span><span class="sxs-lookup"><span data-stu-id="a8a87-162">Gray</span></span> |
| <span data-ttu-id="a8a87-163">Preset13</span><span class="sxs-lookup"><span data-stu-id="a8a87-163">Preset13</span></span> | <span data-ttu-id="a8a87-164">DarkGray</span><span class="sxs-lookup"><span data-stu-id="a8a87-164">DarkGray</span></span> |
| <span data-ttu-id="a8a87-165">Preset14</span><span class="sxs-lookup"><span data-stu-id="a8a87-165">Preset14</span></span> | <span data-ttu-id="a8a87-166">黒</span><span class="sxs-lookup"><span data-stu-id="a8a87-166">Black</span></span> |
| <span data-ttu-id="a8a87-167">Preset15</span><span class="sxs-lookup"><span data-stu-id="a8a87-167">Preset15</span></span> | <span data-ttu-id="a8a87-168">DarkRed</span><span class="sxs-lookup"><span data-stu-id="a8a87-168">DarkRed</span></span> |
| <span data-ttu-id="a8a87-169">Preset16</span><span class="sxs-lookup"><span data-stu-id="a8a87-169">Preset16</span></span> | <span data-ttu-id="a8a87-170">DarkOrange</span><span class="sxs-lookup"><span data-stu-id="a8a87-170">DarkOrange</span></span> |
| <span data-ttu-id="a8a87-171">Preset17</span><span class="sxs-lookup"><span data-stu-id="a8a87-171">Preset17</span></span> | <span data-ttu-id="a8a87-172">DarkBrown</span><span class="sxs-lookup"><span data-stu-id="a8a87-172">DarkBrown</span></span> |
| <span data-ttu-id="a8a87-173">Preset18</span><span class="sxs-lookup"><span data-stu-id="a8a87-173">Preset18</span></span> | <span data-ttu-id="a8a87-174">DarkYellow</span><span class="sxs-lookup"><span data-stu-id="a8a87-174">DarkYellow</span></span> |
| <span data-ttu-id="a8a87-175">Preset19</span><span class="sxs-lookup"><span data-stu-id="a8a87-175">Preset19</span></span> | <span data-ttu-id="a8a87-176">DarkGreen</span><span class="sxs-lookup"><span data-stu-id="a8a87-176">DarkGreen</span></span> |
| <span data-ttu-id="a8a87-177">Preset20</span><span class="sxs-lookup"><span data-stu-id="a8a87-177">Preset20</span></span> | <span data-ttu-id="a8a87-178">DarkTeal</span><span class="sxs-lookup"><span data-stu-id="a8a87-178">DarkTeal</span></span> |
| <span data-ttu-id="a8a87-179">Preset21</span><span class="sxs-lookup"><span data-stu-id="a8a87-179">Preset21</span></span> | <span data-ttu-id="a8a87-180">DarkOlive</span><span class="sxs-lookup"><span data-stu-id="a8a87-180">DarkOlive</span></span> |
| <span data-ttu-id="a8a87-181">Preset22</span><span class="sxs-lookup"><span data-stu-id="a8a87-181">Preset22</span></span> | <span data-ttu-id="a8a87-182">DarkBlue</span><span class="sxs-lookup"><span data-stu-id="a8a87-182">DarkBlue</span></span> |
| <span data-ttu-id="a8a87-183">Preset23</span><span class="sxs-lookup"><span data-stu-id="a8a87-183">Preset23</span></span> | <span data-ttu-id="a8a87-184">DarkPurple</span><span class="sxs-lookup"><span data-stu-id="a8a87-184">DarkPurple</span></span> |
| <span data-ttu-id="a8a87-185">Preset24</span><span class="sxs-lookup"><span data-stu-id="a8a87-185">Preset24</span></span> | <span data-ttu-id="a8a87-186">DarkCranberry</span><span class="sxs-lookup"><span data-stu-id="a8a87-186">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a8a87-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a8a87-187">JSON representation</span></span>
<span data-ttu-id="a8a87-188">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a8a87-188">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="a8a87-189">メソッド</span><span class="sxs-lookup"><span data-stu-id="a8a87-189">Methods</span></span>
| <span data-ttu-id="a8a87-190">メソッド</span><span class="sxs-lookup"><span data-stu-id="a8a87-190">Method</span></span>           | <span data-ttu-id="a8a87-191">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a8a87-191">Return Type</span></span>    |<span data-ttu-id="a8a87-192">説明</span><span class="sxs-lookup"><span data-stu-id="a8a87-192">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8a87-193">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="a8a87-193">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="a8a87-194">[outlookCategory](../resources/outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a8a87-194">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="a8a87-195">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="a8a87-195">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="a8a87-196">カテゴリの取得</span><span class="sxs-lookup"><span data-stu-id="a8a87-196">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="a8a87-197">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a8a87-197">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="a8a87-198">指定した **outlookCategory** オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="a8a87-198">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="a8a87-199">作成</span><span class="sxs-lookup"><span data-stu-id="a8a87-199">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="a8a87-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a8a87-200">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="a8a87-201">ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a8a87-201">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="a8a87-202">更新</span><span class="sxs-lookup"><span data-stu-id="a8a87-202">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="a8a87-203">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a8a87-203">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="a8a87-204">指定した **outlookCategory** オブジェクトの書き込み可能な **color** プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a8a87-204">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="a8a87-205">削除</span><span class="sxs-lookup"><span data-stu-id="a8a87-205">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="a8a87-206">None</span><span class="sxs-lookup"><span data-stu-id="a8a87-206">None</span></span> |<span data-ttu-id="a8a87-207">指定した **outlookCategory** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a8a87-207">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/beta/resources/outlookcategory.md:
      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ],
  "tocPath": ""
}-->
 