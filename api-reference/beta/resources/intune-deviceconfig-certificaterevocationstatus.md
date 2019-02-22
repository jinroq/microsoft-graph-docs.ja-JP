---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c182cf2317f185108570116a283973d481f17ab2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159445"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="772c3-103">certificateRevocationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="772c3-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="772c3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="772c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="772c3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="772c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="772c3-106">証明書の失効状態。</span><span class="sxs-lookup"><span data-stu-id="772c3-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="772c3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="772c3-107">Members</span></span>
|<span data-ttu-id="772c3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="772c3-108">Member</span></span>|<span data-ttu-id="772c3-109">値</span><span class="sxs-lookup"><span data-stu-id="772c3-109">Value</span></span>|<span data-ttu-id="772c3-110">説明</span><span class="sxs-lookup"><span data-stu-id="772c3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="772c3-111">none</span><span class="sxs-lookup"><span data-stu-id="772c3-111">none</span></span>|<span data-ttu-id="772c3-112">.0</span><span class="sxs-lookup"><span data-stu-id="772c3-112">0</span></span>|<span data-ttu-id="772c3-113">取り消されません。</span><span class="sxs-lookup"><span data-stu-id="772c3-113">Not revoked.</span></span>|
|<span data-ttu-id="772c3-114">対する</span><span class="sxs-lookup"><span data-stu-id="772c3-114">pending</span></span>|<span data-ttu-id="772c3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="772c3-115">1</span></span>|<span data-ttu-id="772c3-116">失効が保留中です。</span><span class="sxs-lookup"><span data-stu-id="772c3-116">Revocation pending.</span></span>|
|<span data-ttu-id="772c3-117">発行</span><span class="sxs-lookup"><span data-stu-id="772c3-117">issued</span></span>|<span data-ttu-id="772c3-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="772c3-118">2</span></span>|<span data-ttu-id="772c3-119">失効コマンドが発行されました。</span><span class="sxs-lookup"><span data-stu-id="772c3-119">Revocation command issued.</span></span>|
|<span data-ttu-id="772c3-120">フェール</span><span class="sxs-lookup"><span data-stu-id="772c3-120">failed</span></span>|<span data-ttu-id="772c3-121">1/3</span><span class="sxs-lookup"><span data-stu-id="772c3-121">3</span></span>|<span data-ttu-id="772c3-122">取り消しに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="772c3-122">Revocation failed.</span></span>|
|<span data-ttu-id="772c3-123">破棄</span><span class="sxs-lookup"><span data-stu-id="772c3-123">revoked</span></span>|<span data-ttu-id="772c3-124">2/4</span><span class="sxs-lookup"><span data-stu-id="772c3-124">4</span></span>|<span data-ttu-id="772c3-125">破棄.</span><span class="sxs-lookup"><span data-stu-id="772c3-125">Revoked.</span></span>|




