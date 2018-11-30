---
title: office365ServicesUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 975a70b040ac5886ea36219a5407f580a42aeadc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067407"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="8f5f7-103">office365ServicesUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8f5f7-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8f5f7-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f5f7-104">Properties</span></span>

| <span data-ttu-id="8f5f7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f5f7-105">Property</span></span>                 | <span data-ttu-id="8f5f7-106">型</span><span class="sxs-lookup"><span data-stu-id="8f5f7-106">Type</span></span>   | <span data-ttu-id="8f5f7-107">説明</span><span class="sxs-lookup"><span data-stu-id="8f5f7-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="8f5f7-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8f5f7-108">reportRefreshDate</span></span>        | <span data-ttu-id="8f5f7-109">Date</span><span class="sxs-lookup"><span data-stu-id="8f5f7-109">Date</span></span>   | <span data-ttu-id="8f5f7-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="8f5f7-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-111">exchangeActive</span></span>           | <span data-ttu-id="8f5f7-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-112">Int64</span></span>  | <span data-ttu-id="8f5f7-113">Exchange 上のアクティブ ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-113">The number of active users on Exchange.</span></span> <span data-ttu-id="8f5f7-114">読み取りし、電子メールを送信できるユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="8f5f7-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-115">exchangeInactive</span></span>         | <span data-ttu-id="8f5f7-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-116">Int64</span></span>  | <span data-ttu-id="8f5f7-117">Exchange 上のアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="8f5f7-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-118">oneDriveActive</span></span>           | <span data-ttu-id="8f5f7-119">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-119">Int64</span></span>  | <span data-ttu-id="8f5f7-120">OneDrive のアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="8f5f7-121">表示または編集したファイルを内部または外部でファイルを共有またはファイルを同期するユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="8f5f7-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-122">oneDriveInactive</span></span>         | <span data-ttu-id="8f5f7-123">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-123">Int64</span></span>  | <span data-ttu-id="8f5f7-124">OneDrive 上のアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="8f5f7-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-125">sharePointActive</span></span>         | <span data-ttu-id="8f5f7-126">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-126">Int64</span></span>  | <span data-ttu-id="8f5f7-127">SharePoint のアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="8f5f7-128">表示または編集したファイルをファイルを社内で共有または外部で、ファイルを同期または SharePoint ページを表示したすべてのユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="8f5f7-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-129">sharePointInactive</span></span>       | <span data-ttu-id="8f5f7-130">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-130">Int64</span></span>  | <span data-ttu-id="8f5f7-131">SharePoint でアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="8f5f7-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="8f5f7-133">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-133">Int64</span></span>  | <span data-ttu-id="8f5f7-134">Skype のビジネス上のアクティブ ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="8f5f7-135">整理または会議に参加またはピア ツー ピア セッションに参加しているユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="8f5f7-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="8f5f7-137">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-137">Int64</span></span>  | <span data-ttu-id="8f5f7-138">Skype のビジネス上のアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="8f5f7-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-139">yammerActive</span></span>             | <span data-ttu-id="8f5f7-140">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-140">Int64</span></span>  | <span data-ttu-id="8f5f7-141">Yammer のアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-141">The number of active users on Yammer.</span></span> <span data-ttu-id="8f5f7-142">投稿、読み取り、またはメッセージのようなユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="8f5f7-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-143">yammerInactive</span></span>           | <span data-ttu-id="8f5f7-144">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-144">Int64</span></span>  | <span data-ttu-id="8f5f7-145">Yammer にアクティブでないユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="8f5f7-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-146">teamsActive</span></span>              | <span data-ttu-id="8f5f7-147">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-147">Int64</span></span>  | <span data-ttu-id="8f5f7-148">チームのアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-148">The number of active users on Teams.</span></span> <span data-ttu-id="8f5f7-149">チームのチャネルでメッセージを投稿、プライベート チャットのセッションにメッセージを送信、または会議や通話に参加したユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="8f5f7-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="8f5f7-150">teamsInactive</span></span>            | <span data-ttu-id="8f5f7-151">Int64</span><span class="sxs-lookup"><span data-stu-id="8f5f7-151">Int64</span></span>  | <span data-ttu-id="8f5f7-152">チームのアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-152">The number of active users on Teams.</span></span>     |
| <span data-ttu-id="8f5f7-153">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8f5f7-153">reportPeriod</span></span>             | <span data-ttu-id="8f5f7-154">String</span><span class="sxs-lookup"><span data-stu-id="8f5f7-154">String</span></span> | <span data-ttu-id="8f5f7-155">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-155">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="8f5f7-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f5f7-156">JSON representation</span></span>

<span data-ttu-id="8f5f7-157">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8f5f7-157">The following is a JSON representation of the resource.</span></span>

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
  "reportPeriod": "String"
}
```
