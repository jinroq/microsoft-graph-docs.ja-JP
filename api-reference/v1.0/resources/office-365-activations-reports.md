---
title: Office 365 アクティブ化レポート
description: Office 365 アクティブ化レポートでは、1 つ以上のデバイスで Office 365 サブスクリプションをアクティブ化したユーザーが表示されます。 これらのレポートでは、Office 365 ProPlus、Project、Visio Pro for Office 365 のサブスクリプションのアクティブ化の詳細、およびデスクトップとデバイス全体にわたるアクティブ化の詳細を確認できます。 これらのレポートは、Office サブスクリプションをアクティブ化するために追加サポートが必要なユーザーの識別に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 5ecf1aeb0014ec8ead97fc7d1b01d366c9565291
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035988"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="7976e-105">Office 365 アクティブ化レポート</span><span class="sxs-lookup"><span data-stu-id="7976e-105">Office 365 activations reports</span></span>

<span data-ttu-id="7976e-106">Office 365 アクティブ化レポートでは、1 つ以上のデバイスで Office 365 サブスクリプションをアクティブ化したユーザーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="7976e-106">The Office 365 activation reports can give you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="7976e-107">これらのレポートでは、Office 365 ProPlus、Project、Visio Pro for Office 365 のサブスクリプションのアクティブ化の詳細、およびデスクトップとデバイス全体にわたるアクティブ化の詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="7976e-107">These reports provide a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="7976e-108">これらのレポートは、Office サブスクリプションをアクティブ化するために追加サポートが必要なユーザーの識別に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="7976e-108">These reports could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="7976e-109">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7976e-109">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="7976e-110">レポート</span><span class="sxs-lookup"><span data-stu-id="7976e-110">Reports</span></span>
| <span data-ttu-id="7976e-111">関数</span><span class="sxs-lookup"><span data-stu-id="7976e-111">Function</span></span>                                 | <span data-ttu-id="7976e-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7976e-112">Return Type</span></span> | <span data-ttu-id="7976e-113">説明</span><span class="sxs-lookup"><span data-stu-id="7976e-113">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="7976e-114">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="7976e-114">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="7976e-115">ストリーム</span><span class="sxs-lookup"><span data-stu-id="7976e-115">Stream</span></span>      | <span data-ttu-id="7976e-116">Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="7976e-116">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="7976e-117">ライセンス認証の数を取得する</span><span class="sxs-lookup"><span data-stu-id="7976e-117">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="7976e-118">Stream</span><span class="sxs-lookup"><span data-stu-id="7976e-118">Stream</span></span>      | <span data-ttu-id="7976e-119">デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。</span><span class="sxs-lookup"><span data-stu-id="7976e-119">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="7976e-120">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="7976e-120">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="7976e-121">Stream</span><span class="sxs-lookup"><span data-stu-id="7976e-121">Stream</span></span>      | <span data-ttu-id="7976e-122">有効なユーザーで、デスクトップまたはデバイスで Office サブスクリプションがアクティブ化されているユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="7976e-122">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
