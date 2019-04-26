---
title: OneDrive アクティビティ レポート
description: onedrive のファイルとの相互作用を参照することで、onedrive を使用するためにライセンスされているすべてのユーザーのアクティビティを取得することができます。 また、共有されているファイルの数を表示することで、進行中のコラボレーションのレベルを理解することもできます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3a99ba5dbc1a61b11d916c9fff90cec53a4eeaf9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345533"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="73b6c-104">OneDrive アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="73b6c-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73b6c-105">onedrive のファイルとの相互作用を参照することで、onedrive を使用するためにライセンスされているすべてのユーザーのアクティビティを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="73b6c-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="73b6c-106">また、共有されているファイルの数を表示することで、進行中のコラボレーションのレベルを理解することもできます。</span><span class="sxs-lookup"><span data-stu-id="73b6c-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="73b6c-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73b6c-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="73b6c-108">レポート</span><span class="sxs-lookup"><span data-stu-id="73b6c-108">Reports</span></span>

| <span data-ttu-id="73b6c-109">関数</span><span class="sxs-lookup"><span data-stu-id="73b6c-109">Function</span></span>                                 | <span data-ttu-id="73b6c-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="73b6c-110">CSV return type</span></span> | <span data-ttu-id="73b6c-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="73b6c-111">JSON return type</span></span>                         | <span data-ttu-id="73b6c-112">説明</span><span class="sxs-lookup"><span data-stu-id="73b6c-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="73b6c-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="73b6c-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="73b6c-114">ストリーム</span><span class="sxs-lookup"><span data-stu-id="73b6c-114">Stream</span></span>          | [<span data-ttu-id="73b6c-115">onedrive activityuserdetail</span><span class="sxs-lookup"><span data-stu-id="73b6c-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="73b6c-116">ユーザー別の OneDrive アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="73b6c-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="73b6c-117">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="73b6c-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="73b6c-118">Stream</span><span class="sxs-lookup"><span data-stu-id="73b6c-118">Stream</span></span>          | [<span data-ttu-id="73b6c-119">siteactivitysummary</span><span class="sxs-lookup"><span data-stu-id="73b6c-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="73b6c-120">アクティブな OneDrive ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="73b6c-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="73b6c-121">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="73b6c-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="73b6c-122">Stream</span><span class="sxs-lookup"><span data-stu-id="73b6c-122">Stream</span></span>          | [<span data-ttu-id="73b6c-123">siteactivitysummary</span><span class="sxs-lookup"><span data-stu-id="73b6c-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="73b6c-124">いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="73b6c-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
