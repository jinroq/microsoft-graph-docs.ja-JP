---
title: Microsoft Intune での通信経費の管理
description: Intune と統合している、Saaswedo 通信経費管理サービスを使用すると、会社所有のデバイスでのデータの使用とローミングを制限することができます。 このサービスを使用すると、使用制限を設定および適用し、構成済みのしきい値を超えた場合にユーザーにアラートを送信できます。 また、ユーザーがしきい値を超えた場合にローミングを無効にするなど、さまざまな処理を行うようにサービスを構成することもできます。 Saaswedo コンソールでは、データの使用状況と監視情報を提供するレポートを利用することができます。 Intune で Saaswedo 通信経費管理サービスを使用する前に、Saaswedo コンソールと Intune で設定を構成する必要があります。 Saaswedo サービスおよび Intune に対する接続はオンにする必要があります。 Saaswedo 側の接続が有効で Intune 側の接続が有効でない場合、Intune 側は通信を受信しますが、それを無視します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: b2d581c6c10a1782a1b75be37f7b040f3c9dbd3b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036814"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="89724-109">Microsoft Intune での通信経費の管理</span><span class="sxs-lookup"><span data-stu-id="89724-109">Telecom expense management in Microsoft Intune</span></span>

> <span data-ttu-id="89724-110">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="89724-110">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="89724-111">Intune と統合している、Saaswedo 通信経費管理サービスを使用すると、会社所有のデバイスでのデータの使用とローミングを制限することができます。</span><span class="sxs-lookup"><span data-stu-id="89724-111">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="89724-112">このサービスを使用すると、使用制限を設定および適用し、構成済みのしきい値を超えた場合にユーザーにアラートを送信できます。</span><span class="sxs-lookup"><span data-stu-id="89724-112">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="89724-113">また、ユーザーがしきい値を超えた場合にローミングを無効にするなど、さまざまな処理を行うようにサービスを構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="89724-113">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="89724-114">Saaswedo コンソールでは、データの使用状況と監視情報を提供するレポートを利用することができます。</span><span class="sxs-lookup"><span data-stu-id="89724-114">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="89724-115">Intune で Saaswedo 通信経費管理サービスを使用する前に、Saaswedo コンソールと Intune で設定を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="89724-115">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="89724-116">Saaswedo サービスおよび Intune に対する接続はオンにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="89724-116">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="89724-117">Saaswedo 側の接続が有効で Intune 側の接続が有効でない場合、Intune 側は通信を受信しますが、それを無視します。</span><span class="sxs-lookup"><span data-stu-id="89724-117">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="89724-118">次の Graph リソースを使用して、Intune での通信費を管理できます。</span><span class="sxs-lookup"><span data-stu-id="89724-118">The following Graph resources are available to manage telecom expenses in Intune:</span></span>  

- [<span data-ttu-id="89724-119">通信経費の管理パートナー</span><span class="sxs-lookup"><span data-stu-id="89724-119">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)
