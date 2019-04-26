---
title: メール アプリ使用状況レポート
description: Exchange Online への接続に使用されている電子メールアプリの数を確認できます。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: df40e61108a3933801f5e7c21057f71600b496ef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340195"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="19236-104">メール アプリ使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="19236-104">Email app usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19236-105">Exchange Online への接続に使用されている電子メールアプリの数を確認できます。</span><span class="sxs-lookup"><span data-stu-id="19236-105">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="19236-106">また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。</span><span class="sxs-lookup"><span data-stu-id="19236-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="19236-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19236-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="19236-108">レポート</span><span class="sxs-lookup"><span data-stu-id="19236-108">Reports</span></span>

| <span data-ttu-id="19236-109">関数</span><span class="sxs-lookup"><span data-stu-id="19236-109">Function</span></span>                                 | <span data-ttu-id="19236-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="19236-110">CSV return type</span></span> | <span data-ttu-id="19236-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="19236-111">JSON return type</span></span>                         | <span data-ttu-id="19236-112">説明</span><span class="sxs-lookup"><span data-stu-id="19236-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="19236-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="19236-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="19236-114">ストリーム</span><span class="sxs-lookup"><span data-stu-id="19236-114">Stream</span></span>          | [<span data-ttu-id="19236-115">emailapp使い方 userdetail</span><span class="sxs-lookup"><span data-stu-id="19236-115">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="19236-116">メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="19236-116">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="19236-117">アプリのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="19236-117">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="19236-118">Stream</span><span class="sxs-lookup"><span data-stu-id="19236-118">Stream</span></span>          | [<span data-ttu-id="19236-119">emailapp使い方 appsuser計数</span><span class="sxs-lookup"><span data-stu-id="19236-119">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="19236-120">メール アプリごとの、それぞれ別個のユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="19236-120">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="19236-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="19236-121">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="19236-122">Stream</span><span class="sxs-lookup"><span data-stu-id="19236-122">Stream</span></span>          | [<span data-ttu-id="19236-123">emailapp使い方 user計数</span><span class="sxs-lookup"><span data-stu-id="19236-123">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="19236-124">任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="19236-124">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="19236-125">バージョンのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="19236-125">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="19236-126">Stream</span><span class="sxs-lookup"><span data-stu-id="19236-126">Stream</span></span>          | [<span data-ttu-id="19236-127">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="19236-127">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="19236-128">Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="19236-128">Get the count of unique users by Outlook desktop version.</span></span> |
