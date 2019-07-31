---
title: outlookUser リソースの種類
description: ユーザーが利用できる Outlook サービスを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2c23cccabcea33b8cdaacba6ae9abede456c5c99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009266"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="cc53b-103">outlookUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc53b-103">outlookUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc53b-104">ユーザーが利用できる Outlook サービスを表します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="cc53b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc53b-105">Methods</span></span>

| <span data-ttu-id="cc53b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc53b-106">Method</span></span>           | <span data-ttu-id="cc53b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cc53b-107">Return Type</span></span>    |<span data-ttu-id="cc53b-108">説明</span><span class="sxs-lookup"><span data-stu-id="cc53b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc53b-109">カテゴリの作成</span><span class="sxs-lookup"><span data-stu-id="cc53b-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="cc53b-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="cc53b-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="cc53b-111">ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="cc53b-112">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="cc53b-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="cc53b-113">[outlookCategory](outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cc53b-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="cc53b-114">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="cc53b-115">OutlookTaskFolder の作成</span><span class="sxs-lookup"><span data-stu-id="cc53b-115">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="cc53b-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="cc53b-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="cc53b-117">ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) にタスクフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-117">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="cc53b-118">TaskFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cc53b-118">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="cc53b-119">[Outlooktaskfolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc53b-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="cc53b-120">ユーザーのメールボックス内のすべての Outlook タスクフォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-120">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="cc53b-121">OutlookTaskGroup の作成</span><span class="sxs-lookup"><span data-stu-id="cc53b-121">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="cc53b-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="cc53b-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="cc53b-123">ユーザーのメールボックスに Outlook のタスクグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-123">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="cc53b-124">TaskGroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cc53b-124">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="cc53b-125">[Outlooktaskgroup](outlooktaskgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc53b-125">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="cc53b-126">ユーザーのメールボックス内のすべての Outlook タスクグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-126">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="cc53b-127">OutlookTask の作成</span><span class="sxs-lookup"><span data-stu-id="cc53b-127">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="cc53b-128">outlookTask</span><span class="sxs-lookup"><span data-stu-id="cc53b-128">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="cc53b-129">ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) および既定のタスクフォルダー`Tasks`() に Outlook のタスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-129">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="cc53b-130">List tasks</span><span class="sxs-lookup"><span data-stu-id="cc53b-130">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="cc53b-131">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cc53b-131">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="cc53b-132">ユーザーのメールボックス内のすべての Outlook タスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-132">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="cc53b-133">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="cc53b-133">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="cc53b-134">[localeInfo](localeinfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cc53b-134">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="cc53b-135">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-135">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="cc53b-136">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="cc53b-136">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="cc53b-137">[timeZoneInformation](timezoneinformation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cc53b-137">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="cc53b-138">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="cc53b-138">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="cc53b-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc53b-139">Properties</span></span>
<span data-ttu-id="cc53b-140">なし</span><span class="sxs-lookup"><span data-stu-id="cc53b-140">None</span></span>

## <a name="relationships"></a><span data-ttu-id="cc53b-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc53b-141">Relationships</span></span>
| <span data-ttu-id="cc53b-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc53b-142">Relationship</span></span> | <span data-ttu-id="cc53b-143">型</span><span class="sxs-lookup"><span data-stu-id="cc53b-143">Type</span></span>   |<span data-ttu-id="cc53b-144">説明</span><span class="sxs-lookup"><span data-stu-id="cc53b-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc53b-145">masterCategories</span><span class="sxs-lookup"><span data-stu-id="cc53b-145">masterCategories</span></span>|<span data-ttu-id="cc53b-146">[outlookCategory](../resources/outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cc53b-146">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="cc53b-147">ユーザーに対して定義されているカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="cc53b-147">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="cc53b-148">taskFolders</span><span class="sxs-lookup"><span data-stu-id="cc53b-148">taskFolders</span></span>|<span data-ttu-id="cc53b-149">[Outlooktaskfolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc53b-149">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="cc53b-150">ユーザーの Outlook タスクフォルダー。</span><span class="sxs-lookup"><span data-stu-id="cc53b-150">The user's Outlook task folders.</span></span> <span data-ttu-id="cc53b-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cc53b-151">Read-only.</span></span> <span data-ttu-id="cc53b-152">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cc53b-152">Nullable.</span></span>|
|<span data-ttu-id="cc53b-153">taskGroups</span><span class="sxs-lookup"><span data-stu-id="cc53b-153">taskGroups</span></span>|<span data-ttu-id="cc53b-154">[Outlooktaskgroup](outlooktaskgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc53b-154">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="cc53b-155">ユーザーの Outlook タスクグループ。</span><span class="sxs-lookup"><span data-stu-id="cc53b-155">The user's Outlook task groups.</span></span> <span data-ttu-id="cc53b-156">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cc53b-156">Read-only.</span></span> <span data-ttu-id="cc53b-157">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cc53b-157">Nullable.</span></span>|
|<span data-ttu-id="cc53b-158">tasks</span><span class="sxs-lookup"><span data-stu-id="cc53b-158">tasks</span></span>|<span data-ttu-id="cc53b-159">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cc53b-159">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="cc53b-160">ユーザーの Outlook タスク。</span><span class="sxs-lookup"><span data-stu-id="cc53b-160">The user's Outlook tasks.</span></span> <span data-ttu-id="cc53b-161">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cc53b-161">Read-only.</span></span> <span data-ttu-id="cc53b-162">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cc53b-162">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc53b-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc53b-163">JSON representation</span></span>

<span data-ttu-id="cc53b-164">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="cc53b-164">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookUser"
}-->
```json
{  
    "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
