---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fd9a6cd34df322a057d16e3d803d8685f7cd173
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549383"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="7d7d7-103">certificateRevocationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="7d7d7-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="7d7d7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d7d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d7d7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d7d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d7d7-106">証明書の失効状態。</span><span class="sxs-lookup"><span data-stu-id="7d7d7-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="7d7d7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7d7d7-107">Members</span></span>
|<span data-ttu-id="7d7d7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7d7d7-108">Member</span></span>|<span data-ttu-id="7d7d7-109">値</span><span class="sxs-lookup"><span data-stu-id="7d7d7-109">Value</span></span>|<span data-ttu-id="7d7d7-110">説明</span><span class="sxs-lookup"><span data-stu-id="7d7d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d7d7-111">なし</span><span class="sxs-lookup"><span data-stu-id="7d7d7-111">none</span></span>|<span data-ttu-id="7d7d7-112">.0</span><span class="sxs-lookup"><span data-stu-id="7d7d7-112">0</span></span>|<span data-ttu-id="7d7d7-113">取り消されません。</span><span class="sxs-lookup"><span data-stu-id="7d7d7-113">Not revoked.</span></span>|
|<span data-ttu-id="7d7d7-114">対する</span><span class="sxs-lookup"><span data-stu-id="7d7d7-114">pending</span></span>|<span data-ttu-id="7d7d7-115">1 </span><span class="sxs-lookup"><span data-stu-id="7d7d7-115">1</span></span>|<span data-ttu-id="7d7d7-116">失効が保留中です。</span><span class="sxs-lookup"><span data-stu-id="7d7d7-116">Revocation pending.</span></span>|
|<span data-ttu-id="7d7d7-117">発行</span><span class="sxs-lookup"><span data-stu-id="7d7d7-117">issued</span></span>|<span data-ttu-id="7d7d7-118">2 </span><span class="sxs-lookup"><span data-stu-id="7d7d7-118">2</span></span>|<span data-ttu-id="7d7d7-119">失効コマンドが発行されました。</span><span class="sxs-lookup"><span data-stu-id="7d7d7-119">Revocation command issued.</span></span>|
|<span data-ttu-id="7d7d7-120">フェール</span><span class="sxs-lookup"><span data-stu-id="7d7d7-120">failed</span></span>|<span data-ttu-id="7d7d7-121">3 </span><span class="sxs-lookup"><span data-stu-id="7d7d7-121">3</span></span>|<span data-ttu-id="7d7d7-122">取り消しに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="7d7d7-122">Revocation failed.</span></span>|
|<span data-ttu-id="7d7d7-123">破棄</span><span class="sxs-lookup"><span data-stu-id="7d7d7-123">revoked</span></span>|<span data-ttu-id="7d7d7-124">4 </span><span class="sxs-lookup"><span data-stu-id="7d7d7-124">4</span></span>|<span data-ttu-id="7d7d7-125">破棄.</span><span class="sxs-lookup"><span data-stu-id="7d7d7-125">Revoked.</span></span>|





