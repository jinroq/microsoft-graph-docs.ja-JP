---
title: devicemanagementpartnertenantstate 列挙型
description: このテナントのパートナーの状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 944e9cf172bd39dd50a41e55af5fb02421d81c4f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566536"
---
# <a name="devicemanagementpartnertenantstate-enum-type"></a><span data-ttu-id="b264c-103">devicemanagementpartnertenantstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="b264c-103">deviceManagementPartnerTenantState enum type</span></span>

> <span data-ttu-id="b264c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b264c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b264c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b264c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b264c-106">このテナントのパートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="b264c-106">Partner state of this tenant.</span></span>

## <a name="members"></a><span data-ttu-id="b264c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b264c-107">Members</span></span>
|<span data-ttu-id="b264c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b264c-108">Member</span></span>|<span data-ttu-id="b264c-109">値</span><span class="sxs-lookup"><span data-stu-id="b264c-109">Value</span></span>|<span data-ttu-id="b264c-110">説明</span><span class="sxs-lookup"><span data-stu-id="b264c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b264c-111">不明</span><span class="sxs-lookup"><span data-stu-id="b264c-111">unknown</span></span>|<span data-ttu-id="b264c-112">.0</span><span class="sxs-lookup"><span data-stu-id="b264c-112">0</span></span>|<span data-ttu-id="b264c-113">パートナーの状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="b264c-113">Partner state is unknown.</span></span>|
|<span data-ttu-id="b264c-114">無効</span><span class="sxs-lookup"><span data-stu-id="b264c-114">unavailable</span></span>|<span data-ttu-id="b264c-115">1 </span><span class="sxs-lookup"><span data-stu-id="b264c-115">1</span></span>|<span data-ttu-id="b264c-116">パートナーは利用できません。</span><span class="sxs-lookup"><span data-stu-id="b264c-116">Partner is unavailable.</span></span>|
|<span data-ttu-id="b264c-117">enabled</span><span class="sxs-lookup"><span data-stu-id="b264c-117">enabled</span></span>|<span data-ttu-id="b264c-118">2 </span><span class="sxs-lookup"><span data-stu-id="b264c-118">2</span></span>|<span data-ttu-id="b264c-119">パートナーが有効になっている。</span><span class="sxs-lookup"><span data-stu-id="b264c-119">Partner is enabled.</span></span>|
|<span data-ttu-id="b264c-120">停止</span><span class="sxs-lookup"><span data-stu-id="b264c-120">terminated</span></span>|<span data-ttu-id="b264c-121">3 </span><span class="sxs-lookup"><span data-stu-id="b264c-121">3</span></span>|<span data-ttu-id="b264c-122">パートナー接続が終了します。</span><span class="sxs-lookup"><span data-stu-id="b264c-122">Partner connection is terminated.</span></span>|
|<span data-ttu-id="b264c-123">拒否</span><span class="sxs-lookup"><span data-stu-id="b264c-123">rejected</span></span>|<span data-ttu-id="b264c-124">4 </span><span class="sxs-lookup"><span data-stu-id="b264c-124">4</span></span>|<span data-ttu-id="b264c-125">パートナーメッセージは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="b264c-125">Partner messages are rejected.</span></span>|
|<span data-ttu-id="b264c-126">なかっ</span><span class="sxs-lookup"><span data-stu-id="b264c-126">unresponsive</span></span>|<span data-ttu-id="b264c-127">5 </span><span class="sxs-lookup"><span data-stu-id="b264c-127">5</span></span>|<span data-ttu-id="b264c-128">パートナーが応答していません。</span><span class="sxs-lookup"><span data-stu-id="b264c-128">Partner is unresponsive.</span></span>|





