---
title: OneDrive アクティビティ レポート
description: OneDrive 上のファイルとの相互作用を参照して OneDrive を使用するライセンスのすべてのユーザーの利用状況を取得できます。 共有されるファイルの数を表示することによって起こっているのコラボレーションのレベルを理解することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d545f1d92beee89e19eb47cfd8c6ba8c391c5349
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574006"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="3163a-104">OneDrive アクティビティ レポート</span><span class="sxs-lookup"><span data-stu-id="3163a-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3163a-105">OneDrive 上のファイルとの相互作用を参照して OneDrive を使用するライセンスのすべてのユーザーの利用状況を取得できます。</span><span class="sxs-lookup"><span data-stu-id="3163a-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="3163a-106">共有されるファイルの数を表示することによって起こっているのコラボレーションのレベルを理解することができます。</span><span class="sxs-lookup"><span data-stu-id="3163a-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="3163a-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business のアクティビティ](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3163a-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="3163a-108">レポート</span><span class="sxs-lookup"><span data-stu-id="3163a-108">Reports</span></span>

| <span data-ttu-id="3163a-109">関数</span><span class="sxs-lookup"><span data-stu-id="3163a-109">Function</span></span>                                 | <span data-ttu-id="3163a-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3163a-110">CSV return type</span></span> | <span data-ttu-id="3163a-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3163a-111">JSON return type</span></span>                         | <span data-ttu-id="3163a-112">説明</span><span class="sxs-lookup"><span data-stu-id="3163a-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="3163a-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="3163a-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="3163a-114">Stream</span><span class="sxs-lookup"><span data-stu-id="3163a-114">Stream</span></span>          | [<span data-ttu-id="3163a-115">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="3163a-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="3163a-116">ユーザー別の OneDrive アクティビティに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="3163a-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="3163a-117">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="3163a-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="3163a-118">Stream</span><span class="sxs-lookup"><span data-stu-id="3163a-118">Stream</span></span>          | [<span data-ttu-id="3163a-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="3163a-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="3163a-120">アクティブな OneDrive ユーザーの数の傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="3163a-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="3163a-121">ファイルの数を取得する</span><span class="sxs-lookup"><span data-stu-id="3163a-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="3163a-122">Stream</span><span class="sxs-lookup"><span data-stu-id="3163a-122">Stream</span></span>          | [<span data-ttu-id="3163a-123">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="3163a-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="3163a-124">いずれかの OneDrive アカウントに対してファイル操作を実行した、一意のライセンス ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="3163a-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
