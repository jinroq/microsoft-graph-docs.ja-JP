---
title: Microsoft Intune での通信経費管理-Microsoft Graph API
description: テナント組織の通信経費管理に関連した Intune エンドポイント (REST) の Microsoft Graph API を一覧表示します。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 9856f01337d7ed6af6fc6df6c2e3e118b762ca0a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938619"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="24d90-103">Microsoft Intune での通信経費の管理</span><span class="sxs-lookup"><span data-stu-id="24d90-103">Telecom expense management in Microsoft Intune</span></span>

> <span data-ttu-id="24d90-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24d90-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24d90-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24d90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24d90-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24d90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="24d90-107">Intune と統合している、Saaswedo 通信経費管理サービスを使用すると、会社所有のデバイスでのデータの使用とローミングを制限することができます。</span><span class="sxs-lookup"><span data-stu-id="24d90-107">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="24d90-108">このサービスを使用すると、使用制限を設定および適用し、構成済みのしきい値を超えた場合にユーザーにアラートを送信できます。</span><span class="sxs-lookup"><span data-stu-id="24d90-108">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="24d90-109">また、ユーザーがしきい値を超えた場合にローミングを無効にするなど、さまざまな処理を行うようにサービスを構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="24d90-109">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="24d90-110">Saaswedo コンソールでは、データの使用状況と監視情報を提供するレポートを利用することができます。</span><span class="sxs-lookup"><span data-stu-id="24d90-110">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="24d90-111">Intune で Saaswedo 通信経費管理サービスを使用する前に、Saaswedo コンソールと Intune で設定を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="24d90-111">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="24d90-112">Saaswedo サービスおよび Intune に対する接続はオンにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="24d90-112">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="24d90-113">Saaswedo 側の接続が有効で Intune 側の接続が有効でない場合、Intune 側は通信を受信しますが、それを無視します。</span><span class="sxs-lookup"><span data-stu-id="24d90-113">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="24d90-114">次の Graph リソースを使用して、Intune での通信費を管理できます。</span><span class="sxs-lookup"><span data-stu-id="24d90-114">The following Graph resources are available to manage telecom expenses in Intune:</span></span>

- [<span data-ttu-id="24d90-115">通信経費の管理パートナー</span><span class="sxs-lookup"><span data-stu-id="24d90-115">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)
