---
title: Yammer デバイス使用状況レポート
description: Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。 一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5067da550813f3511e82cd968ef51f605dca3d1c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521902"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="c36d3-104">Yammer デバイス使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="c36d3-104">Yammer device usage reports</span></span>

<span data-ttu-id="c36d3-105">Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="c36d3-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="c36d3-106">一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。</span><span class="sxs-lookup"><span data-stu-id="c36d3-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="c36d3-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c36d3-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="c36d3-108">レポート</span><span class="sxs-lookup"><span data-stu-id="c36d3-108">Reports</span></span>

| <span data-ttu-id="c36d3-109">関数</span><span class="sxs-lookup"><span data-stu-id="c36d3-109">Function</span></span>                                 | <span data-ttu-id="c36d3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c36d3-110">Return Type</span></span> | <span data-ttu-id="c36d3-111">説明</span><span class="sxs-lookup"><span data-stu-id="c36d3-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="c36d3-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="c36d3-112">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="c36d3-113">Stream</span><span class="sxs-lookup"><span data-stu-id="c36d3-113">Stream</span></span>      | <span data-ttu-id="c36d3-114">ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="c36d3-114">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="c36d3-115">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="c36d3-115">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="c36d3-116">Stream</span><span class="sxs-lookup"><span data-stu-id="c36d3-116">Stream</span></span>      | <span data-ttu-id="c36d3-117">デバイスの種類別にユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c36d3-117">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="c36d3-118">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="c36d3-118">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="c36d3-119">Stream</span><span class="sxs-lookup"><span data-stu-id="c36d3-119">Stream</span></span>      | <span data-ttu-id="c36d3-120">デバイスの種類別に日次ユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c36d3-120">Get the number of daily users by device type.</span></span> |
