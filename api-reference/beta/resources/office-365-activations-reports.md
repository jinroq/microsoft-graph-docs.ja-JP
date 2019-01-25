---
title: Office 365 アクティブ化レポート
description: Office 365 のライセンス認証のレポートを使用すると、ユーザー先のデバイスが少なくとも 1 つの Office 365 サブスクリプションを有効にして表示します。 デスクトップとデバイスの間でのアクティブ化の詳細と、Office 365 サブスクリプションのライセンス認証を Office 365 用リソース、プロジェクト、および Visio Pro の内訳を提供します。 このレポートを使用すると可能性があります、Office のサブスクリプションをアクティブにするのには追加のサポートを必要とするユーザーを識別できます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3f0abf320fed495040513df662be6d5c93658656
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522323"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="5cfa0-105">Office 365 アクティブ化レポート</span><span class="sxs-lookup"><span data-stu-id="5cfa0-105">Office 365 activations reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cfa0-106">Office 365 のライセンス認証のレポートを使用すると、ユーザー先のデバイスが少なくとも 1 つの Office 365 サブスクリプションを有効にして表示します。</span><span class="sxs-lookup"><span data-stu-id="5cfa0-106">The Office 365 activation report gives you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="5cfa0-107">デスクトップとデバイスの間でのアクティブ化の詳細と、Office 365 サブスクリプションのライセンス認証を Office 365 用リソース、プロジェクト、および Visio Pro の内訳を提供します。</span><span class="sxs-lookup"><span data-stu-id="5cfa0-107">It provides a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="5cfa0-108">このレポートを使用すると可能性があります、Office のサブスクリプションをアクティブにするのには追加のサポートを必要とするユーザーを識別できます。</span><span class="sxs-lookup"><span data-stu-id="5cfa0-108">This report could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="5cfa0-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cfa0-109">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="5cfa0-110">レポート</span><span class="sxs-lookup"><span data-stu-id="5cfa0-110">Reports</span></span>
| <span data-ttu-id="5cfa0-111">関数</span><span class="sxs-lookup"><span data-stu-id="5cfa0-111">Function</span></span>                                 | <span data-ttu-id="5cfa0-112">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5cfa0-112">CSV return type</span></span> | <span data-ttu-id="5cfa0-113">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5cfa0-113">JSON return type</span></span>                         | <span data-ttu-id="5cfa0-114">説明</span><span class="sxs-lookup"><span data-stu-id="5cfa0-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="5cfa0-115">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="5cfa0-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="5cfa0-116">Stream</span><span class="sxs-lookup"><span data-stu-id="5cfa0-116">Stream</span></span>          | [<span data-ttu-id="5cfa0-117">office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="5cfa0-117">office365ActivationsUserDetail</span></span>](../resources/office365activationsuserdetail.md) | <span data-ttu-id="5cfa0-118">Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="5cfa0-118">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="5cfa0-119">ライセンス認証の数を取得する</span><span class="sxs-lookup"><span data-stu-id="5cfa0-119">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="5cfa0-120">Stream</span><span class="sxs-lookup"><span data-stu-id="5cfa0-120">Stream</span></span>          | [<span data-ttu-id="5cfa0-121">office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="5cfa0-121">office365ActivationCounts</span></span>](../resources/office365activationcounts.md) | <span data-ttu-id="5cfa0-122">デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="5cfa0-122">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="5cfa0-123">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="5cfa0-123">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="5cfa0-124">Stream</span><span class="sxs-lookup"><span data-stu-id="5cfa0-124">Stream</span></span>          | [<span data-ttu-id="5cfa0-125">office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="5cfa0-125">office365ActivationsUserCounts</span></span>](../resources/office365activationsusercounts.md) | <span data-ttu-id="5cfa0-126">有効なユーザーで、デスクトップまたはデバイスで Office サブスクリプションがアクティブ化されているユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="5cfa0-126">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-activations-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
