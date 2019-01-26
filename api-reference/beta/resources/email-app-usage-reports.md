---
title: メール アプリ使用状況レポート
description: 電子メール アプリケーションの数を使用して Exchange Online に接続を確認できます。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 7f332359af9a6147894bb69e6d12532a83394bb5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573747"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="c4e86-104">メール アプリ使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="c4e86-104">Email app usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4e86-105">電子メール アプリケーションの数を使用して Exchange Online に接続を確認できます。</span><span class="sxs-lookup"><span data-stu-id="c4e86-105">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="c4e86-106">また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。</span><span class="sxs-lookup"><span data-stu-id="c4e86-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="c4e86-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4e86-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="c4e86-108">レポート</span><span class="sxs-lookup"><span data-stu-id="c4e86-108">Reports</span></span>

| <span data-ttu-id="c4e86-109">関数</span><span class="sxs-lookup"><span data-stu-id="c4e86-109">Function</span></span>                                 | <span data-ttu-id="c4e86-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c4e86-110">CSV return type</span></span> | <span data-ttu-id="c4e86-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c4e86-111">JSON return type</span></span>                         | <span data-ttu-id="c4e86-112">説明</span><span class="sxs-lookup"><span data-stu-id="c4e86-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="c4e86-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="c4e86-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="c4e86-114">Stream</span><span class="sxs-lookup"><span data-stu-id="c4e86-114">Stream</span></span>          | [<span data-ttu-id="c4e86-115">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="c4e86-115">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="c4e86-116">メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="c4e86-116">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="c4e86-117">アプリのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="c4e86-117">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="c4e86-118">Stream</span><span class="sxs-lookup"><span data-stu-id="c4e86-118">Stream</span></span>          | [<span data-ttu-id="c4e86-119">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="c4e86-119">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="c4e86-120">メール アプリごとの、それぞれ別個のユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c4e86-120">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="c4e86-121">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="c4e86-121">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="c4e86-122">Stream</span><span class="sxs-lookup"><span data-stu-id="c4e86-122">Stream</span></span>          | [<span data-ttu-id="c4e86-123">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="c4e86-123">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="c4e86-124">任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c4e86-124">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="c4e86-125">バージョンのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="c4e86-125">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="c4e86-126">Stream</span><span class="sxs-lookup"><span data-stu-id="c4e86-126">Stream</span></span>          | [<span data-ttu-id="c4e86-127">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="c4e86-127">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="c4e86-128">Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c4e86-128">Get the count of unique users by Outlook desktop version.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-app-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
