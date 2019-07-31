---
title: outlookCategory リソースの種類
description: ユーザーが Outlook アイテム (メッセージやイベントなど) をグループ化するために使用できるカテゴリを表します。 Outlook では、ユーザーがマスターリストでカテゴリを定義し、1つ以上のユーザー定義を適用できます。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b480f676c39e64c87048765b4ccc145a077036d9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009252"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="c74d4-104">outlookCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c74d4-104">outlookCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c74d4-105">ユーザーが Outlook アイテム (メッセージやイベントなど) をグループ化するために使用できるカテゴリを表します。</span><span class="sxs-lookup"><span data-stu-id="c74d4-105">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="c74d4-106">Outlook では、ユーザーがマスターリストでカテゴリを定義し、1つまたは複数のユーザー定義の分類項目をアイテムに適用することができます。</span><span class="sxs-lookup"><span data-stu-id="c74d4-106">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="c74d4-107">カテゴリを[作成](../api/outlookuser-post-mastercategories.md)してユーザーのマスター カテゴリ リストに定義するには、REST API を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="c74d4-107">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="c74d4-108">また、[このマスター カテゴリ リストの取得](../api/outlookuser-list-mastercategories.md)、[特定のカテゴリの取得](../api/outlookcategory-get.md)、カテゴリに関連付けられている色の[更新](../api/outlookcategory-update.md)、カテゴリの[削除](../api/outlookcategory-delete.md)などの操作を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="c74d4-108">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="c74d4-109">カテゴリをアイテムに適用するには、適用対象とするアイテムの **categories** コレクションに、カテゴリの **displayName** プロパティを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="c74d4-109">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="c74d4-110">カテゴリに割り当てることができるリソースには、 [contact](contact.md)、 [event](event.md)、 [message](message.md)、 [outlooktask](outlooktask.md)、 [post](post.md)があります。</span><span class="sxs-lookup"><span data-stu-id="c74d4-110">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="c74d4-111">各カテゴリを特徴付けるプロパティには、**displayName** と **color** の 2 つがあります。</span><span class="sxs-lookup"><span data-stu-id="c74d4-111">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="c74d4-112">**displayName** の値は、ユーザーのマスター リスト内で一意でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="c74d4-112">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="c74d4-113">一方、**color** には一意の値を設定する必要はありません。マスター リストに含まれる複数のカテゴリに、同じ色をマッピングすることができます。</span><span class="sxs-lookup"><span data-stu-id="c74d4-113">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="c74d4-114">ユーザーのマスター リスト内のカテゴリには、最大 25 種類の色をマッピングできます。</span><span class="sxs-lookup"><span data-stu-id="c74d4-114">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="c74d4-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c74d4-115">Properties</span></span>
| <span data-ttu-id="c74d4-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c74d4-116">Property</span></span>     | <span data-ttu-id="c74d4-117">型</span><span class="sxs-lookup"><span data-stu-id="c74d4-117">Type</span></span>   |<span data-ttu-id="c74d4-118">説明</span><span class="sxs-lookup"><span data-stu-id="c74d4-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c74d4-119">displayName</span><span class="sxs-lookup"><span data-stu-id="c74d4-119">displayName</span></span>|<span data-ttu-id="c74d4-120">文字列</span><span class="sxs-lookup"><span data-stu-id="c74d4-120">String</span></span>|<span data-ttu-id="c74d4-121">ユーザーのメールボックス内でカテゴリを識別する一意の名前。</span><span class="sxs-lookup"><span data-stu-id="c74d4-121">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="c74d4-122">カテゴリが作成された後に、この名前を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="c74d4-122">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="c74d4-123">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c74d4-123">Read-only.</span></span>|
|<span data-ttu-id="c74d4-124">color</span><span class="sxs-lookup"><span data-stu-id="c74d4-124">color</span></span>|<span data-ttu-id="c74d4-125">String</span><span class="sxs-lookup"><span data-stu-id="c74d4-125">String</span></span>|<span data-ttu-id="c74d4-126">カテゴリを特徴付ける、あらかじめ設定された色の定数。定数は、事前定義された 25 種類の色のいずれか 1 つにマッピングされています。</span><span class="sxs-lookup"><span data-stu-id="c74d4-126">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="c74d4-127">次の注を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c74d4-127">See the note below.</span></span> |

