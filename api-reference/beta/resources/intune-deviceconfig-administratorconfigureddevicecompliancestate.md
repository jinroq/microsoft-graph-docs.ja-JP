---
title: administratorConfiguredDeviceComplianceState 列挙型
description: 管理者には、デバイス準拠状態の列挙型が構成されています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dee68ef312d54410b0a1be6c97ac338c6a240916
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829135"
---
# <a name="administratorconfigureddevicecompliancestate-enum-type"></a><span data-ttu-id="c58d2-103">administratorConfiguredDeviceComplianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="c58d2-103">administratorConfiguredDeviceComplianceState enum type</span></span>

> <span data-ttu-id="c58d2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c58d2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c58d2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c58d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c58d2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c58d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c58d2-107">管理者には、デバイス準拠状態の列挙型が構成されています。</span><span class="sxs-lookup"><span data-stu-id="c58d2-107">Administrator configured device compliance state Enum</span></span>
## <a name="members"></a><span data-ttu-id="c58d2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c58d2-108">Members</span></span>
|<span data-ttu-id="c58d2-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c58d2-109">Member</span></span>|<span data-ttu-id="c58d2-110">値</span><span class="sxs-lookup"><span data-stu-id="c58d2-110">Value</span></span>|<span data-ttu-id="c58d2-111">説明</span><span class="sxs-lookup"><span data-stu-id="c58d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c58d2-112">basedOnDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c58d2-112">basedOnDeviceCompliancePolicy</span></span>|<span data-ttu-id="c58d2-113">0</span><span class="sxs-lookup"><span data-stu-id="c58d2-113">0</span></span>|<span data-ttu-id="c58d2-114">ポリシーの他のコンプライアンスに基づくコンプライアンスの状態を設定します。</span><span class="sxs-lookup"><span data-stu-id="c58d2-114">Set compliance state based on other compliance polices</span></span>|
|<span data-ttu-id="c58d2-115">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="c58d2-115">nonCompliant</span></span>|<span data-ttu-id="c58d2-116">1</span><span class="sxs-lookup"><span data-stu-id="c58d2-116">1</span></span>|<span data-ttu-id="c58d2-117">一連のコンプライアンスに準拠していません。</span><span class="sxs-lookup"><span data-stu-id="c58d2-117">Set compliance to nonCompliant</span></span>|





