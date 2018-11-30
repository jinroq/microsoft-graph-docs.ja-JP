---
title: メールボックス使用状況レポート
description: メールボックス使用状況レポートを使用して、主に電子メールの送受信に基づき、メールボックスを持つユーザーの情報と、そのアクティビティのレベルを取得します。 また、各メールボックスが消費するストレージの量と、ストレージのクォータに近づいているメールボックスの数も確認できます。
ms.openlocfilehash: 6ebaa1e829d4f97f8fa354a42a175a8f392e0c69
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022466"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="e7c6b-104">メールボックス使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="e7c6b-104">Mailbox usage reports</span></span>

<span data-ttu-id="e7c6b-105">メールボックス使用状況レポートを使用して、主に電子メールの送受信に基づき、メールボックスを持つユーザーの情報と、そのアクティビティのレベルを取得します。</span><span class="sxs-lookup"><span data-stu-id="e7c6b-105">Use the mailbox usage reports to get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="e7c6b-106">また、各メールボックスが消費するストレージの量と、ストレージのクォータに近づいているメールボックスの数も確認できます。</span><span class="sxs-lookup"><span data-stu-id="e7c6b-106">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="e7c6b-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7c6b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="e7c6b-108">レポート</span><span class="sxs-lookup"><span data-stu-id="e7c6b-108">Reports</span></span>

| <span data-ttu-id="e7c6b-109">関数</span><span class="sxs-lookup"><span data-stu-id="e7c6b-109">Function</span></span>                                 | <span data-ttu-id="e7c6b-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e7c6b-110">Return Type</span></span> | <span data-ttu-id="e7c6b-111">説明</span><span class="sxs-lookup"><span data-stu-id="e7c6b-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="e7c6b-112">メールボックスの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="e7c6b-112">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="e7c6b-113">Stream</span><span class="sxs-lookup"><span data-stu-id="e7c6b-113">Stream</span></span>      | <span data-ttu-id="e7c6b-114">メールボックスの使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="e7c6b-114">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="e7c6b-115">メールボックスの数を取得する</span><span class="sxs-lookup"><span data-stu-id="e7c6b-115">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="e7c6b-116">Stream</span><span class="sxs-lookup"><span data-stu-id="e7c6b-116">Stream</span></span>      | <span data-ttu-id="e7c6b-117">組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e7c6b-117">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="e7c6b-118">メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。</span><span class="sxs-lookup"><span data-stu-id="e7c6b-118">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="e7c6b-119">クォータ状態のメールボックスの数を取得する</span><span class="sxs-lookup"><span data-stu-id="e7c6b-119">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="e7c6b-120">Stream</span><span class="sxs-lookup"><span data-stu-id="e7c6b-120">Stream</span></span>      | <span data-ttu-id="e7c6b-121">各クォータ カテゴリのユーザーのメールボックス数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e7c6b-121">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="e7c6b-122">ストレージを取得する</span><span class="sxs-lookup"><span data-stu-id="e7c6b-122">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="e7c6b-123">Stream</span><span class="sxs-lookup"><span data-stu-id="e7c6b-123">Stream</span></span>      | <span data-ttu-id="e7c6b-124">組織で使用されているストレージの量を取得します。</span><span class="sxs-lookup"><span data-stu-id="e7c6b-124">Get the amount of storage used in your organization.</span></span> |