> <span data-ttu-id="c74d4-128">**注:** **color** に使用できる値は、あらかじめ設定されている `None`、`preset0`、`preset1` などの定数です。</span><span class="sxs-lookup"><span data-stu-id="c74d4-128">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="c74d4-129">設定済みの定数は、それぞれ 1 つの色にマッピングされています。ただし、実際の色は、カテゴリを表示する Outloook クライアントに依存します。</span><span class="sxs-lookup"><span data-stu-id="c74d4-129">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="c74d4-130">次の表に、設定済みの各定数に Outlook (デスクトップ クライアント) でマッピングされている色を記載します。</span><span class="sxs-lookup"><span data-stu-id="c74d4-130">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="c74d4-131">設定済みの定数</span><span class="sxs-lookup"><span data-stu-id="c74d4-131">Pre-set constant</span></span>  | <span data-ttu-id="c74d4-132">Outlook でマッピングされている色</span><span class="sxs-lookup"><span data-stu-id="c74d4-132">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c74d4-133">None</span><span class="sxs-lookup"><span data-stu-id="c74d4-133">None</span></span> | <span data-ttu-id="c74d4-134">マッピングされている色なし</span><span class="sxs-lookup"><span data-stu-id="c74d4-134">No color mapped</span></span> |
| <span data-ttu-id="c74d4-135">Preset0</span><span class="sxs-lookup"><span data-stu-id="c74d4-135">Preset0</span></span> | <span data-ttu-id="c74d4-136">赤</span><span class="sxs-lookup"><span data-stu-id="c74d4-136">Red</span></span> |
| <span data-ttu-id="c74d4-137">Preset1</span><span class="sxs-lookup"><span data-stu-id="c74d4-137">Preset1</span></span> | <span data-ttu-id="c74d4-138">オレンジ</span><span class="sxs-lookup"><span data-stu-id="c74d4-138">Orange</span></span> |
| <span data-ttu-id="c74d4-139">Preset2</span><span class="sxs-lookup"><span data-stu-id="c74d4-139">Preset2</span></span> | <span data-ttu-id="c74d4-140">茶</span><span class="sxs-lookup"><span data-stu-id="c74d4-140">Brown</span></span> |
| <span data-ttu-id="c74d4-141">Preset3</span><span class="sxs-lookup"><span data-stu-id="c74d4-141">Preset3</span></span> | <span data-ttu-id="c74d4-142">黄</span><span class="sxs-lookup"><span data-stu-id="c74d4-142">Yellow</span></span> |
| <span data-ttu-id="c74d4-143">Preset4</span><span class="sxs-lookup"><span data-stu-id="c74d4-143">Preset4</span></span> | <span data-ttu-id="c74d4-144">緑</span><span class="sxs-lookup"><span data-stu-id="c74d4-144">Green</span></span> |
| <span data-ttu-id="c74d4-145">Preset5</span><span class="sxs-lookup"><span data-stu-id="c74d4-145">Preset5</span></span> | <span data-ttu-id="c74d4-146">青緑</span><span class="sxs-lookup"><span data-stu-id="c74d4-146">Teal</span></span> |
| <span data-ttu-id="c74d4-147">Preset6</span><span class="sxs-lookup"><span data-stu-id="c74d4-147">Preset6</span></span> | <span data-ttu-id="c74d4-148">オリーブ</span><span class="sxs-lookup"><span data-stu-id="c74d4-148">Olive</span></span> |
| <span data-ttu-id="c74d4-149">Preset7</span><span class="sxs-lookup"><span data-stu-id="c74d4-149">Preset7</span></span> | <span data-ttu-id="c74d4-150">青</span><span class="sxs-lookup"><span data-stu-id="c74d4-150">Blue</span></span> |
| <span data-ttu-id="c74d4-151">Preset8</span><span class="sxs-lookup"><span data-stu-id="c74d4-151">Preset8</span></span> | <span data-ttu-id="c74d4-152">紫</span><span class="sxs-lookup"><span data-stu-id="c74d4-152">Purple</span></span> |
| <span data-ttu-id="c74d4-153">Preset9</span><span class="sxs-lookup"><span data-stu-id="c74d4-153">Preset9</span></span> | <span data-ttu-id="c74d4-154">深紅</span><span class="sxs-lookup"><span data-stu-id="c74d4-154">Cranberry</span></span> |
| <span data-ttu-id="c74d4-155">Preset10</span><span class="sxs-lookup"><span data-stu-id="c74d4-155">Preset10</span></span> | <span data-ttu-id="c74d4-156">鋼色</span><span class="sxs-lookup"><span data-stu-id="c74d4-156">Steel</span></span> |
| <span data-ttu-id="c74d4-157">Preset11</span><span class="sxs-lookup"><span data-stu-id="c74d4-157">Preset11</span></span> | <span data-ttu-id="c74d4-158">DarkSteel</span><span class="sxs-lookup"><span data-stu-id="c74d4-158">DarkSteel</span></span> |
| <span data-ttu-id="c74d4-159">Preset12</span><span class="sxs-lookup"><span data-stu-id="c74d4-159">Preset12</span></span> | <span data-ttu-id="c74d4-160">灰色</span><span class="sxs-lookup"><span data-stu-id="c74d4-160">Gray</span></span> |
| <span data-ttu-id="c74d4-161">Preset13</span><span class="sxs-lookup"><span data-stu-id="c74d4-161">Preset13</span></span> | <span data-ttu-id="c74d4-162">DarkGray</span><span class="sxs-lookup"><span data-stu-id="c74d4-162">DarkGray</span></span> |
| <span data-ttu-id="c74d4-163">Preset14</span><span class="sxs-lookup"><span data-stu-id="c74d4-163">Preset14</span></span> | <span data-ttu-id="c74d4-164">黒</span><span class="sxs-lookup"><span data-stu-id="c74d4-164">Black</span></span> |
| <span data-ttu-id="c74d4-165">Preset15</span><span class="sxs-lookup"><span data-stu-id="c74d4-165">Preset15</span></span> | <span data-ttu-id="c74d4-166">DarkRed</span><span class="sxs-lookup"><span data-stu-id="c74d4-166">DarkRed</span></span> |
| <span data-ttu-id="c74d4-167">Preset16</span><span class="sxs-lookup"><span data-stu-id="c74d4-167">Preset16</span></span> | <span data-ttu-id="c74d4-168">DarkOrange</span><span class="sxs-lookup"><span data-stu-id="c74d4-168">DarkOrange</span></span> |
| <span data-ttu-id="c74d4-169">Preset17</span><span class="sxs-lookup"><span data-stu-id="c74d4-169">Preset17</span></span> | <span data-ttu-id="c74d4-170">DarkBrown</span><span class="sxs-lookup"><span data-stu-id="c74d4-170">DarkBrown</span></span> |
| <span data-ttu-id="c74d4-171">Preset18</span><span class="sxs-lookup"><span data-stu-id="c74d4-171">Preset18</span></span> | <span data-ttu-id="c74d4-172">DarkYellow</span><span class="sxs-lookup"><span data-stu-id="c74d4-172">DarkYellow</span></span> |
| <span data-ttu-id="c74d4-173">Preset19</span><span class="sxs-lookup"><span data-stu-id="c74d4-173">Preset19</span></span> | <span data-ttu-id="c74d4-174">DarkGreen</span><span class="sxs-lookup"><span data-stu-id="c74d4-174">DarkGreen</span></span> |
| <span data-ttu-id="c74d4-175">Preset20</span><span class="sxs-lookup"><span data-stu-id="c74d4-175">Preset20</span></span> | <span data-ttu-id="c74d4-176">DarkTeal</span><span class="sxs-lookup"><span data-stu-id="c74d4-176">DarkTeal</span></span> |
| <span data-ttu-id="c74d4-177">Preset21</span><span class="sxs-lookup"><span data-stu-id="c74d4-177">Preset21</span></span> | <span data-ttu-id="c74d4-178">DarkOlive</span><span class="sxs-lookup"><span data-stu-id="c74d4-178">DarkOlive</span></span> |
| <span data-ttu-id="c74d4-179">Preset22</span><span class="sxs-lookup"><span data-stu-id="c74d4-179">Preset22</span></span> | <span data-ttu-id="c74d4-180">DarkBlue</span><span class="sxs-lookup"><span data-stu-id="c74d4-180">DarkBlue</span></span> |
| <span data-ttu-id="c74d4-181">Preset23</span><span class="sxs-lookup"><span data-stu-id="c74d4-181">Preset23</span></span> | <span data-ttu-id="c74d4-182">DarkPurple</span><span class="sxs-lookup"><span data-stu-id="c74d4-182">DarkPurple</span></span> |
| <span data-ttu-id="c74d4-183">Preset24</span><span class="sxs-lookup"><span data-stu-id="c74d4-183">Preset24</span></span> | <span data-ttu-id="c74d4-184">DarkCranberry</span><span class="sxs-lookup"><span data-stu-id="c74d4-184">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c74d4-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c74d4-185">JSON representation</span></span>
<span data-ttu-id="c74d4-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c74d4-186">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="c74d4-187">メソッド</span><span class="sxs-lookup"><span data-stu-id="c74d4-187">Methods</span></span>
| <span data-ttu-id="c74d4-188">メソッド</span><span class="sxs-lookup"><span data-stu-id="c74d4-188">Method</span></span>           | <span data-ttu-id="c74d4-189">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c74d4-189">Return Type</span></span>    |<span data-ttu-id="c74d4-190">説明</span><span class="sxs-lookup"><span data-stu-id="c74d4-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c74d4-191">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="c74d4-191">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="c74d4-192">[outlookCategory](../resources/outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c74d4-192">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="c74d4-193">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="c74d4-193">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="c74d4-194">カテゴリの取得</span><span class="sxs-lookup"><span data-stu-id="c74d4-194">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="c74d4-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c74d4-195">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="c74d4-196">指定した **outlookCategory** オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="c74d4-196">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="c74d4-197">作成</span><span class="sxs-lookup"><span data-stu-id="c74d4-197">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="c74d4-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c74d4-198">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="c74d4-199">ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c74d4-199">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="c74d4-200">更新</span><span class="sxs-lookup"><span data-stu-id="c74d4-200">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="c74d4-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c74d4-201">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="c74d4-202">指定した **outlookCategory** オブジェクトの書き込み可能な **color** プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c74d4-202">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="c74d4-203">Delete</span><span class="sxs-lookup"><span data-stu-id="c74d4-203">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="c74d4-204">None</span><span class="sxs-lookup"><span data-stu-id="c74d4-204">None</span></span> |<span data-ttu-id="c74d4-205">指定した **outlookCategory** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="c74d4-205">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/outlookcategory.md:\r\n      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ]
}
-->
 
