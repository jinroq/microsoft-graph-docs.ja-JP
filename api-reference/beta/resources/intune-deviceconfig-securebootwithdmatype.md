---
title: secureBootWithDMAType 列挙型
description: DMA を使用したセキュアブートの可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2cffc336503fa683b622540bbf7f941df3bef249
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001749"
---
# <a name="securebootwithdmatype-enum-type"></a><span data-ttu-id="05b4c-103">secureBootWithDMAType 列挙型</span><span class="sxs-lookup"><span data-stu-id="05b4c-103">secureBootWithDMAType enum type</span></span>

> <span data-ttu-id="05b4c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05b4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05b4c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="05b4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05b4c-106">DMA を使用したセキュアブートの可能な値</span><span class="sxs-lookup"><span data-stu-id="05b4c-106">Possible values of Secure Boot with DMA</span></span>

## <a name="members"></a><span data-ttu-id="05b4c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="05b4c-107">Members</span></span>
|<span data-ttu-id="05b4c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="05b4c-108">Member</span></span>|<span data-ttu-id="05b4c-109">値</span><span class="sxs-lookup"><span data-stu-id="05b4c-109">Value</span></span>|<span data-ttu-id="05b4c-110">説明</span><span class="sxs-lookup"><span data-stu-id="05b4c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05b4c-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="05b4c-111">notConfigured</span></span>|<span data-ttu-id="05b4c-112">.0</span><span class="sxs-lookup"><span data-stu-id="05b4c-112">0</span></span>|<span data-ttu-id="05b4c-113">未構成、操作なし</span><span class="sxs-lookup"><span data-stu-id="05b4c-113">Not configured, no operation</span></span>|
|<span data-ttu-id="05b4c-114">Dma なし</span><span class="sxs-lookup"><span data-stu-id="05b4c-114">withoutDMA</span></span>|<span data-ttu-id="05b4c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="05b4c-115">1</span></span>|<span data-ttu-id="05b4c-116">セキュアブートを使用して VBS を有効にする</span><span class="sxs-lookup"><span data-stu-id="05b4c-116">Turns on VBS with Secure Boot</span></span>|
|<span data-ttu-id="05b4c-117">withDMA</span><span class="sxs-lookup"><span data-stu-id="05b4c-117">withDMA</span></span>|<span data-ttu-id="05b4c-118">1/3</span><span class="sxs-lookup"><span data-stu-id="05b4c-118">3</span></span>|<span data-ttu-id="05b4c-119">セキュリティで保護されたブートと DMA を使用して VBS を有効にする</span><span class="sxs-lookup"><span data-stu-id="05b4c-119">Turns on VBS with Secure Boot and DMA</span></span>|





