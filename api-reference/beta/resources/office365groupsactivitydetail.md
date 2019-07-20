---
title: office365GroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 176e960c7d9ae8dd1bc29600ad7b64e45e2940fa
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805215"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="c4fd1-103">office365GroupsActivityDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4fd1-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c4fd1-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4fd1-104">Properties</span></span>

| <span data-ttu-id="c4fd1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4fd1-105">Property</span></span>                          | <span data-ttu-id="c4fd1-106">型</span><span class="sxs-lookup"><span data-stu-id="c4fd1-106">Type</span></span>    | <span data-ttu-id="c4fd1-107">説明</span><span class="sxs-lookup"><span data-stu-id="c4fd1-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="c4fd1-108">groupId</span><span class="sxs-lookup"><span data-stu-id="c4fd1-108">groupId</span></span>                           | <span data-ttu-id="c4fd1-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c4fd1-109">String</span></span>  | <span data-ttu-id="c4fd1-110">グループ id。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-110">The group id.</span></span>          |
| <span data-ttu-id="c4fd1-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c4fd1-111">reportRefreshDate</span></span>                 | <span data-ttu-id="c4fd1-112">日付</span><span class="sxs-lookup"><span data-stu-id="c4fd1-112">Date</span></span>    | <span data-ttu-id="c4fd1-113">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-113">The latest date of the content.</span></span>          |
| <span data-ttu-id="c4fd1-114">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="c4fd1-114">groupDisplayName</span></span>                  | <span data-ttu-id="c4fd1-115">String</span><span class="sxs-lookup"><span data-stu-id="c4fd1-115">String</span></span>  | <span data-ttu-id="c4fd1-116">グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-116">The display name of the group.</span></span>           |
| <span data-ttu-id="c4fd1-117">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c4fd1-117">isDeleted</span></span>                         | <span data-ttu-id="c4fd1-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4fd1-118">Boolean</span></span> | <span data-ttu-id="c4fd1-119">このユーザーが削除されているか、または削除されているか。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-119">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="c4fd1-120">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c4fd1-120">ownerPrincipalName</span></span>                | <span data-ttu-id="c4fd1-121">String</span><span class="sxs-lookup"><span data-stu-id="c4fd1-121">String</span></span>  | <span data-ttu-id="c4fd1-122">グループ所有者のプリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-122">The group owner principal name.</span></span>          |
| <span data-ttu-id="c4fd1-123">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c4fd1-123">lastActivityDate</span></span>                  | <span data-ttu-id="c4fd1-124">日付</span><span class="sxs-lookup"><span data-stu-id="c4fd1-124">Date</span></span>    | <span data-ttu-id="c4fd1-125">次のシナリオの最後のアクティビティの日付: グループメールが受信した電子メール。SharePoint ドキュメントライブラリでユーザーが表示、編集、共有、または同期されたファイル。ユーザーが SharePoint ページを表示した。Yammer グループ内のユーザー投稿、閲覧、またはいいねのメッセージ。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-125">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="c4fd1-126">groupType</span><span class="sxs-lookup"><span data-stu-id="c4fd1-126">groupType</span></span>                         | <span data-ttu-id="c4fd1-127">String</span><span class="sxs-lookup"><span data-stu-id="c4fd1-127">String</span></span>  | <span data-ttu-id="c4fd1-128">グループの種類。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-128">The group type.</span></span> <span data-ttu-id="c4fd1-129">使用可能な値は、 **Public**または**Private**です。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-129">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="c4fd1-130">memberCount</span><span class="sxs-lookup"><span data-stu-id="c4fd1-130">memberCount</span></span>                       | <span data-ttu-id="c4fd1-131">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-131">Int64</span></span>   | <span data-ttu-id="c4fd1-132">グループメンバー数。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-132">The group member count.</span></span>                  |
| <span data-ttu-id="c4fd1-133">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="c4fd1-133">externalMemberCount</span></span>               | <span data-ttu-id="c4fd1-134">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-134">Int64</span></span>   | <span data-ttu-id="c4fd1-135">グループの外部メンバー数。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-135">The group external member count.</span></span>         |
| <span data-ttu-id="c4fd1-136">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="c4fd1-136">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="c4fd1-137">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-137">Int64</span></span>   | <span data-ttu-id="c4fd1-138">グループメールボックスが受信したメールの数。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-138">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="c4fd1-139">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="c4fd1-139">sharePointActiveFileCount</span></span>         | <span data-ttu-id="c4fd1-140">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-140">Int64</span></span>   | <span data-ttu-id="c4fd1-141">SharePoint グループサイト内のアクティブなファイルの数。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-141">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="c4fd1-142">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="c4fd1-142">yammerPostedMessageCount</span></span>          | <span data-ttu-id="c4fd1-143">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-143">Int64</span></span>   | <span data-ttu-id="c4fd1-144">Yammer グループに投稿されたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-144">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="c4fd1-145">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="c4fd1-145">yammerReadMessageCount</span></span>            | <span data-ttu-id="c4fd1-146">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-146">Int64</span></span>   | <span data-ttu-id="c4fd1-147">Yammer グループで読み取られたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-147">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="c4fd1-148">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="c4fd1-148">yammerLikedMessageCount</span></span>           | <span data-ttu-id="c4fd1-149">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-149">Int64</span></span>   | <span data-ttu-id="c4fd1-150">Yammer グループに賛同されたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-150">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="c4fd1-151">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="c4fd1-151">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="c4fd1-152">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-152">Int64</span></span>   | <span data-ttu-id="c4fd1-153">グループメールボックス内のアイテムの数。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-153">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="c4fd1-154">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="c4fd1-154">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="c4fd1-155">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-155">Int64</span></span>   | <span data-ttu-id="c4fd1-156">グループメールボックスで使用されている記憶域。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-156">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="c4fd1-157">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="c4fd1-157">sharePointTotalFileCount</span></span>          | <span data-ttu-id="c4fd1-158">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-158">Int64</span></span>   | <span data-ttu-id="c4fd1-159">SharePoint グループサイト内のファイルの合計数。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-159">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="c4fd1-160">Sharepointsitestorageused Inbytes</span><span class="sxs-lookup"><span data-stu-id="c4fd1-160">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="c4fd1-161">Int64</span><span class="sxs-lookup"><span data-stu-id="c4fd1-161">Int64</span></span>   | <span data-ttu-id="c4fd1-162">SharePoint グループサイトで使用される記憶域。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-162">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="c4fd1-163">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c4fd1-163">reportPeriod</span></span>                      | <span data-ttu-id="c4fd1-164">String</span><span class="sxs-lookup"><span data-stu-id="c4fd1-164">String</span></span>  | <span data-ttu-id="c4fd1-165">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-165">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c4fd1-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4fd1-166">JSON representation</span></span>

<span data-ttu-id="c4fd1-167">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c4fd1-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
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
