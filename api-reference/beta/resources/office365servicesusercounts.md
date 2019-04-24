---
title: office365ServicesUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505460"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="88695-103">office365ServicesUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88695-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="88695-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88695-104">Properties</span></span>

| <span data-ttu-id="88695-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88695-105">Property</span></span>                 | <span data-ttu-id="88695-106">型</span><span class="sxs-lookup"><span data-stu-id="88695-106">Type</span></span>   | <span data-ttu-id="88695-107">説明</span><span class="sxs-lookup"><span data-stu-id="88695-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="88695-108">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="88695-108">reportRefreshDate</span></span>        | <span data-ttu-id="88695-109">Date</span><span class="sxs-lookup"><span data-stu-id="88695-109">Date</span></span>   | <span data-ttu-id="88695-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="88695-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="88695-111">exchangeactive</span><span class="sxs-lookup"><span data-stu-id="88695-111">exchangeActive</span></span>           | <span data-ttu-id="88695-112">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-112">Int64</span></span>  | <span data-ttu-id="88695-113">Exchange 上のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-113">The number of active users on Exchange.</span></span> <span data-ttu-id="88695-114">電子メールを読んだり、送信したりできるユーザーは、アクティブなユーザーであると見なされます。</span><span class="sxs-lookup"><span data-stu-id="88695-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="88695-115">exchangeinactive</span><span class="sxs-lookup"><span data-stu-id="88695-115">exchangeInactive</span></span>         | <span data-ttu-id="88695-116">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-116">Int64</span></span>  | <span data-ttu-id="88695-117">Exchange 上の非アクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="88695-118">onedrive active</span><span class="sxs-lookup"><span data-stu-id="88695-118">oneDriveActive</span></span>           | <span data-ttu-id="88695-119">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-119">Int64</span></span>  | <span data-ttu-id="88695-120">OneDrive 上のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="88695-121">ファイルを表示または編集したユーザー、内部または外部の共有ファイル、または同期したファイルは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="88695-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="88695-122">onedrive 非アクティブ</span><span class="sxs-lookup"><span data-stu-id="88695-122">oneDriveInactive</span></span>         | <span data-ttu-id="88695-123">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-123">Int64</span></span>  | <span data-ttu-id="88695-124">OneDrive 上の非アクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="88695-125">sharepointactive</span><span class="sxs-lookup"><span data-stu-id="88695-125">sharePointActive</span></span>         | <span data-ttu-id="88695-126">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-126">Int64</span></span>  | <span data-ttu-id="88695-127">SharePoint 上のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="88695-128">ファイルを表示または編集したユーザー、内部または外部の共有ファイル、同期したファイル、または SharePoint ページを表示したユーザーは、アクティブなユーザーであると見なされます。</span><span class="sxs-lookup"><span data-stu-id="88695-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="88695-129">sharepointinactive</span><span class="sxs-lookup"><span data-stu-id="88695-129">sharePointInactive</span></span>       | <span data-ttu-id="88695-130">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-130">Int64</span></span>  | <span data-ttu-id="88695-131">SharePoint 上の非アクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="88695-132">skypeforbusinessactive</span><span class="sxs-lookup"><span data-stu-id="88695-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="88695-133">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-133">Int64</span></span>  | <span data-ttu-id="88695-134">Skype for business 上のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="88695-135">電話会議に参加している、またはピアツーピアセッションに参加しているユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="88695-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="88695-136">skypeforbusinessinactive</span><span class="sxs-lookup"><span data-stu-id="88695-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="88695-137">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-137">Int64</span></span>  | <span data-ttu-id="88695-138">Skype for business で使用されていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="88695-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="88695-139">yammerActive</span></span>             | <span data-ttu-id="88695-140">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-140">Int64</span></span>  | <span data-ttu-id="88695-141">Yammer のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-141">The number of active users on Yammer.</span></span> <span data-ttu-id="88695-142">メッセージを投稿、閲覧、またはそのようにすることができるユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="88695-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="88695-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="88695-143">yammerInactive</span></span>           | <span data-ttu-id="88695-144">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-144">Int64</span></span>  | <span data-ttu-id="88695-145">Yammer の非アクティブユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="88695-146">teamsactive</span><span class="sxs-lookup"><span data-stu-id="88695-146">teamsActive</span></span>              | <span data-ttu-id="88695-147">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-147">Int64</span></span>  | <span data-ttu-id="88695-148">Microsoft Teams のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="88695-149">チームチャネルでメッセージを投稿したユーザー、プライベートチャットセッションでメッセージを送信したユーザー、または会議または通話に参加したユーザーは、アクティブなユーザーであると見なされます。</span><span class="sxs-lookup"><span data-stu-id="88695-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="88695-150">teamsinactive</span><span class="sxs-lookup"><span data-stu-id="88695-150">teamsInactive</span></span>            | <span data-ttu-id="88695-151">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-151">Int64</span></span>  | <span data-ttu-id="88695-152">Microsoft Teams の非アクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="88695-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="88695-153">office365Active</span></span>          | <span data-ttu-id="88695-154">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-154">Int64</span></span>  | <span data-ttu-id="88695-155">Office 365 上のアクティブユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="88695-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="88695-156">office365Inactive</span></span>        | <span data-ttu-id="88695-157">Int64</span><span class="sxs-lookup"><span data-stu-id="88695-157">Int64</span></span>  | <span data-ttu-id="88695-158">Office 365 の非アクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="88695-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="88695-159">reportperiod</span><span class="sxs-lookup"><span data-stu-id="88695-159">reportPeriod</span></span>             | <span data-ttu-id="88695-160">String</span><span class="sxs-lookup"><span data-stu-id="88695-160">String</span></span> | <span data-ttu-id="88695-161">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="88695-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="88695-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88695-162">JSON representation</span></span>

<span data-ttu-id="88695-163">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="88695-163">The following is a JSON representation of the resource.</span></span>

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
