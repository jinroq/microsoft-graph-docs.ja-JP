---
title: Skype for Business デバイス使用状況レポート
description: 組織全体にわたってクライアントと使用されているデバイスの種類の詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ad7e1b0948bf4adefe418e287a48de96440d5d47
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513243"
---
# <a name="skype-for-business-device-usage-reports"></a><span data-ttu-id="1bcfb-104">Skype for Business デバイス使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="1bcfb-104">Skype for Business device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bcfb-105">組織全体にわたってクライアントと使用されているデバイスの種類の詳細を取得できます。</span><span class="sxs-lookup"><span data-stu-id="1bcfb-105">You can get details on the types of clients and devices that are used across your organization.</span></span> <span data-ttu-id="1bcfb-106">これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1bcfb-106">These details are very helpful when you are investigating, planning, and making other business decisions for your organization.</span></span>

> <span data-ttu-id="1bcfb-107">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 使用している Skype for Business クライアント](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1bcfb-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="reports"></a><span data-ttu-id="1bcfb-108">レポート</span><span class="sxs-lookup"><span data-stu-id="1bcfb-108">Reports</span></span>

| <span data-ttu-id="1bcfb-109">関数</span><span class="sxs-lookup"><span data-stu-id="1bcfb-109">Function</span></span>                                 | <span data-ttu-id="1bcfb-110">CSV の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1bcfb-110">CSV return type</span></span> | <span data-ttu-id="1bcfb-111">JSON の戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1bcfb-111">JSON return type</span></span>                         | <span data-ttu-id="1bcfb-112">説明</span><span class="sxs-lookup"><span data-stu-id="1bcfb-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="1bcfb-113">ユーザーの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="1bcfb-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="1bcfb-114">Stream</span><span class="sxs-lookup"><span data-stu-id="1bcfb-114">Stream</span></span>          | [<span data-ttu-id="1bcfb-115">skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="1bcfb-115">skypeForBusinessDeviceUsageUserDetail</span></span>](../resources/skypeforbusinessdeviceusageuserdetail.md) | <span data-ttu-id="1bcfb-116">ユーザー別の Skype for Business デバイス使用状況に関する詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="1bcfb-116">Get details about Skype for Business device usage by user.</span></span> |
| [<span data-ttu-id="1bcfb-117">配布のユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="1bcfb-117">Get distribution user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="1bcfb-118">Stream</span><span class="sxs-lookup"><span data-stu-id="1bcfb-118">Stream</span></span>          | [<span data-ttu-id="1bcfb-119">skypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="1bcfb-119">skypeForBusinessDeviceUsageDistributionUserCounts</span></span>](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) | <span data-ttu-id="1bcfb-120">組織内でそれぞれ別個のデバイスを使用するユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="1bcfb-120">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="1bcfb-121">このレポートでは、Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad を含むデバイス別のユーザーの数を表示します。</span><span class="sxs-lookup"><span data-stu-id="1bcfb-121">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span> |
| [<span data-ttu-id="1bcfb-122">ユーザーの数を取得する</span><span class="sxs-lookup"><span data-stu-id="1bcfb-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="1bcfb-123">Stream</span><span class="sxs-lookup"><span data-stu-id="1bcfb-123">Stream</span></span>          | [<span data-ttu-id="1bcfb-124">skypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="1bcfb-124">skypeForBusinessDeviceUsageUserCounts</span></span>](../resources/skypeforbusinessdeviceusageusercounts.md) | <span data-ttu-id="1bcfb-125">Skype for Business アプリを使用して接続した組織内のユーザー数について、使用傾向を取得します。</span><span class="sxs-lookup"><span data-stu-id="1bcfb-125">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="1bcfb-126">組織内で Skype for Business クライアント アプリをインストールし、使用したデバイスの種類 (Windows、Windows スマートフォン、Android スマートフォン、iPhone、iPad) の詳細も取得できます。</span><span class="sxs-lookup"><span data-stu-id="1bcfb-126">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
