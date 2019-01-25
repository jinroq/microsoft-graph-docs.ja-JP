---
title: Office 365 アクティブ ユーザー レポート
description: 製品ライセンスの数は、個人、組織内で使用されているを確認するのには Office 365 のユーザーのアクティブなレポートを使用し、ユーザーについては、どのような製品を使用している情報にドリルダウンできます。 このレポートは、管理者が使用率の低い製品またはその他のトレーニングや情報が必要なユーザーの識別に役立ちます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e85924b7066dde92f0db5fd0b3f1f83dd32fd0c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516211"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="bb17d-104">Office 365 アクティブ ユーザー レポート</span><span class="sxs-lookup"><span data-stu-id="bb17d-104">Office 365 active users reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb17d-105">製品ライセンスの数は、個人、組織内で使用されているを確認するのには Office 365 のユーザーのアクティブなレポートを使用し、ユーザーについては、どのような製品を使用している情報にドリルダウンできます。</span><span class="sxs-lookup"><span data-stu-id="bb17d-105">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="bb17d-106">このレポートは、管理者が使用率の低い製品またはその他のトレーニングや情報が必要なユーザーの識別に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="bb17d-106">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="bb17d-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb17d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="bb17d-108">レポート</span><span class="sxs-lookup"><span data-stu-id="bb17d-108">Reports</span></span>
| <span data-ttu-id="bb17d-109">関数</span><span class="sxs-lookup"><span data-stu-id="bb17d-109">Function</span></span>                                 | <span data-ttu-id="bb17d-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bb17d-110">CSV return type</span></span> | <span data-ttu-id="bb17d-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bb17d-111">JSON return type</span></span>                         | <span data-ttu-id="bb17d-112">説明</span><span class="sxs-lookup"><span data-stu-id="bb17d-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="bb17d-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="bb17d-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="bb17d-114">Stream</span><span class="sxs-lookup"><span data-stu-id="bb17d-114">Stream</span></span>          | [<span data-ttu-id="bb17d-115">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="bb17d-115">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="bb17d-116">Office 365 アクティブ ユーザーに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="bb17d-116">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="bb17d-117">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="bb17d-117">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="bb17d-118">ストリーム</span><span class="sxs-lookup"><span data-stu-id="bb17d-118">Stream</span></span>          | [<span data-ttu-id="bb17d-119">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="bb17d-119">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="bb17d-120">レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。</span><span class="sxs-lookup"><span data-stu-id="bb17d-120">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="bb17d-121">サービスのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="bb17d-121">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="bb17d-122">Stream</span><span class="sxs-lookup"><span data-stu-id="bb17d-122">Stream</span></span>          | [<span data-ttu-id="bb17d-123">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="bb17d-123">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="bb17d-124">アクティビティの種類とサービス別のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="bb17d-124">Get the count of users by activity type and service.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
