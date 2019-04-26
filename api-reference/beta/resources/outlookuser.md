---
title: outlookUser リソースの種類
description: ユーザーが利用できる Outlook サービスを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a649de502728bbc51ac53e072c08d95291d20853
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568597"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="509f8-103">outlookUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="509f8-103">outlookUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="509f8-104">ユーザーが利用できる Outlook サービスを表します。</span><span class="sxs-lookup"><span data-stu-id="509f8-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="509f8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="509f8-105">Methods</span></span>

| <span data-ttu-id="509f8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="509f8-106">Method</span></span>           | <span data-ttu-id="509f8-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="509f8-107">Return Type</span></span>    |<span data-ttu-id="509f8-108">説明</span><span class="sxs-lookup"><span data-stu-id="509f8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="509f8-109">カテゴリの作成</span><span class="sxs-lookup"><span data-stu-id="509f8-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="509f8-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="509f8-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="509f8-111">ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="509f8-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="509f8-112">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="509f8-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="509f8-113">[outlookCategory](outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="509f8-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="509f8-114">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="509f8-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="509f8-115">outlooktaskfolder の作成</span><span class="sxs-lookup"><span data-stu-id="509f8-115">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="509f8-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="509f8-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="509f8-117">ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) にタスクフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="509f8-117">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="509f8-118">taskfolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="509f8-118">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="509f8-119">[outlooktaskfolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="509f8-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="509f8-120">ユーザーのメールボックス内のすべての Outlook タスクフォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="509f8-120">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="509f8-121">outlooktaskgroup の作成</span><span class="sxs-lookup"><span data-stu-id="509f8-121">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="509f8-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="509f8-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="509f8-123">ユーザーのメールボックスに Outlook のタスクグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="509f8-123">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="509f8-124">taskgroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="509f8-124">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="509f8-125">[outlooktaskgroup](outlooktaskgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="509f8-125">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="509f8-126">ユーザーのメールボックス内のすべての Outlook タスクグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="509f8-126">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="509f8-127">outlooktask の作成</span><span class="sxs-lookup"><span data-stu-id="509f8-127">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="509f8-128">outlookTask</span><span class="sxs-lookup"><span data-stu-id="509f8-128">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="509f8-129">ユーザーのメールボックスの既定のタスクグループ (`My Tasks`) および既定のタスクフォルダー`Tasks`() に Outlook のタスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="509f8-129">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="509f8-130">タスクを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="509f8-130">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="509f8-131">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="509f8-131">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="509f8-132">ユーザーのメールボックス内のすべての Outlook タスクを取得します。</span><span class="sxs-lookup"><span data-stu-id="509f8-132">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="509f8-133">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="509f8-133">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="509f8-134">[localeInfo](localeinfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="509f8-134">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="509f8-135">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="509f8-135">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="509f8-136">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="509f8-136">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="509f8-137">[timeZoneInformation](timezoneinformation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="509f8-137">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="509f8-138">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="509f8-138">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="509f8-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="509f8-139">Properties</span></span>
<span data-ttu-id="509f8-140">なし</span><span class="sxs-lookup"><span data-stu-id="509f8-140">None</span></span>

## <a name="relationships"></a><span data-ttu-id="509f8-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="509f8-141">Relationships</span></span>
| <span data-ttu-id="509f8-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="509f8-142">Relationship</span></span> | <span data-ttu-id="509f8-143">型</span><span class="sxs-lookup"><span data-stu-id="509f8-143">Type</span></span>   |<span data-ttu-id="509f8-144">説明</span><span class="sxs-lookup"><span data-stu-id="509f8-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="509f8-145">masterCategories</span><span class="sxs-lookup"><span data-stu-id="509f8-145">masterCategories</span></span>|<span data-ttu-id="509f8-146">[outlookCategory](../resources/outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="509f8-146">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="509f8-147">ユーザーに対して定義されているカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="509f8-147">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="509f8-148">taskfolders</span><span class="sxs-lookup"><span data-stu-id="509f8-148">taskFolders</span></span>|<span data-ttu-id="509f8-149">[outlooktaskfolder](outlooktaskfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="509f8-149">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="509f8-150">ユーザーの Outlook タスクフォルダー。</span><span class="sxs-lookup"><span data-stu-id="509f8-150">The user's Outlook task folders.</span></span> <span data-ttu-id="509f8-151">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="509f8-151">Read-only.</span></span> <span data-ttu-id="509f8-152">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="509f8-152">Nullable.</span></span>|
|<span data-ttu-id="509f8-153">taskGroups</span><span class="sxs-lookup"><span data-stu-id="509f8-153">taskGroups</span></span>|<span data-ttu-id="509f8-154">[outlooktaskgroup](outlooktaskgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="509f8-154">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="509f8-155">ユーザーの Outlook タスクグループ。</span><span class="sxs-lookup"><span data-stu-id="509f8-155">The user's Outlook task groups.</span></span> <span data-ttu-id="509f8-156">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="509f8-156">Read-only.</span></span> <span data-ttu-id="509f8-157">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="509f8-157">Nullable.</span></span>|
|<span data-ttu-id="509f8-158">tasks</span><span class="sxs-lookup"><span data-stu-id="509f8-158">tasks</span></span>|<span data-ttu-id="509f8-159">[outlookTask](outlooktask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="509f8-159">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="509f8-160">ユーザーの Outlook タスク。</span><span class="sxs-lookup"><span data-stu-id="509f8-160">The user's Outlook tasks.</span></span> <span data-ttu-id="509f8-161">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="509f8-161">Read-only.</span></span> <span data-ttu-id="509f8-162">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="509f8-162">Nullable.</span></span>|

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
