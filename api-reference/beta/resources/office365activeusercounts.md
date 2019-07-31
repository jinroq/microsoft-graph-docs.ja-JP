---
title: office365ActiveUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0d0ebd451252766801239e63804b59b9a1747764
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966546"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="8afd0-103">office365ActiveUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8afd0-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8afd0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8afd0-104">Properties</span></span>

| <span data-ttu-id="8afd0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8afd0-105">Property</span></span>          | <span data-ttu-id="8afd0-106">型</span><span class="sxs-lookup"><span data-stu-id="8afd0-106">Type</span></span>   | <span data-ttu-id="8afd0-107">説明</span><span class="sxs-lookup"><span data-stu-id="8afd0-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="8afd0-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8afd0-108">reportRefreshDate</span></span> | <span data-ttu-id="8afd0-109">日付</span><span class="sxs-lookup"><span data-stu-id="8afd0-109">Date</span></span>   | <span data-ttu-id="8afd0-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="8afd0-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="8afd0-111">office</span><span class="sxs-lookup"><span data-stu-id="8afd0-111">office365</span></span>         | <span data-ttu-id="8afd0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8afd0-112">Int64</span></span>  | <span data-ttu-id="8afd0-113">Office 365 でアクティブになっているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8afd0-113">The number of active users in Office 365.</span></span> <span data-ttu-id="8afd0-114">この番号には、Exchange、OneDrive、SharePoint、Skype For Business、Yammer、Microsoft Teams のすべてのアクティブユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8afd0-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="8afd0-115">各製品のアクティブユーザーの定義については、それぞれのプロパティの説明を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8afd0-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="8afd0-116">変換</span><span class="sxs-lookup"><span data-stu-id="8afd0-116">exchange</span></span>          | <span data-ttu-id="8afd0-117">Int64</span><span class="sxs-lookup"><span data-stu-id="8afd0-117">Int64</span></span>  | <span data-ttu-id="8afd0-118">Exchange 内のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8afd0-118">The number of active users in Exchange.</span></span> <span data-ttu-id="8afd0-119">電子メールを読んだり、送信したりできるユーザーは、アクティブなユーザーであると見なされます。</span><span class="sxs-lookup"><span data-stu-id="8afd0-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="8afd0-120">スペース</span><span class="sxs-lookup"><span data-stu-id="8afd0-120">oneDrive</span></span>          | <span data-ttu-id="8afd0-121">Int64</span><span class="sxs-lookup"><span data-stu-id="8afd0-121">Int64</span></span>  | <span data-ttu-id="8afd0-122">OneDrive でアクティブになっているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8afd0-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="8afd0-123">ファイルを表示または編集したユーザー、内部または外部の共有ファイル、または同期したファイルは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="8afd0-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="8afd0-124">sharePoint</span><span class="sxs-lookup"><span data-stu-id="8afd0-124">sharePoint</span></span>        | <span data-ttu-id="8afd0-125">Int64</span><span class="sxs-lookup"><span data-stu-id="8afd0-125">Int64</span></span>  | <span data-ttu-id="8afd0-126">SharePoint のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8afd0-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="8afd0-127">ファイルを表示または編集したユーザー、内部または外部の共有ファイル、同期したファイル、または SharePoint ページを表示したユーザーは、アクティブなユーザーであると見なされます。</span><span class="sxs-lookup"><span data-stu-id="8afd0-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="8afd0-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="8afd0-128">skypeForBusiness</span></span>  | <span data-ttu-id="8afd0-129">Int64</span><span class="sxs-lookup"><span data-stu-id="8afd0-129">Int64</span></span>  | <span data-ttu-id="8afd0-130">Skype For Business のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8afd0-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="8afd0-131">電話会議に参加している、またはピアツーピアセッションに参加しているユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="8afd0-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="8afd0-132">yammer</span><span class="sxs-lookup"><span data-stu-id="8afd0-132">yammer</span></span>            | <span data-ttu-id="8afd0-133">Int64</span><span class="sxs-lookup"><span data-stu-id="8afd0-133">Int64</span></span>  | <span data-ttu-id="8afd0-134">Yammer のアクティブユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8afd0-134">The number of active users in Yammer.</span></span> <span data-ttu-id="8afd0-135">メッセージを投稿、閲覧、またはそのようにすることができるユーザーは、アクティブなユーザーと見なされます。</span><span class="sxs-lookup"><span data-stu-id="8afd0-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="8afd0-136">teams</span><span class="sxs-lookup"><span data-stu-id="8afd0-136">teams</span></span>             | <span data-ttu-id="8afd0-137">Int64</span><span class="sxs-lookup"><span data-stu-id="8afd0-137">Int64</span></span>  | <span data-ttu-id="8afd0-138">Microsoft Teams のアクティブなユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8afd0-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="8afd0-139">チームチャネルでメッセージを投稿したユーザー、プライベートチャットセッションでメッセージを送信したユーザー、または会議または通話に参加したユーザーは、アクティブなユーザーであると見なされます。</span><span class="sxs-lookup"><span data-stu-id="8afd0-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="8afd0-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="8afd0-140">reportDate</span></span>        | <span data-ttu-id="8afd0-141">日付</span><span class="sxs-lookup"><span data-stu-id="8afd0-141">Date</span></span>   | <span data-ttu-id="8afd0-142">ユーザー数がアクティブであった日付。</span><span class="sxs-lookup"><span data-stu-id="8afd0-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="8afd0-143">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8afd0-143">reportPeriod</span></span>      | <span data-ttu-id="8afd0-144">String</span><span class="sxs-lookup"><span data-stu-id="8afd0-144">String</span></span> | <span data-ttu-id="8afd0-145">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="8afd0-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="8afd0-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8afd0-146">JSON representation</span></span>

<span data-ttu-id="8afd0-147">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8afd0-147">The following is a JSON representation of the resource.</span></span>

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
