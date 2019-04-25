---
title: Skype for Business デバイス使用状況レポート
description: Skype for Business デバイス使用状況レポートを使用すると、組織全体で使用されているクライアントやデバイスの種類の詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8eb1f5896a261610eb5400611a78f5ac75952256
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565899"
---
# <a name="skype-for-business-device-usage-reports"></a><span data-ttu-id="fe4c6-104">Skype for Business デバイス使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="fe4c6-104">Skype for Business device usage reports</span></span>

<span data-ttu-id="fe4c6-105">Skype for Business デバイス使用状況レポートを使用すると、組織全体で使用されているクライアントやデバイスの種類の詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="fe4c6-105">You can use the Skype for Business device usage reports to get details on the types of clients and devices that are used across your organization.</span></span> <span data-ttu-id="fe4c6-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="fe4c6-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="fe4c6-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe4c6-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="reports"></a><span data-ttu-id="fe4c6-108">レポート</span><span class="sxs-lookup"><span data-stu-id="fe4c6-108">Reports</span></span>

| <span data-ttu-id="fe4c6-109">関数</span><span class="sxs-lookup"><span data-stu-id="fe4c6-109">Function</span></span>                                 | <span data-ttu-id="fe4c6-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fe4c6-110">Return Type</span></span> | <span data-ttu-id="fe4c6-111">説明</span><span class="sxs-lookup"><span data-stu-id="fe4c6-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="fe4c6-112">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="fe4c6-112">Get user detail</span></span>](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="fe4c6-113">Stream</span><span class="sxs-lookup"><span data-stu-id="fe4c6-113">Stream</span></span>      | <span data-ttu-id="fe4c6-114">ユーザー別の Skype for Business デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="fe4c6-114">Get details about Skype for Business device usage by user.</span></span> |
| [<span data-ttu-id="fe4c6-115">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="fe4c6-115">Get distribution user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="fe4c6-116">Stream</span><span class="sxs-lookup"><span data-stu-id="fe4c6-116">Stream</span></span>      | <span data-ttu-id="fe4c6-117">組織内でそれぞれ別個のデバイスを使用するユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="fe4c6-117">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="fe4c6-118">このレポートでは、Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad を含むデバイス別のユーザーの数を表示します。</span><span class="sxs-lookup"><span data-stu-id="fe4c6-118">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span> |
| [<span data-ttu-id="fe4c6-119">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="fe4c6-119">Get user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="fe4c6-120">Stream</span><span class="sxs-lookup"><span data-stu-id="fe4c6-120">Stream</span></span>      | <span data-ttu-id="fe4c6-121">Skype for Business アプリを使用して接続した組織内のユーザー数について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="fe4c6-121">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="fe4c6-122">組織内で Skype for Business クライアント アプリをインストールし、使用したデバイスの種類 (Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad) の詳細も取得できます。</span><span class="sxs-lookup"><span data-stu-id="fe4c6-122">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span> |
