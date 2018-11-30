---
title: Office 365 アクティブ ユーザー レポート
description: Office 365 アクティブ ユーザー レポートを使用すると、組織内の個人に使用されている製品ライセンスの数を確認し、どのユーザーがどんな製品を使用しているかについて、情報を掘り下げることができます。 これらのレポートによって、管理者は使用率の低い製品や、追加トレーニングや追加情報を必要とする可能性のあるユーザーを特定することができます。
ms.openlocfilehash: 79f61dad9182b76c38de75b05cd458e2d23550e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022984"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="625de-104">Office 365 アクティブ ユーザー レポート</span><span class="sxs-lookup"><span data-stu-id="625de-104">Office 365 active users reports</span></span>

<span data-ttu-id="625de-105">Office 365 アクティブ ユーザー レポートを使用すると、組織内の個人に使用されている製品ライセンスの数を確認し、どのユーザーがどんな製品を使用しているかについて、情報を掘り下げることができます。</span><span class="sxs-lookup"><span data-stu-id="625de-105">You can use the Office 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="625de-106">これらのレポートによって、管理者は使用率の低い製品や、追加トレーニングや追加情報を必要とする可能性のあるユーザーを特定することができます。</span><span class="sxs-lookup"><span data-stu-id="625de-106">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="625de-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="625de-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="625de-108">レポート</span><span class="sxs-lookup"><span data-stu-id="625de-108">Reports</span></span>
| <span data-ttu-id="625de-109">関数</span><span class="sxs-lookup"><span data-stu-id="625de-109">Function</span></span>                                 | <span data-ttu-id="625de-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="625de-110">Return Type</span></span> | <span data-ttu-id="625de-111">説明</span><span class="sxs-lookup"><span data-stu-id="625de-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="625de-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="625de-112">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="625de-113">Stream</span><span class="sxs-lookup"><span data-stu-id="625de-113">Stream</span></span>      | <span data-ttu-id="625de-114">Office 365 アクティブ ユーザーに関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="625de-114">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="625de-115">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="625de-115">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="625de-116">Stream</span><span class="sxs-lookup"><span data-stu-id="625de-116">Stream</span></span>      | <span data-ttu-id="625de-117">レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。</span><span class="sxs-lookup"><span data-stu-id="625de-117">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="625de-118">サービスのユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="625de-118">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="625de-119">Stream</span><span class="sxs-lookup"><span data-stu-id="625de-119">Stream</span></span>      | <span data-ttu-id="625de-120">アクティビティの種類とサービス別のユーザー数を取得します。</span><span class="sxs-lookup"><span data-stu-id="625de-120">Get the count of users by activity type and service.</span></span> |
