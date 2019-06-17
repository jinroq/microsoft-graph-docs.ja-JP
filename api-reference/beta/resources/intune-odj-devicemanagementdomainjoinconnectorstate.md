---
title: Devicemanagementdomainjoinコネクタ状態列挙型
description: ODJ 要求の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a584a77c0a921b9d5864270c5a42a9991123eb8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001917"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="0feb4-103">Devicemanagementdomainjoinコネクタ状態列挙型</span><span class="sxs-lookup"><span data-stu-id="0feb4-103">deviceManagementDomainJoinConnectorState enum type</span></span>

> <span data-ttu-id="0feb4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0feb4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0feb4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0feb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0feb4-106">ODJ 要求の状態。</span><span class="sxs-lookup"><span data-stu-id="0feb4-106">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="0feb4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0feb4-107">Members</span></span>
|<span data-ttu-id="0feb4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0feb4-108">Member</span></span>|<span data-ttu-id="0feb4-109">値</span><span class="sxs-lookup"><span data-stu-id="0feb4-109">Value</span></span>|<span data-ttu-id="0feb4-110">説明</span><span class="sxs-lookup"><span data-stu-id="0feb4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0feb4-111">active</span><span class="sxs-lookup"><span data-stu-id="0feb4-111">active</span></span>|<span data-ttu-id="0feb4-112">.0</span><span class="sxs-lookup"><span data-stu-id="0feb4-112">0</span></span>|<span data-ttu-id="0feb4-113">コネクタは、アクティブな Intune に ping を行います。</span><span class="sxs-lookup"><span data-stu-id="0feb4-113">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="0feb4-114">error</span><span class="sxs-lookup"><span data-stu-id="0feb4-114">error</span></span>|<span data-ttu-id="0feb4-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0feb4-115">1</span></span>|<span data-ttu-id="0feb4-116">過去1時間のコネクタからのハートビートはありません。</span><span class="sxs-lookup"><span data-stu-id="0feb4-116">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="0feb4-117">未使用</span><span class="sxs-lookup"><span data-stu-id="0feb4-117">inactive</span></span>|<span data-ttu-id="0feb4-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0feb4-118">2</span></span>|<span data-ttu-id="0feb4-119">過去5日間のコネクタからのハートビートはありません。</span><span class="sxs-lookup"><span data-stu-id="0feb4-119">There is no heart-beat from connector from last 5 days.</span></span>|





