---
title: office365GroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b467f73ed2a4a5e48cb1243c5b1326591bcd707
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581451"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="dc782-103">office365GroupsActivityDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc782-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="dc782-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc782-104">Properties</span></span>

| <span data-ttu-id="dc782-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc782-105">Property</span></span>                          | <span data-ttu-id="dc782-106">型</span><span class="sxs-lookup"><span data-stu-id="dc782-106">Type</span></span>    | <span data-ttu-id="dc782-107">説明</span><span class="sxs-lookup"><span data-stu-id="dc782-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="dc782-108">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="dc782-108">reportRefreshDate</span></span>                 | <span data-ttu-id="dc782-109">Date</span><span class="sxs-lookup"><span data-stu-id="dc782-109">Date</span></span>    | <span data-ttu-id="dc782-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="dc782-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="dc782-111">groupdisplayname</span><span class="sxs-lookup"><span data-stu-id="dc782-111">groupDisplayName</span></span>                  | <span data-ttu-id="dc782-112">String</span><span class="sxs-lookup"><span data-stu-id="dc782-112">String</span></span>  | <span data-ttu-id="dc782-113">グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="dc782-113">The display name of the group.</span></span>           |
| <span data-ttu-id="dc782-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="dc782-114">isDeleted</span></span>                         | <span data-ttu-id="dc782-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc782-115">Boolean</span></span> | <span data-ttu-id="dc782-116">このユーザーが削除されているか、または削除されているか。</span><span class="sxs-lookup"><span data-stu-id="dc782-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="dc782-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dc782-117">ownerPrincipalName</span></span>                | <span data-ttu-id="dc782-118">String</span><span class="sxs-lookup"><span data-stu-id="dc782-118">String</span></span>  | <span data-ttu-id="dc782-119">グループ所有者のプリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="dc782-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="dc782-120">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="dc782-120">lastActivityDate</span></span>                  | <span data-ttu-id="dc782-121">Date</span><span class="sxs-lookup"><span data-stu-id="dc782-121">Date</span></span>    | <span data-ttu-id="dc782-122">次のシナリオの最後のアクティビティの日付: グループメールが受信した電子メール。SharePoint ドキュメントライブラリでユーザーが表示、編集、共有、または同期されたファイル。ユーザーが SharePoint ページを表示した。Yammer グループ内のユーザー投稿、閲覧、またはいいねのメッセージ。</span><span class="sxs-lookup"><span data-stu-id="dc782-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="dc782-123">groupType</span><span class="sxs-lookup"><span data-stu-id="dc782-123">groupType</span></span>                         | <span data-ttu-id="dc782-124">String</span><span class="sxs-lookup"><span data-stu-id="dc782-124">String</span></span>  | <span data-ttu-id="dc782-125">グループの種類。</span><span class="sxs-lookup"><span data-stu-id="dc782-125">The group type.</span></span> <span data-ttu-id="dc782-126">使用可能な値は、 **Public**または**Private**です。</span><span class="sxs-lookup"><span data-stu-id="dc782-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="dc782-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="dc782-127">memberCount</span></span>                       | <span data-ttu-id="dc782-128">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-128">Int64</span></span>   | <span data-ttu-id="dc782-129">グループメンバー数。</span><span class="sxs-lookup"><span data-stu-id="dc782-129">The group member count.</span></span>                  |
| <span data-ttu-id="dc782-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="dc782-130">externalMemberCount</span></span>               | <span data-ttu-id="dc782-131">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-131">Int64</span></span>   | <span data-ttu-id="dc782-132">グループの外部メンバー数。</span><span class="sxs-lookup"><span data-stu-id="dc782-132">The group external member count.</span></span>         |
| <span data-ttu-id="dc782-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="dc782-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="dc782-134">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-134">Int64</span></span>   | <span data-ttu-id="dc782-135">グループメールボックスが受信したメールの数。</span><span class="sxs-lookup"><span data-stu-id="dc782-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="dc782-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="dc782-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="dc782-137">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-137">Int64</span></span>   | <span data-ttu-id="dc782-138">SharePoint グループサイト内のアクティブなファイルの数。</span><span class="sxs-lookup"><span data-stu-id="dc782-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="dc782-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="dc782-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="dc782-140">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-140">Int64</span></span>   | <span data-ttu-id="dc782-141">Yammer グループに投稿されたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="dc782-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="dc782-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="dc782-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="dc782-143">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-143">Int64</span></span>   | <span data-ttu-id="dc782-144">Yammer グループで読み取られたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="dc782-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="dc782-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="dc782-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="dc782-146">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-146">Int64</span></span>   | <span data-ttu-id="dc782-147">Yammer グループに賛同されたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="dc782-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="dc782-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="dc782-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="dc782-149">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-149">Int64</span></span>   | <span data-ttu-id="dc782-150">グループメールボックス内のアイテムの数。</span><span class="sxs-lookup"><span data-stu-id="dc782-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="dc782-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="dc782-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="dc782-152">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-152">Int64</span></span>   | <span data-ttu-id="dc782-153">グループメールボックスで使用されている記憶域。</span><span class="sxs-lookup"><span data-stu-id="dc782-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="dc782-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="dc782-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="dc782-155">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-155">Int64</span></span>   | <span data-ttu-id="dc782-156">SharePoint グループサイト内のファイルの合計数。</span><span class="sxs-lookup"><span data-stu-id="dc782-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="dc782-157">sharepointsitestorageused inbytes</span><span class="sxs-lookup"><span data-stu-id="dc782-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="dc782-158">Int64</span><span class="sxs-lookup"><span data-stu-id="dc782-158">Int64</span></span>   | <span data-ttu-id="dc782-159">SharePoint グループサイトで使用される記憶域。</span><span class="sxs-lookup"><span data-stu-id="dc782-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="dc782-160">reportperiod</span><span class="sxs-lookup"><span data-stu-id="dc782-160">reportPeriod</span></span>                      | <span data-ttu-id="dc782-161">String</span><span class="sxs-lookup"><span data-stu-id="dc782-161">String</span></span>  | <span data-ttu-id="dc782-162">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc782-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="dc782-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc782-163">JSON representation</span></span>

<span data-ttu-id="dc782-164">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc782-164">The following is a JSON representation of the resource.</span></span>

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
