---
title: メール アプリ使用状況レポート
description: メール アプリの使用状況レポートを使用して、Exchange Online に接続するために使用されたメール アプリの数を確認します。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。
localization_priority: Normal
ms.openlocfilehash: 3288d987719dd7ba005b0c6bb23231e367b2ad37
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869987"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="fba76-104">メール アプリ使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="fba76-104">Email app usage reports</span></span>

<span data-ttu-id="fba76-105">メール アプリの使用状況レポートを使用して、Exchange Online に接続するために使用されたメール アプリの数を確認します。</span><span class="sxs-lookup"><span data-stu-id="fba76-105">Use the email app usage reports to see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="fba76-106">また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。</span><span class="sxs-lookup"><span data-stu-id="fba76-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="fba76-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fba76-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="fba76-108">レポート</span><span class="sxs-lookup"><span data-stu-id="fba76-108">Reports</span></span>

| <span data-ttu-id="fba76-109">関数</span><span class="sxs-lookup"><span data-stu-id="fba76-109">Function</span></span>                                 | <span data-ttu-id="fba76-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fba76-110">Return Type</span></span> | <span data-ttu-id="fba76-111">説明</span><span class="sxs-lookup"><span data-stu-id="fba76-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="fba76-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="fba76-112">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="fba76-113">Stream</span><span class="sxs-lookup"><span data-stu-id="fba76-113">Stream</span></span>      | <span data-ttu-id="fba76-114">メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="fba76-114">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="fba76-115">アプリのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="fba76-115">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="fba76-116">Stream</span><span class="sxs-lookup"><span data-stu-id="fba76-116">Stream</span></span>      | <span data-ttu-id="fba76-117">メール アプリごとの、それぞれ別個のユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="fba76-117">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="fba76-118">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="fba76-118">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="fba76-119">Stream</span><span class="sxs-lookup"><span data-stu-id="fba76-119">Stream</span></span>      | <span data-ttu-id="fba76-120">任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="fba76-120">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="fba76-121">バージョンのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="fba76-121">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="fba76-122">Stream</span><span class="sxs-lookup"><span data-stu-id="fba76-122">Stream</span></span>      | <span data-ttu-id="fba76-123">Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="fba76-123">Get the count of unique users by Outlook desktop version.</span></span> |
