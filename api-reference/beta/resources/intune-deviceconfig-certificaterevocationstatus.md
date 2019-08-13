---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68f510771370e5be95a8360526d0058ff8c307b1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333703"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="078af-103">certificateRevocationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="078af-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="078af-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="078af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="078af-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="078af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="078af-106">証明書の失効状態。</span><span class="sxs-lookup"><span data-stu-id="078af-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="078af-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="078af-107">Members</span></span>
|<span data-ttu-id="078af-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="078af-108">Member</span></span>|<span data-ttu-id="078af-109">値</span><span class="sxs-lookup"><span data-stu-id="078af-109">Value</span></span>|<span data-ttu-id="078af-110">説明</span><span class="sxs-lookup"><span data-stu-id="078af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="078af-111">none</span><span class="sxs-lookup"><span data-stu-id="078af-111">none</span></span>|<span data-ttu-id="078af-112">.0</span><span class="sxs-lookup"><span data-stu-id="078af-112">0</span></span>|<span data-ttu-id="078af-113">取り消されません。</span><span class="sxs-lookup"><span data-stu-id="078af-113">Not revoked.</span></span>|
|<span data-ttu-id="078af-114">対する</span><span class="sxs-lookup"><span data-stu-id="078af-114">pending</span></span>|<span data-ttu-id="078af-115">1-d</span><span class="sxs-lookup"><span data-stu-id="078af-115">1</span></span>|<span data-ttu-id="078af-116">失効が保留中です。</span><span class="sxs-lookup"><span data-stu-id="078af-116">Revocation pending.</span></span>|
|<span data-ttu-id="078af-117">発行</span><span class="sxs-lookup"><span data-stu-id="078af-117">issued</span></span>|<span data-ttu-id="078af-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="078af-118">2</span></span>|<span data-ttu-id="078af-119">失効コマンドが発行されました。</span><span class="sxs-lookup"><span data-stu-id="078af-119">Revocation command issued.</span></span>|
|<span data-ttu-id="078af-120">フェール</span><span class="sxs-lookup"><span data-stu-id="078af-120">failed</span></span>|<span data-ttu-id="078af-121">1/3</span><span class="sxs-lookup"><span data-stu-id="078af-121">3</span></span>|<span data-ttu-id="078af-122">取り消しに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="078af-122">Revocation failed.</span></span>|
|<span data-ttu-id="078af-123">破棄</span><span class="sxs-lookup"><span data-stu-id="078af-123">revoked</span></span>|<span data-ttu-id="078af-124">2/4</span><span class="sxs-lookup"><span data-stu-id="078af-124">4</span></span>|<span data-ttu-id="078af-125">破棄.</span><span class="sxs-lookup"><span data-stu-id="078af-125">Revoked.</span></span>|



