---
title: office365ActiveUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bbc51e4859b005c01b0f8d2cfb2db3ca902d60e2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572207"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="0fc95-103">office365ActiveUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0fc95-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0fc95-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fc95-104">Properties</span></span>

| <span data-ttu-id="0fc95-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fc95-105">Property</span></span>          | <span data-ttu-id="0fc95-106">型</span><span class="sxs-lookup"><span data-stu-id="0fc95-106">Type</span></span>   | <span data-ttu-id="0fc95-107">説明</span><span class="sxs-lookup"><span data-stu-id="0fc95-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="0fc95-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0fc95-108">reportRefreshDate</span></span> | <span data-ttu-id="0fc95-109">日付</span><span class="sxs-lookup"><span data-stu-id="0fc95-109">Date</span></span>   | <span data-ttu-id="0fc95-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="0fc95-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="0fc95-111">office365</span><span class="sxs-lookup"><span data-stu-id="0fc95-111">office365</span></span>         | <span data-ttu-id="0fc95-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0fc95-112">Int64</span></span>  | <span data-ttu-id="0fc95-113">Office 365 のアクティブ ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="0fc95-113">The number of active users in Office 365.</span></span> <span data-ttu-id="0fc95-114">この数値には、Exchange、OneDrive、SharePoint、Skype のビジネス、Yammer、およびマイクロソフトのチームで作業中のすべてのユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="0fc95-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="0fc95-115">それぞれのプロパティの説明では、各製品のアクティブなユーザーの定義が表示されます。</span><span class="sxs-lookup"><span data-stu-id="0fc95-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="0fc95-116">交換</span><span class="sxs-lookup"><span data-stu-id="0fc95-116">exchange</span></span>          | <span data-ttu-id="0fc95-117">Int64</span><span class="sxs-lookup"><span data-stu-id="0fc95-117">Int64</span></span>  | <span data-ttu-id="0fc95-118">Exchange 内のアクティブ ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="0fc95-118">The number of active users in Exchange.</span></span> <span data-ttu-id="0fc95-119">読み取りし、電子メールを送信できるユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="0fc95-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="0fc95-120">oneDrive</span><span class="sxs-lookup"><span data-stu-id="0fc95-120">oneDrive</span></span>          | <span data-ttu-id="0fc95-121">Int64</span><span class="sxs-lookup"><span data-stu-id="0fc95-121">Int64</span></span>  | <span data-ttu-id="0fc95-122">OneDrive でアクティブなユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="0fc95-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="0fc95-123">表示または編集したファイルを内部または外部でファイルを共有またはファイルを同期するユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="0fc95-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="0fc95-124">sharePoint</span><span class="sxs-lookup"><span data-stu-id="0fc95-124">sharePoint</span></span>        | <span data-ttu-id="0fc95-125">Int64</span><span class="sxs-lookup"><span data-stu-id="0fc95-125">Int64</span></span>  | <span data-ttu-id="0fc95-126">SharePoint でのアクティブ ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="0fc95-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="0fc95-127">表示または編集したファイルをファイルを社内で共有または外部で、ファイルを同期または SharePoint ページを表示したすべてのユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="0fc95-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="0fc95-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="0fc95-128">skypeForBusiness</span></span>  | <span data-ttu-id="0fc95-129">Int64</span><span class="sxs-lookup"><span data-stu-id="0fc95-129">Int64</span></span>  | <span data-ttu-id="0fc95-130">Skype のビジネスでのアクティブ ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="0fc95-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="0fc95-131">整理または会議に参加またはピア ツー ピア セッションに参加しているユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="0fc95-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="0fc95-132">yammer</span><span class="sxs-lookup"><span data-stu-id="0fc95-132">yammer</span></span>            | <span data-ttu-id="0fc95-133">Int64</span><span class="sxs-lookup"><span data-stu-id="0fc95-133">Int64</span></span>  | <span data-ttu-id="0fc95-134">Yammer のアクティブ ユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="0fc95-134">The number of active users in Yammer.</span></span> <span data-ttu-id="0fc95-135">投稿、読み取り、またはメッセージのようなユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="0fc95-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="0fc95-136">チーム</span><span class="sxs-lookup"><span data-stu-id="0fc95-136">teams</span></span>             | <span data-ttu-id="0fc95-137">Int64</span><span class="sxs-lookup"><span data-stu-id="0fc95-137">Int64</span></span>  | <span data-ttu-id="0fc95-138">マイクロソフトのチームで作業中のユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="0fc95-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="0fc95-139">チームのチャネルでメッセージを投稿、プライベート チャットのセッションにメッセージを送信、または会議や通話に参加したユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="0fc95-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="0fc95-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="0fc95-140">reportDate</span></span>        | <span data-ttu-id="0fc95-141">日付</span><span class="sxs-lookup"><span data-stu-id="0fc95-141">Date</span></span>   | <span data-ttu-id="0fc95-142">複数のユーザーがアクティブだった日付。</span><span class="sxs-lookup"><span data-stu-id="0fc95-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="0fc95-143">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0fc95-143">reportPeriod</span></span>      | <span data-ttu-id="0fc95-144">String</span><span class="sxs-lookup"><span data-stu-id="0fc95-144">String</span></span> | <span data-ttu-id="0fc95-145">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="0fc95-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="0fc95-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0fc95-146">JSON representation</span></span>

<span data-ttu-id="0fc95-147">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0fc95-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
