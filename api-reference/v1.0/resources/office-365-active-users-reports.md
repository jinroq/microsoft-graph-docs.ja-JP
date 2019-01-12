---
title: Office 365 アクティブ ユーザー レポート
description: Office 365 アクティブ ユーザー レポートを使用すると、組織内の個人に使用されている製品ライセンスの数を確認し、どのユーザーがどんな製品を使用しているかについて、情報を掘り下げることができます。 これらのレポートによって、管理者は使用率の低い製品や、追加トレーニングや追加情報を必要とする可能性のあるユーザーを特定することができます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 0ac5c3080469b8d918ee631edaf1473141a60dca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918001"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="979d4-104">Office 365 アクティブ ユーザー レポート</span><span class="sxs-lookup"><span data-stu-id="979d4-104">Office 365 active users reports</span></span>

<span data-ttu-id="979d4-105">Office 365 アクティブ ユーザー レポートを使用すると、組織内の個人に使用されている製品ライセンスの数を確認し、どのユーザーがどんな製品を使用しているかについて、情報を掘り下げることができます。</span><span class="sxs-lookup"><span data-stu-id="979d4-105">You can use the Office 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="979d4-106">これらのレポートによって、管理者は使用率の低い製品や、追加トレーニングや追加情報を必要とする可能性のあるユーザーを特定することができます。</span><span class="sxs-lookup"><span data-stu-id="979d4-106">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="979d4-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="979d4-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="979d4-108">レポート</span><span class="sxs-lookup"><span data-stu-id="979d4-108">Reports</span></span>
| <span data-ttu-id="979d4-109">関数</span><span class="sxs-lookup"><span data-stu-id="979d4-109">Function</span></span>                                 | <span data-ttu-id="979d4-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="979d4-110">Return Type</span></span> | <span data-ttu-id="979d4-111">説明</span><span class="sxs-lookup"><span data-stu-id="979d4-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="979d4-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="979d4-112">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="979d4-113">Stream</span><span class="sxs-lookup"><span data-stu-id="979d4-113">Stream</span></span>      | <span data-ttu-id="979d4-114">Office 365 アクティブ ユーザーに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="979d4-114">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="979d4-115">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="979d4-115">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="979d4-116">Stream</span><span class="sxs-lookup"><span data-stu-id="979d4-116">Stream</span></span>      | <span data-ttu-id="979d4-117">レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。</span><span class="sxs-lookup"><span data-stu-id="979d4-117">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="979d4-118">サービスのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="979d4-118">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="979d4-119">Stream</span><span class="sxs-lookup"><span data-stu-id="979d4-119">Stream</span></span>      | <span data-ttu-id="979d4-120">アクティビティの種類とサービス別のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="979d4-120">Get the count of users by activity type and service.</span></span> |
