---
title: Office 365 アクティブ化レポート
description: office 365 アクティブ化レポートには、少なくとも1つのデバイスで office 365 サブスクリプションをアクティブ化したユーザーが表示されます。 これにより、office 365 ProPlus、Project、および Visio Pro for office 365 サブスクリプションのライセンス認証の内訳に加え、デスクトップとデバイス間でのライセンス認証の内訳が提供されます。 このレポートは、Office サブスクリプションのライセンス認証を行うために追加のサポートが必要になる可能性があるユーザーを特定するのに役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 345ab500ef5986471bb801a88ee5886473a3dd60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581593"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="238ee-105">Office 365 アクティブ化レポート</span><span class="sxs-lookup"><span data-stu-id="238ee-105">Office 365 activations reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="238ee-106">office 365 アクティブ化レポートには、少なくとも1つのデバイスで office 365 サブスクリプションをアクティブ化したユーザーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="238ee-106">The Office 365 activation report gives you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="238ee-107">これにより、office 365 ProPlus、Project、および Visio Pro for office 365 サブスクリプションのライセンス認証の内訳に加え、デスクトップとデバイス間でのライセンス認証の内訳が提供されます。</span><span class="sxs-lookup"><span data-stu-id="238ee-107">It provides a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="238ee-108">このレポートは、Office サブスクリプションのライセンス認証を行うために追加のサポートが必要になる可能性があるユーザーを特定するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="238ee-108">This report could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="238ee-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="238ee-109">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="238ee-110">レポート</span><span class="sxs-lookup"><span data-stu-id="238ee-110">Reports</span></span>
| <span data-ttu-id="238ee-111">関数</span><span class="sxs-lookup"><span data-stu-id="238ee-111">Function</span></span>                                 | <span data-ttu-id="238ee-112">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="238ee-112">CSV return type</span></span> | <span data-ttu-id="238ee-113">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="238ee-113">JSON return type</span></span>                         | <span data-ttu-id="238ee-114">説明</span><span class="sxs-lookup"><span data-stu-id="238ee-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="238ee-115">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="238ee-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="238ee-116">ストリーム</span><span class="sxs-lookup"><span data-stu-id="238ee-116">Stream</span></span>          | [<span data-ttu-id="238ee-117">office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="238ee-117">office365ActivationsUserDetail</span></span>](../resources/office365activationsuserdetail.md) | <span data-ttu-id="238ee-118">Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="238ee-118">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="238ee-119">ライセンス認証の数を取得する</span><span class="sxs-lookup"><span data-stu-id="238ee-119">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="238ee-120">Stream</span><span class="sxs-lookup"><span data-stu-id="238ee-120">Stream</span></span>          | [<span data-ttu-id="238ee-121">office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="238ee-121">office365ActivationCounts</span></span>](../resources/office365activationcounts.md) | <span data-ttu-id="238ee-122">デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="238ee-122">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="238ee-123">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="238ee-123">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="238ee-124">Stream</span><span class="sxs-lookup"><span data-stu-id="238ee-124">Stream</span></span>          | [<span data-ttu-id="238ee-125">office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="238ee-125">office365ActivationsUserCounts</span></span>](../resources/office365activationsusercounts.md) | <span data-ttu-id="238ee-126">有効なユーザーで、デスクトップまたはデバイスで Office サブスクリプションがアクティブ化されているユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="238ee-126">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-activations-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
