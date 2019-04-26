---
title: メールボックス使用状況レポート
description: メールボックスと、主に電子メールの送受信に基づくアクティビティレベルのユーザーに関する情報を取得できます。 また、各メールボックスが消費するストレージの量と、ストレージのクォータに近づいているメールボックスの数も確認できます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 324f936e497142b5f8bab5ea6607005ea1c35c2b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345111"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="ce72c-104">メールボックス使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="ce72c-104">Mailbox usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce72c-105">メールボックスと、主に電子メールの送受信に基づくアクティビティレベルのユーザーに関する情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="ce72c-105">You can get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="ce72c-106">また、各メールボックスが消費するストレージの量と、ストレージのクォータに近づいているメールボックスの数も確認できます。</span><span class="sxs-lookup"><span data-stu-id="ce72c-106">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="ce72c-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce72c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="ce72c-108">レポート</span><span class="sxs-lookup"><span data-stu-id="ce72c-108">Reports</span></span>

| <span data-ttu-id="ce72c-109">関数</span><span class="sxs-lookup"><span data-stu-id="ce72c-109">Function</span></span>                                 | <span data-ttu-id="ce72c-110">CSV 戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ce72c-110">CSV return type</span></span> | <span data-ttu-id="ce72c-111">JSON 戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="ce72c-111">JSON return type</span></span>                         | <span data-ttu-id="ce72c-112">説明</span><span class="sxs-lookup"><span data-stu-id="ce72c-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ce72c-113">メールボックスの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="ce72c-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="ce72c-114">Stream</span><span class="sxs-lookup"><span data-stu-id="ce72c-114">Stream</span></span>          | [<span data-ttu-id="ce72c-115">mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="ce72c-115">mailboxUsageDetail</span></span>](../resources/mailboxusagedetail.md) | <span data-ttu-id="ce72c-116">メールボックスの使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce72c-116">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="ce72c-117">メールボックスの数を取得する</span><span class="sxs-lookup"><span data-stu-id="ce72c-117">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="ce72c-118">Stream</span><span class="sxs-lookup"><span data-stu-id="ce72c-118">Stream</span></span>          | [<span data-ttu-id="ce72c-119">mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="ce72c-119">mailboxUsageMailboxCounts</span></span>](../resources/mailboxusagemailboxcounts.md) | <span data-ttu-id="ce72c-120">組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce72c-120">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="ce72c-121">メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="ce72c-121">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="ce72c-122">クォータ状態のメールボックスの数を取得する</span><span class="sxs-lookup"><span data-stu-id="ce72c-122">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="ce72c-123">Stream</span><span class="sxs-lookup"><span data-stu-id="ce72c-123">Stream</span></span>          | [<span data-ttu-id="ce72c-124">mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="ce72c-124">mailboxUsageQuotaStatusMailboxCounts</span></span>](../resources/mailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="ce72c-125">各クォータ カテゴリのユーザーのメールボックス数を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce72c-125">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="ce72c-126">ストレージを取得する</span><span class="sxs-lookup"><span data-stu-id="ce72c-126">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="ce72c-127">Stream</span><span class="sxs-lookup"><span data-stu-id="ce72c-127">Stream</span></span>          | [<span data-ttu-id="ce72c-128">mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="ce72c-128">mailboxUsageStorage</span></span>](../resources/mailboxusagestorage.md) | <span data-ttu-id="ce72c-129">組織で使用されているストレージの量を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce72c-129">Get the amount of storage used in your organization.</span></span> |
