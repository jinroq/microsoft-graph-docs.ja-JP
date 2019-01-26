---
title: office365ServicesUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573894"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="19264-103">office365ServicesUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="19264-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="19264-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19264-104">Properties</span></span>

| <span data-ttu-id="19264-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19264-105">Property</span></span>                 | <span data-ttu-id="19264-106">型</span><span class="sxs-lookup"><span data-stu-id="19264-106">Type</span></span>   | <span data-ttu-id="19264-107">説明</span><span class="sxs-lookup"><span data-stu-id="19264-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="19264-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="19264-108">reportRefreshDate</span></span>        | <span data-ttu-id="19264-109">日付</span><span class="sxs-lookup"><span data-stu-id="19264-109">Date</span></span>   | <span data-ttu-id="19264-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="19264-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="19264-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="19264-111">exchangeActive</span></span>           | <span data-ttu-id="19264-112">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-112">Int64</span></span>  | <span data-ttu-id="19264-113">Exchange 上のアクティブ ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-113">The number of active users on Exchange.</span></span> <span data-ttu-id="19264-114">読み取りし、電子メールを送信できるユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="19264-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="19264-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="19264-115">exchangeInactive</span></span>         | <span data-ttu-id="19264-116">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-116">Int64</span></span>  | <span data-ttu-id="19264-117">Exchange 上のアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="19264-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="19264-118">oneDriveActive</span></span>           | <span data-ttu-id="19264-119">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-119">Int64</span></span>  | <span data-ttu-id="19264-120">OneDrive のアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="19264-121">表示または編集したファイルを内部または外部でファイルを共有またはファイルを同期するユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="19264-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="19264-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="19264-122">oneDriveInactive</span></span>         | <span data-ttu-id="19264-123">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-123">Int64</span></span>  | <span data-ttu-id="19264-124">OneDrive 上のアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="19264-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="19264-125">sharePointActive</span></span>         | <span data-ttu-id="19264-126">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-126">Int64</span></span>  | <span data-ttu-id="19264-127">SharePoint のアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="19264-128">表示または編集したファイルをファイルを社内で共有または外部で、ファイルを同期または SharePoint ページを表示したすべてのユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="19264-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="19264-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="19264-129">sharePointInactive</span></span>       | <span data-ttu-id="19264-130">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-130">Int64</span></span>  | <span data-ttu-id="19264-131">SharePoint でアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="19264-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="19264-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="19264-133">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-133">Int64</span></span>  | <span data-ttu-id="19264-134">Skype のビジネス上のアクティブ ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="19264-135">整理または会議に参加またはピア ツー ピア セッションに参加しているユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="19264-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="19264-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="19264-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="19264-137">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-137">Int64</span></span>  | <span data-ttu-id="19264-138">Skype のビジネス上のアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="19264-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="19264-139">yammerActive</span></span>             | <span data-ttu-id="19264-140">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-140">Int64</span></span>  | <span data-ttu-id="19264-141">Yammer のアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-141">The number of active users on Yammer.</span></span> <span data-ttu-id="19264-142">投稿、読み取り、またはメッセージのようなユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="19264-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="19264-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="19264-143">yammerInactive</span></span>           | <span data-ttu-id="19264-144">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-144">Int64</span></span>  | <span data-ttu-id="19264-145">Yammer にアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="19264-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="19264-146">teamsActive</span></span>              | <span data-ttu-id="19264-147">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-147">Int64</span></span>  | <span data-ttu-id="19264-148">マイクロソフトのチームのアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="19264-149">チームのチャネルでメッセージを投稿、プライベート チャットのセッションにメッセージを送信、または会議や通話に参加したユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="19264-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="19264-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="19264-150">teamsInactive</span></span>            | <span data-ttu-id="19264-151">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-151">Int64</span></span>  | <span data-ttu-id="19264-152">マイクロソフト チームのアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="19264-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="19264-153">office365Active</span></span>          | <span data-ttu-id="19264-154">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-154">Int64</span></span>  | <span data-ttu-id="19264-155">Office 365 のアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="19264-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="19264-156">office365Inactive</span></span>        | <span data-ttu-id="19264-157">Int64</span><span class="sxs-lookup"><span data-stu-id="19264-157">Int64</span></span>  | <span data-ttu-id="19264-158">Office 365 で使用頻度の低いユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="19264-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="19264-159">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="19264-159">reportPeriod</span></span>             | <span data-ttu-id="19264-160">String</span><span class="sxs-lookup"><span data-stu-id="19264-160">String</span></span> | <span data-ttu-id="19264-161">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="19264-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="19264-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="19264-162">JSON representation</span></span>

<span data-ttu-id="19264-163">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19264-163">The following is a JSON representation of the resource.</span></span>

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
