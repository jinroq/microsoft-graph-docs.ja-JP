---
title: office365ServicesUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 5958ab3cb05767465b0866078d378208f1b466e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009469"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="82f14-103">office365ServicesUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82f14-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="82f14-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82f14-104">Properties</span></span>

| <span data-ttu-id="82f14-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82f14-105">Property</span></span>                 | <span data-ttu-id="82f14-106">型</span><span class="sxs-lookup"><span data-stu-id="82f14-106">Type</span></span>   | <span data-ttu-id="82f14-107">説明</span><span class="sxs-lookup"><span data-stu-id="82f14-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="82f14-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="82f14-108">reportRefreshDate</span></span>        | <span data-ttu-id="82f14-109">日付</span><span class="sxs-lookup"><span data-stu-id="82f14-109">Date</span></span>   | <span data-ttu-id="82f14-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="82f14-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="82f14-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="82f14-111">exchangeActive</span></span>           | <span data-ttu-id="82f14-112">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-112">Int64</span></span>  | <span data-ttu-id="82f14-113">Exchange 上のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-113">The number of active users on Exchange.</span></span> <span data-ttu-id="82f14-114">電子メールを読んだり、送信したりできるユーザーは、アクティブなユーザーであると見なされます。</span><span class="sxs-lookup"><span data-stu-id="82f14-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="82f14-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="82f14-115">exchangeInactive</span></span>         | <span data-ttu-id="82f14-116">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-116">Int64</span></span>  | <span data-ttu-id="82f14-117">Exchange 上の非アクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="82f14-118">Onedrive Active</span><span class="sxs-lookup"><span data-stu-id="82f14-118">oneDriveActive</span></span>           | <span data-ttu-id="82f14-119">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-119">Int64</span></span>  | <span data-ttu-id="82f14-120">OneDrive 上のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="82f14-121">ファイルを表示または編集したユーザー、内部または外部の共有ファイル、または同期したファイルは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="82f14-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="82f14-122">Onedrive 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="82f14-122">oneDriveInactive</span></span>         | <span data-ttu-id="82f14-123">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-123">Int64</span></span>  | <span data-ttu-id="82f14-124">OneDrive 上の非アクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="82f14-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="82f14-125">sharePointActive</span></span>         | <span data-ttu-id="82f14-126">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-126">Int64</span></span>  | <span data-ttu-id="82f14-127">SharePoint 上のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="82f14-128">ファイルを表示または編集したユーザー、内部または外部の共有ファイル、同期したファイル、または SharePoint ページを表示したユーザーは、アクティブなユーザーであると見なされます。</span><span class="sxs-lookup"><span data-stu-id="82f14-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="82f14-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="82f14-129">sharePointInactive</span></span>       | <span data-ttu-id="82f14-130">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-130">Int64</span></span>  | <span data-ttu-id="82f14-131">SharePoint 上の非アクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="82f14-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="82f14-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="82f14-133">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-133">Int64</span></span>  | <span data-ttu-id="82f14-134">Skype For Business 上のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="82f14-135">電話会議に参加している、またはピアツーピアセッションに参加しているユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="82f14-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="82f14-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="82f14-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="82f14-137">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-137">Int64</span></span>  | <span data-ttu-id="82f14-138">Skype For Business で使用されていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="82f14-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="82f14-139">yammerActive</span></span>             | <span data-ttu-id="82f14-140">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-140">Int64</span></span>  | <span data-ttu-id="82f14-141">Yammer のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-141">The number of active users on Yammer.</span></span> <span data-ttu-id="82f14-142">メッセージを投稿、閲覧、またはそのようにすることができるユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="82f14-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="82f14-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="82f14-143">yammerInactive</span></span>           | <span data-ttu-id="82f14-144">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-144">Int64</span></span>  | <span data-ttu-id="82f14-145">Yammer の非アクティブユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="82f14-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="82f14-146">teamsActive</span></span>              | <span data-ttu-id="82f14-147">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-147">Int64</span></span>  | <span data-ttu-id="82f14-148">Microsoft Teams のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="82f14-149">チームチャネルでメッセージを投稿したユーザー、プライベートチャットセッションでメッセージを送信したユーザー、または会議または通話に参加したユーザーは、アクティブなユーザーであると見なされます。</span><span class="sxs-lookup"><span data-stu-id="82f14-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="82f14-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="82f14-150">teamsInactive</span></span>            | <span data-ttu-id="82f14-151">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-151">Int64</span></span>  | <span data-ttu-id="82f14-152">Microsoft Teams の非アクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="82f14-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="82f14-153">office365Active</span></span>          | <span data-ttu-id="82f14-154">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-154">Int64</span></span>  | <span data-ttu-id="82f14-155">Office 365 上のアクティブユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="82f14-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="82f14-156">office365Inactive</span></span>        | <span data-ttu-id="82f14-157">Int64</span><span class="sxs-lookup"><span data-stu-id="82f14-157">Int64</span></span>  | <span data-ttu-id="82f14-158">Office 365 の非アクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="82f14-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="82f14-159">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="82f14-159">reportPeriod</span></span>             | <span data-ttu-id="82f14-160">String</span><span class="sxs-lookup"><span data-stu-id="82f14-160">String</span></span> | <span data-ttu-id="82f14-161">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="82f14-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="82f14-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82f14-162">JSON representation</span></span>

<span data-ttu-id="82f14-163">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="82f14-163">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```
