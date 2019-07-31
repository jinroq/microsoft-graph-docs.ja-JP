---
title: メール アプリ使用状況レポート
description: Exchange Online への接続に使用されている電子メールアプリの数を確認できます。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: b7aeac4800fbd7681b60210e7f65c96e7086705c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972258"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="abfac-104">メール アプリ使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="abfac-104">Email app usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abfac-105">Exchange Online への接続に使用されている電子メールアプリの数を確認できます。</span><span class="sxs-lookup"><span data-stu-id="abfac-105">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="abfac-106">また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。</span><span class="sxs-lookup"><span data-stu-id="abfac-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="abfac-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abfac-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="abfac-108">レポート</span><span class="sxs-lookup"><span data-stu-id="abfac-108">Reports</span></span>

| <span data-ttu-id="abfac-109">関数</span><span class="sxs-lookup"><span data-stu-id="abfac-109">Function</span></span>                                 | <span data-ttu-id="abfac-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="abfac-110">CSV return type</span></span> | <span data-ttu-id="abfac-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="abfac-111">JSON return type</span></span>                         | <span data-ttu-id="abfac-112">説明</span><span class="sxs-lookup"><span data-stu-id="abfac-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="abfac-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="abfac-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="abfac-114">ストリーム</span><span class="sxs-lookup"><span data-stu-id="abfac-114">Stream</span></span>          | [<span data-ttu-id="abfac-115">Emailapp使い方 Userdetail</span><span class="sxs-lookup"><span data-stu-id="abfac-115">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="abfac-116">メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="abfac-116">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="abfac-117">アプリのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="abfac-117">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="abfac-118">Stream</span><span class="sxs-lookup"><span data-stu-id="abfac-118">Stream</span></span>          | [<span data-ttu-id="abfac-119">Emailapp使い方 Appsuser計数</span><span class="sxs-lookup"><span data-stu-id="abfac-119">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="abfac-120">メール アプリごとの、それぞれ別個のユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="abfac-120">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="abfac-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="abfac-121">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="abfac-122">Stream</span><span class="sxs-lookup"><span data-stu-id="abfac-122">Stream</span></span>          | [<span data-ttu-id="abfac-123">Emailapp使い方 User計数</span><span class="sxs-lookup"><span data-stu-id="abfac-123">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="abfac-124">任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="abfac-124">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="abfac-125">バージョンのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="abfac-125">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="abfac-126">Stream</span><span class="sxs-lookup"><span data-stu-id="abfac-126">Stream</span></span>          | [<span data-ttu-id="abfac-127">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="abfac-127">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="abfac-128">Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="abfac-128">Get the count of unique users by Outlook desktop version.</span></span> |
