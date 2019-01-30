---
title: outlookUser リソースの種類
description: ユーザーが利用できる Outlook サービスを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a649de502728bbc51ac53e072c08d95291d20853
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643546"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="c9731-103">outlookUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9731-103">outlookUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9731-104">ユーザーが利用できる Outlook サービスを表します。</span><span class="sxs-lookup"><span data-stu-id="c9731-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="c9731-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9731-105">Methods</span></span>

| <span data-ttu-id="c9731-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9731-106">Method</span></span>           | <span data-ttu-id="c9731-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c9731-107">Return Type</span></span>    |<span data-ttu-id="c9731-108">説明</span><span class="sxs-lookup"><span data-stu-id="c9731-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9731-109">カテゴリの作成</span><span class="sxs-lookup"><span data-stu-id="c9731-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="c9731-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c9731-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="c9731-111">ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c9731-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="c9731-112">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="c9731-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="c9731-113">[outlookCategory](outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c9731-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="c9731-114">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="c9731-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="c9731-115">OutlookTaskFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="c9731-115">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="c9731-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="c9731-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="c9731-117">既定のタスク グループにタスク フォルダーを作成 (`My Tasks`) ユーザーのメールボックスの。</span><span class="sxs-lookup"><span data-stu-id="c9731-117">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="c9731-118">リスト taskFolders</span><span class="sxs-lookup"><span data-stu-id="c9731-118">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="c9731-119">[outlookTaskFolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c9731-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="c9731-120">ユーザーのメールボックス内のすべての Outlook タスク フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="c9731-120">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="c9731-121">OutlookTaskGroup を作成します。</span><span class="sxs-lookup"><span data-stu-id="c9731-121">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="c9731-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c9731-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="c9731-123">ユーザーのメールボックスに Outlook のタスク グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="c9731-123">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="c9731-124">TaskGroups のリスト</span><span class="sxs-lookup"><span data-stu-id="c9731-124">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="c9731-125">[outlookTaskGroup](outlooktaskgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c9731-125">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="c9731-126">ユーザーのメールボックス内のすべての Outlook のタスク グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="c9731-126">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="c9731-127">OutlookTask を作成します。</span><span class="sxs-lookup"><span data-stu-id="c9731-127">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="c9731-128">outlookTask</span><span class="sxs-lookup"><span data-stu-id="c9731-128">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="c9731-129">デフォルトのタスク グループに Outlook のタスクを作成する (`My Tasks`) と既定の作業フォルダー (`Tasks`) ユーザーのメールボックスにします。</span><span class="sxs-lookup"><span data-stu-id="c9731-129">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="c9731-130">List tasks</span><span class="sxs-lookup"><span data-stu-id="c9731-130">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="c9731-131">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c9731-131">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="c9731-132">ユーザーのメールボックス内のすべての Outlook タスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="c9731-132">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="c9731-133">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="c9731-133">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="c9731-134">[localeInfo](localeinfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c9731-134">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="c9731-135">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="c9731-135">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="c9731-136">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="c9731-136">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="c9731-137">[timeZoneInformation](timezoneinformation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c9731-137">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="c9731-138">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="c9731-138">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="c9731-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9731-139">Properties</span></span>
<span data-ttu-id="c9731-140">なし</span><span class="sxs-lookup"><span data-stu-id="c9731-140">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c9731-141">関係</span><span class="sxs-lookup"><span data-stu-id="c9731-141">Relationships</span></span>
| <span data-ttu-id="c9731-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c9731-142">Relationship</span></span> | <span data-ttu-id="c9731-143">型</span><span class="sxs-lookup"><span data-stu-id="c9731-143">Type</span></span>   |<span data-ttu-id="c9731-144">説明</span><span class="sxs-lookup"><span data-stu-id="c9731-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9731-145">masterCategories</span><span class="sxs-lookup"><span data-stu-id="c9731-145">masterCategories</span></span>|<span data-ttu-id="c9731-146">[outlookCategory](../resources/outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c9731-146">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="c9731-147">ユーザーに対して定義されているカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="c9731-147">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="c9731-148">taskFolders</span><span class="sxs-lookup"><span data-stu-id="c9731-148">taskFolders</span></span>|<span data-ttu-id="c9731-149">[outlookTaskFolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c9731-149">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="c9731-150">ユーザーの Outlook の仕事フォルダー。</span><span class="sxs-lookup"><span data-stu-id="c9731-150">The user's Outlook task folders.</span></span> <span data-ttu-id="c9731-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c9731-151">Read-only.</span></span> <span data-ttu-id="c9731-152">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c9731-152">Nullable.</span></span>|
|<span data-ttu-id="c9731-153">taskGroups</span><span class="sxs-lookup"><span data-stu-id="c9731-153">taskGroups</span></span>|<span data-ttu-id="c9731-154">[outlookTaskGroup](outlooktaskgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c9731-154">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="c9731-155">ユーザーの Outlook のタスク グループ。</span><span class="sxs-lookup"><span data-stu-id="c9731-155">The user's Outlook task groups.</span></span> <span data-ttu-id="c9731-156">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c9731-156">Read-only.</span></span> <span data-ttu-id="c9731-157">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c9731-157">Nullable.</span></span>|
|<span data-ttu-id="c9731-158">tasks</span><span class="sxs-lookup"><span data-stu-id="c9731-158">tasks</span></span>|<span data-ttu-id="c9731-159">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c9731-159">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="c9731-160">ユーザーの Outlook の仕事です。</span><span class="sxs-lookup"><span data-stu-id="c9731-160">The user's Outlook tasks.</span></span> <span data-ttu-id="c9731-161">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c9731-161">Read-only.</span></span> <span data-ttu-id="c9731-162">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c9731-162">Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
