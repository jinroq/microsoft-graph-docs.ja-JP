---
title: administratorConfiguredDeviceComplianceState 列挙型
description: 管理者には、デバイス準拠状態の列挙型が構成されています。
author: tfitzmac
ms.openlocfilehash: e1b76c40f0e5f815e42efa0a4fef776aeb3e0b00
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314869"
---
# <a name="administratorconfigureddevicecompliancestate-enum-type"></a><span data-ttu-id="202b5-103">administratorConfiguredDeviceComplianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="202b5-103">administratorConfiguredDeviceComplianceState enum type</span></span>

> <span data-ttu-id="202b5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="202b5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="202b5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="202b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="202b5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="202b5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="202b5-107">管理者には、デバイス準拠状態の列挙型が構成されています。</span><span class="sxs-lookup"><span data-stu-id="202b5-107">Administrator configured device compliance state Enum</span></span>
## <a name="members"></a><span data-ttu-id="202b5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="202b5-108">Members</span></span>
|<span data-ttu-id="202b5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="202b5-109">Member</span></span>|<span data-ttu-id="202b5-110">値</span><span class="sxs-lookup"><span data-stu-id="202b5-110">Value</span></span>|<span data-ttu-id="202b5-111">説明</span><span class="sxs-lookup"><span data-stu-id="202b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="202b5-112">basedOnDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="202b5-112">basedOnDeviceCompliancePolicy</span></span>|<span data-ttu-id="202b5-113">0</span><span class="sxs-lookup"><span data-stu-id="202b5-113">0</span></span>|<span data-ttu-id="202b5-114">ポリシーの他のコンプライアンスに基づくコンプライアンスの状態を設定します。</span><span class="sxs-lookup"><span data-stu-id="202b5-114">Set compliance state based on other compliance polices</span></span>|
|<span data-ttu-id="202b5-115">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="202b5-115">nonCompliant</span></span>|<span data-ttu-id="202b5-116">1</span><span class="sxs-lookup"><span data-stu-id="202b5-116">1</span></span>|<span data-ttu-id="202b5-117">一連のコンプライアンスに準拠していません。</span><span class="sxs-lookup"><span data-stu-id="202b5-117">Set compliance to nonCompliant</span></span>|





