---
title: Devicemanagementdomainjoinコネクタ状態列挙型
description: ODJ 要求の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f664a6b57d92f5a8cd2d586f8bc2747ffa6db71c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342006"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="61e07-103">Devicemanagementdomainjoinコネクタ状態列挙型</span><span class="sxs-lookup"><span data-stu-id="61e07-103">deviceManagementDomainJoinConnectorState enum type</span></span>

> <span data-ttu-id="61e07-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61e07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61e07-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="61e07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61e07-106">ODJ 要求の状態。</span><span class="sxs-lookup"><span data-stu-id="61e07-106">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="61e07-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="61e07-107">Members</span></span>
|<span data-ttu-id="61e07-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="61e07-108">Member</span></span>|<span data-ttu-id="61e07-109">値</span><span class="sxs-lookup"><span data-stu-id="61e07-109">Value</span></span>|<span data-ttu-id="61e07-110">説明</span><span class="sxs-lookup"><span data-stu-id="61e07-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61e07-111">active</span><span class="sxs-lookup"><span data-stu-id="61e07-111">active</span></span>|<span data-ttu-id="61e07-112">.0</span><span class="sxs-lookup"><span data-stu-id="61e07-112">0</span></span>|<span data-ttu-id="61e07-113">コネクタは、アクティブな Intune に ping を行います。</span><span class="sxs-lookup"><span data-stu-id="61e07-113">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="61e07-114">error</span><span class="sxs-lookup"><span data-stu-id="61e07-114">error</span></span>|<span data-ttu-id="61e07-115">1-d</span><span class="sxs-lookup"><span data-stu-id="61e07-115">1</span></span>|<span data-ttu-id="61e07-116">過去1時間のコネクタからのハートビートはありません。</span><span class="sxs-lookup"><span data-stu-id="61e07-116">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="61e07-117">未使用</span><span class="sxs-lookup"><span data-stu-id="61e07-117">inactive</span></span>|<span data-ttu-id="61e07-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="61e07-118">2</span></span>|<span data-ttu-id="61e07-119">過去5日間のコネクタからのハートビートはありません。</span><span class="sxs-lookup"><span data-stu-id="61e07-119">There is no heart-beat from connector from last 5 days.</span></span>|



