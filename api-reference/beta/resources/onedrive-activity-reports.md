---
title: OneDrive アクティビティ レポート
description: Onedrive のファイルとの相互作用を参照することで、OneDrive を使用するためにライセンスされているすべてのユーザーのアクティビティを取得することができます。 また、共有されているファイルの数を表示することで、進行中のコラボレーションのレベルを理解することもできます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 710b2ed88deeec26846bb5afe7503808d8c470c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009441"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="2b72b-104">OneDrive アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="2b72b-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b72b-105">Onedrive のファイルとの相互作用を参照することで、OneDrive を使用するためにライセンスされているすべてのユーザーのアクティビティを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="2b72b-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="2b72b-106">また、共有されているファイルの数を表示することで、進行中のコラボレーションのレベルを理解することもできます。</span><span class="sxs-lookup"><span data-stu-id="2b72b-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="2b72b-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b72b-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="2b72b-108">レポート</span><span class="sxs-lookup"><span data-stu-id="2b72b-108">Reports</span></span>

| <span data-ttu-id="2b72b-109">関数</span><span class="sxs-lookup"><span data-stu-id="2b72b-109">Function</span></span>                                 | <span data-ttu-id="2b72b-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2b72b-110">CSV return type</span></span> | <span data-ttu-id="2b72b-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="2b72b-111">JSON return type</span></span>                         | <span data-ttu-id="2b72b-112">説明</span><span class="sxs-lookup"><span data-stu-id="2b72b-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="2b72b-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="2b72b-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="2b72b-114">ストリーム</span><span class="sxs-lookup"><span data-stu-id="2b72b-114">Stream</span></span>          | [<span data-ttu-id="2b72b-115">Onedrive Activityuserdetail</span><span class="sxs-lookup"><span data-stu-id="2b72b-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="2b72b-116">ユーザー別の OneDrive アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="2b72b-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="2b72b-117">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="2b72b-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="2b72b-118">Stream</span><span class="sxs-lookup"><span data-stu-id="2b72b-118">Stream</span></span>          | [<span data-ttu-id="2b72b-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="2b72b-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="2b72b-120">アクティブな OneDrive ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="2b72b-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="2b72b-121">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="2b72b-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="2b72b-122">Stream</span><span class="sxs-lookup"><span data-stu-id="2b72b-122">Stream</span></span>          | [<span data-ttu-id="2b72b-123">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="2b72b-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="2b72b-124">いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="2b72b-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
