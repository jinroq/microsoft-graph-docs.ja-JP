---
title: Office 365 アクティブ ユーザー レポート
description: Office 365 アクティブユーザーレポートを使用して、組織内の個人が使用している製品ライセンスの数を確認し、どのユーザーがどの製品を使用しているかに関する情報をドリルダウンできます。 このレポートは、監理者が十分に活用されていない製品や追加のトレーニングまたは情報を必要としているユーザーを特定するのに役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e31bc0ef8d2fa3147528503902c46b33d4944ce7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341998"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="06c58-104">Office 365 アクティブ ユーザー レポート</span><span class="sxs-lookup"><span data-stu-id="06c58-104">Office 365 active users reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06c58-105">Office 365 アクティブユーザーレポートを使用して、組織内の個人が使用している製品ライセンスの数を確認し、どのユーザーがどの製品を使用しているかに関する情報をドリルダウンできます。</span><span class="sxs-lookup"><span data-stu-id="06c58-105">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="06c58-106">このレポートは、監理者が十分に活用されていない製品や追加のトレーニングまたは情報を必要としているユーザーを特定するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="06c58-106">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="06c58-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06c58-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="06c58-108">レポート</span><span class="sxs-lookup"><span data-stu-id="06c58-108">Reports</span></span>
| <span data-ttu-id="06c58-109">関数</span><span class="sxs-lookup"><span data-stu-id="06c58-109">Function</span></span>                                 | <span data-ttu-id="06c58-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="06c58-110">CSV return type</span></span> | <span data-ttu-id="06c58-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="06c58-111">JSON return type</span></span>                         | <span data-ttu-id="06c58-112">説明</span><span class="sxs-lookup"><span data-stu-id="06c58-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="06c58-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="06c58-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="06c58-114">ストリーム</span><span class="sxs-lookup"><span data-stu-id="06c58-114">Stream</span></span>          | [<span data-ttu-id="06c58-115">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="06c58-115">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="06c58-116">Office 365 アクティブ ユーザーに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="06c58-116">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="06c58-117">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="06c58-117">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="06c58-118">Stream</span><span class="sxs-lookup"><span data-stu-id="06c58-118">Stream</span></span>          | [<span data-ttu-id="06c58-119">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="06c58-119">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="06c58-120">レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。</span><span class="sxs-lookup"><span data-stu-id="06c58-120">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="06c58-121">サービスのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="06c58-121">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="06c58-122">Stream</span><span class="sxs-lookup"><span data-stu-id="06c58-122">Stream</span></span>          | [<span data-ttu-id="06c58-123">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="06c58-123">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="06c58-124">アクティビティの種類とサービス別のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="06c58-124">Get the count of users by activity type and service.</span></span> |
