---
title: office365GroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: dfc45c4973194d26c1830f8c36d3bf3b407d2e3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009504"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="7c110-103">office365GroupsActivityDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7c110-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7c110-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c110-104">Properties</span></span>

| <span data-ttu-id="7c110-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c110-105">Property</span></span>                          | <span data-ttu-id="7c110-106">型</span><span class="sxs-lookup"><span data-stu-id="7c110-106">Type</span></span>    | <span data-ttu-id="7c110-107">説明</span><span class="sxs-lookup"><span data-stu-id="7c110-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="7c110-108">groupId</span><span class="sxs-lookup"><span data-stu-id="7c110-108">groupId</span></span>                           | <span data-ttu-id="7c110-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7c110-109">String</span></span>  | <span data-ttu-id="7c110-110">グループ id。</span><span class="sxs-lookup"><span data-stu-id="7c110-110">The group id.</span></span>          |
| <span data-ttu-id="7c110-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7c110-111">reportRefreshDate</span></span>                 | <span data-ttu-id="7c110-112">日付</span><span class="sxs-lookup"><span data-stu-id="7c110-112">Date</span></span>    | <span data-ttu-id="7c110-113">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="7c110-113">The latest date of the content.</span></span>          |
| <span data-ttu-id="7c110-114">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="7c110-114">groupDisplayName</span></span>                  | <span data-ttu-id="7c110-115">String</span><span class="sxs-lookup"><span data-stu-id="7c110-115">String</span></span>  | <span data-ttu-id="7c110-116">グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="7c110-116">The display name of the group.</span></span>           |
| <span data-ttu-id="7c110-117">isDeleted</span><span class="sxs-lookup"><span data-stu-id="7c110-117">isDeleted</span></span>                         | <span data-ttu-id="7c110-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c110-118">Boolean</span></span> | <span data-ttu-id="7c110-119">このユーザーが削除されているか、または削除されているか。</span><span class="sxs-lookup"><span data-stu-id="7c110-119">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="7c110-120">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7c110-120">ownerPrincipalName</span></span>                | <span data-ttu-id="7c110-121">String</span><span class="sxs-lookup"><span data-stu-id="7c110-121">String</span></span>  | <span data-ttu-id="7c110-122">グループ所有者のプリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="7c110-122">The group owner principal name.</span></span>          |
| <span data-ttu-id="7c110-123">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7c110-123">lastActivityDate</span></span>                  | <span data-ttu-id="7c110-124">日付</span><span class="sxs-lookup"><span data-stu-id="7c110-124">Date</span></span>    | <span data-ttu-id="7c110-125">次のシナリオの最後のアクティビティの日付: グループメールが受信した電子メール。SharePoint ドキュメントライブラリでユーザーが表示、編集、共有、または同期されたファイル。ユーザーが SharePoint ページを表示した。Yammer グループ内のユーザー投稿、閲覧、またはいいねのメッセージ。</span><span class="sxs-lookup"><span data-stu-id="7c110-125">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="7c110-126">groupType</span><span class="sxs-lookup"><span data-stu-id="7c110-126">groupType</span></span>                         | <span data-ttu-id="7c110-127">String</span><span class="sxs-lookup"><span data-stu-id="7c110-127">String</span></span>  | <span data-ttu-id="7c110-128">グループの種類。</span><span class="sxs-lookup"><span data-stu-id="7c110-128">The group type.</span></span> <span data-ttu-id="7c110-129">使用可能な値は、 **Public**または**Private**です。</span><span class="sxs-lookup"><span data-stu-id="7c110-129">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="7c110-130">memberCount</span><span class="sxs-lookup"><span data-stu-id="7c110-130">memberCount</span></span>                       | <span data-ttu-id="7c110-131">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-131">Int64</span></span>   | <span data-ttu-id="7c110-132">グループメンバー数。</span><span class="sxs-lookup"><span data-stu-id="7c110-132">The group member count.</span></span>                  |
| <span data-ttu-id="7c110-133">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="7c110-133">externalMemberCount</span></span>               | <span data-ttu-id="7c110-134">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-134">Int64</span></span>   | <span data-ttu-id="7c110-135">グループの外部メンバー数。</span><span class="sxs-lookup"><span data-stu-id="7c110-135">The group external member count.</span></span>         |
| <span data-ttu-id="7c110-136">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="7c110-136">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="7c110-137">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-137">Int64</span></span>   | <span data-ttu-id="7c110-138">グループメールボックスが受信したメールの数。</span><span class="sxs-lookup"><span data-stu-id="7c110-138">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="7c110-139">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="7c110-139">sharePointActiveFileCount</span></span>         | <span data-ttu-id="7c110-140">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-140">Int64</span></span>   | <span data-ttu-id="7c110-141">SharePoint グループサイト内のアクティブなファイルの数。</span><span class="sxs-lookup"><span data-stu-id="7c110-141">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="7c110-142">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="7c110-142">yammerPostedMessageCount</span></span>          | <span data-ttu-id="7c110-143">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-143">Int64</span></span>   | <span data-ttu-id="7c110-144">Yammer グループに投稿されたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="7c110-144">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="7c110-145">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="7c110-145">yammerReadMessageCount</span></span>            | <span data-ttu-id="7c110-146">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-146">Int64</span></span>   | <span data-ttu-id="7c110-147">Yammer グループで読み取られたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="7c110-147">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="7c110-148">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="7c110-148">yammerLikedMessageCount</span></span>           | <span data-ttu-id="7c110-149">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-149">Int64</span></span>   | <span data-ttu-id="7c110-150">Yammer グループに賛同されたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="7c110-150">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="7c110-151">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="7c110-151">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="7c110-152">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-152">Int64</span></span>   | <span data-ttu-id="7c110-153">グループメールボックス内のアイテムの数。</span><span class="sxs-lookup"><span data-stu-id="7c110-153">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="7c110-154">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="7c110-154">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="7c110-155">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-155">Int64</span></span>   | <span data-ttu-id="7c110-156">グループメールボックスで使用されている記憶域。</span><span class="sxs-lookup"><span data-stu-id="7c110-156">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="7c110-157">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="7c110-157">sharePointTotalFileCount</span></span>          | <span data-ttu-id="7c110-158">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-158">Int64</span></span>   | <span data-ttu-id="7c110-159">SharePoint グループサイト内のファイルの合計数。</span><span class="sxs-lookup"><span data-stu-id="7c110-159">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="7c110-160">Sharepointsitestorageused Inbytes</span><span class="sxs-lookup"><span data-stu-id="7c110-160">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="7c110-161">Int64</span><span class="sxs-lookup"><span data-stu-id="7c110-161">Int64</span></span>   | <span data-ttu-id="7c110-162">SharePoint グループサイトで使用される記憶域。</span><span class="sxs-lookup"><span data-stu-id="7c110-162">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="7c110-163">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7c110-163">reportPeriod</span></span>                      | <span data-ttu-id="7c110-164">String</span><span class="sxs-lookup"><span data-stu-id="7c110-164">String</span></span>  | <span data-ttu-id="7c110-165">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c110-165">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="7c110-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7c110-166">JSON representation</span></span>

<span data-ttu-id="7c110-167">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c110-167">The following is a JSON representation of the resource.</span></span>

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
