---
title: office365GroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b467f73ed2a4a5e48cb1243c5b1326591bcd707
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575119"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="2ad5d-103">office365GroupsActivityDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ad5d-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2ad5d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ad5d-104">Properties</span></span>

| <span data-ttu-id="2ad5d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ad5d-105">Property</span></span>                          | <span data-ttu-id="2ad5d-106">型</span><span class="sxs-lookup"><span data-stu-id="2ad5d-106">Type</span></span>    | <span data-ttu-id="2ad5d-107">説明</span><span class="sxs-lookup"><span data-stu-id="2ad5d-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="2ad5d-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2ad5d-108">reportRefreshDate</span></span>                 | <span data-ttu-id="2ad5d-109">日付</span><span class="sxs-lookup"><span data-stu-id="2ad5d-109">Date</span></span>    | <span data-ttu-id="2ad5d-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="2ad5d-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ad5d-111">groupDisplayName</span></span>                  | <span data-ttu-id="2ad5d-112">String</span><span class="sxs-lookup"><span data-stu-id="2ad5d-112">String</span></span>  | <span data-ttu-id="2ad5d-113">グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-113">The display name of the group.</span></span>           |
| <span data-ttu-id="2ad5d-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="2ad5d-114">isDeleted</span></span>                         | <span data-ttu-id="2ad5d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad5d-115">Boolean</span></span> | <span data-ttu-id="2ad5d-116">このユーザーが削除されたか、またはソフトをされてかどうかを削除します。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="2ad5d-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2ad5d-117">ownerPrincipalName</span></span>                | <span data-ttu-id="2ad5d-118">String</span><span class="sxs-lookup"><span data-stu-id="2ad5d-118">String</span></span>  | <span data-ttu-id="2ad5d-119">グループの所有者のプリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="2ad5d-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="2ad5d-120">lastActivityDate</span></span>                  | <span data-ttu-id="2ad5d-121">日付</span><span class="sxs-lookup"><span data-stu-id="2ad5d-121">Date</span></span>    | <span data-ttu-id="2ad5d-122">次のシナリオの最後のアクティビティの日付: グループのメールボックスに受信した電子メールです。ユーザーを表示、編集、共有、または SharePoint ドキュメント ライブラリ内のファイルの同期ユーザーが SharePoint ページを表示ユーザーは、投稿、読み取り、または、Yammer グループ内のメッセージを気に入られました。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="2ad5d-123">groupType</span><span class="sxs-lookup"><span data-stu-id="2ad5d-123">groupType</span></span>                         | <span data-ttu-id="2ad5d-124">String</span><span class="sxs-lookup"><span data-stu-id="2ad5d-124">String</span></span>  | <span data-ttu-id="2ad5d-125">グループの種類。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-125">The group type.</span></span> <span data-ttu-id="2ad5d-126">使用可能な値:**パブリック**または**プライベート**です。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="2ad5d-127">membercount プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ad5d-127">memberCount</span></span>                       | <span data-ttu-id="2ad5d-128">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-128">Int64</span></span>   | <span data-ttu-id="2ad5d-129">グループ メンバーの数です。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-129">The group member count.</span></span>                  |
| <span data-ttu-id="2ad5d-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="2ad5d-130">externalMemberCount</span></span>               | <span data-ttu-id="2ad5d-131">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-131">Int64</span></span>   | <span data-ttu-id="2ad5d-132">グループ外部のメンバーの数です。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-132">The group external member count.</span></span>         |
| <span data-ttu-id="2ad5d-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="2ad5d-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="2ad5d-134">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-134">Int64</span></span>   | <span data-ttu-id="2ad5d-135">グループのメールボックスで受信した電子メールの数。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="2ad5d-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="2ad5d-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="2ad5d-137">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-137">Int64</span></span>   | <span data-ttu-id="2ad5d-138">SharePoint グループのサイト内のアクティブなファイルの数です。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="2ad5d-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="2ad5d-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="2ad5d-140">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-140">Int64</span></span>   | <span data-ttu-id="2ad5d-141">Yammer のグループに投稿されたメッセージの数です。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="2ad5d-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="2ad5d-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="2ad5d-143">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-143">Int64</span></span>   | <span data-ttu-id="2ad5d-144">Yammer グループでメッセージの数を読み取る。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="2ad5d-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="2ad5d-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="2ad5d-146">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-146">Int64</span></span>   | <span data-ttu-id="2ad5d-147">Yammer グループに賛同のメッセージの数です。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="2ad5d-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="2ad5d-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="2ad5d-149">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-149">Int64</span></span>   | <span data-ttu-id="2ad5d-150">グループ メールボックス内のアイテムの数です。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="2ad5d-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="2ad5d-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="2ad5d-152">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-152">Int64</span></span>   | <span data-ttu-id="2ad5d-153">・ ストレージ ・ グループのメールボックスのために使用します。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="2ad5d-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="2ad5d-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="2ad5d-155">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-155">Int64</span></span>   | <span data-ttu-id="2ad5d-156">SharePoint グループのサイト内のファイルの合計数です。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="2ad5d-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="2ad5d-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="2ad5d-158">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad5d-158">Int64</span></span>   | <span data-ttu-id="2ad5d-159">・ ストレージ ・ グループを SharePoint サイトで使用されます。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="2ad5d-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2ad5d-160">reportPeriod</span></span>                      | <span data-ttu-id="2ad5d-161">String</span><span class="sxs-lookup"><span data-stu-id="2ad5d-161">String</span></span>  | <span data-ttu-id="2ad5d-162">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2ad5d-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ad5d-163">JSON representation</span></span>

<span data-ttu-id="2ad5d-164">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```
