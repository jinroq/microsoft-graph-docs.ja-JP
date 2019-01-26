---
title: outlookUser リソースの種類
description: ユーザーが利用できる Outlook サービスを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f8265f9da285ce0f52e6201ffdb1298893b86753
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574097"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="bd171-103">outlookUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd171-103">outlookUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd171-104">ユーザーが利用できる Outlook サービスを表します。</span><span class="sxs-lookup"><span data-stu-id="bd171-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="bd171-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="bd171-105">Methods</span></span>

| <span data-ttu-id="bd171-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="bd171-106">Method</span></span>           | <span data-ttu-id="bd171-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bd171-107">Return Type</span></span>    |<span data-ttu-id="bd171-108">説明</span><span class="sxs-lookup"><span data-stu-id="bd171-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd171-109">カテゴリの作成</span><span class="sxs-lookup"><span data-stu-id="bd171-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="bd171-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bd171-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="bd171-111">ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bd171-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="bd171-112">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="bd171-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="bd171-113">[outlookCategory](outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd171-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="bd171-114">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="bd171-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="bd171-115">OutlookTaskFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="bd171-115">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="bd171-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="bd171-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="bd171-117">既定のタスク グループにタスク フォルダーを作成 (`My Tasks`) ユーザーのメールボックスの。</span><span class="sxs-lookup"><span data-stu-id="bd171-117">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="bd171-118">リスト taskFolders</span><span class="sxs-lookup"><span data-stu-id="bd171-118">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="bd171-119">[outlookTaskFolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bd171-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="bd171-120">ユーザーのメールボックス内のすべての Outlook タスク フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="bd171-120">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="bd171-121">OutlookTaskGroup を作成します。</span><span class="sxs-lookup"><span data-stu-id="bd171-121">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="bd171-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="bd171-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="bd171-123">ユーザーのメールボックスに Outlook のタスク グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="bd171-123">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="bd171-124">TaskGroups のリスト</span><span class="sxs-lookup"><span data-stu-id="bd171-124">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="bd171-125">[outlookTaskGroup](outlooktaskgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bd171-125">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="bd171-126">ユーザーのメールボックス内のすべての Outlook のタスク グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="bd171-126">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="bd171-127">OutlookTask を作成します。</span><span class="sxs-lookup"><span data-stu-id="bd171-127">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="bd171-128">outlookTask</span><span class="sxs-lookup"><span data-stu-id="bd171-128">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="bd171-129">デフォルトのタスク グループに Outlook のタスクを作成する (`My Tasks`) と既定の作業フォルダー (`Tasks`) ユーザーのメールボックスにします。</span><span class="sxs-lookup"><span data-stu-id="bd171-129">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="bd171-130">List tasks</span><span class="sxs-lookup"><span data-stu-id="bd171-130">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="bd171-131">[outlookTask](outlooktask.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bd171-131">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="bd171-132">ユーザーのメールボックス内のすべての Outlook タスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="bd171-132">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="bd171-133">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="bd171-133">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="bd171-134">[localeInfo](localeinfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd171-134">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="bd171-135">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="bd171-135">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="bd171-136">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="bd171-136">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="bd171-137">[timeZoneInformation](timezoneinformation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd171-137">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="bd171-138">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="bd171-138">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="bd171-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd171-139">Properties</span></span>
<span data-ttu-id="bd171-140">なし</span><span class="sxs-lookup"><span data-stu-id="bd171-140">None</span></span>

## <a name="relationships"></a><span data-ttu-id="bd171-141">関係</span><span class="sxs-lookup"><span data-stu-id="bd171-141">Relationships</span></span>
| <span data-ttu-id="bd171-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bd171-142">Relationship</span></span> | <span data-ttu-id="bd171-143">型</span><span class="sxs-lookup"><span data-stu-id="bd171-143">Type</span></span>   |<span data-ttu-id="bd171-144">説明</span><span class="sxs-lookup"><span data-stu-id="bd171-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd171-145">masterCategories</span><span class="sxs-lookup"><span data-stu-id="bd171-145">masterCategories</span></span>|<span data-ttu-id="bd171-146">[outlookCategory](../resources/outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bd171-146">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="bd171-147">ユーザーに対して定義されているカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="bd171-147">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="bd171-148">taskFolders</span><span class="sxs-lookup"><span data-stu-id="bd171-148">taskFolders</span></span>|<span data-ttu-id="bd171-149">[outlookTaskFolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bd171-149">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="bd171-150">ユーザーの Outlook の仕事フォルダー。</span><span class="sxs-lookup"><span data-stu-id="bd171-150">The user's Outlook task folders.</span></span> <span data-ttu-id="bd171-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bd171-151">Read-only.</span></span> <span data-ttu-id="bd171-152">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bd171-152">Nullable.</span></span>|
|<span data-ttu-id="bd171-153">taskGroups</span><span class="sxs-lookup"><span data-stu-id="bd171-153">taskGroups</span></span>|<span data-ttu-id="bd171-154">[outlookTaskGroup](outlooktaskgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bd171-154">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="bd171-155">ユーザーの Outlook のタスク グループ。</span><span class="sxs-lookup"><span data-stu-id="bd171-155">The user's Outlook task groups.</span></span> <span data-ttu-id="bd171-156">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bd171-156">Read-only.</span></span> <span data-ttu-id="bd171-157">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bd171-157">Nullable.</span></span>|
|<span data-ttu-id="bd171-158">tasks</span><span class="sxs-lookup"><span data-stu-id="bd171-158">tasks</span></span>|<span data-ttu-id="bd171-159">[outlookTask](outlooktask.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bd171-159">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="bd171-160">ユーザーの Outlook の仕事です。</span><span class="sxs-lookup"><span data-stu-id="bd171-160">The user's Outlook tasks.</span></span> <span data-ttu-id="bd171-161">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bd171-161">Read-only.</span></span> <span data-ttu-id="bd171-162">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bd171-162">Nullable.</span></span>|


<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.outlookUser"
}-->
```json
{
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
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
