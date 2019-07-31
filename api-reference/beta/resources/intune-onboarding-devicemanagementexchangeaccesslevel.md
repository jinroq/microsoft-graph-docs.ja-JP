---
title: deviceManagementExchangeAccessLevel 列挙型
description: Exchange のアクセスレベル。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ec6ddbf48d7e511a05140391937c4ce079a3bbdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998157"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="99054-103">deviceManagementExchangeAccessLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="99054-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="99054-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99054-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99054-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="99054-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99054-106">Exchange のアクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="99054-106">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="99054-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="99054-107">Members</span></span>
|<span data-ttu-id="99054-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="99054-108">Member</span></span>|<span data-ttu-id="99054-109">値</span><span class="sxs-lookup"><span data-stu-id="99054-109">Value</span></span>|<span data-ttu-id="99054-110">説明</span><span class="sxs-lookup"><span data-stu-id="99054-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99054-111">none</span><span class="sxs-lookup"><span data-stu-id="99054-111">none</span></span>|<span data-ttu-id="99054-112">.0</span><span class="sxs-lookup"><span data-stu-id="99054-112">0</span></span>|<span data-ttu-id="99054-113">Exchange でデバイスアクセスルールが構成されていません。</span><span class="sxs-lookup"><span data-stu-id="99054-113">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="99054-114">使う</span><span class="sxs-lookup"><span data-stu-id="99054-114">allow</span></span>|<span data-ttu-id="99054-115">1-d</span><span class="sxs-lookup"><span data-stu-id="99054-115">1</span></span>|<span data-ttu-id="99054-116">デバイスへのアクセスを Exchange に許可します。</span><span class="sxs-lookup"><span data-stu-id="99054-116">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="99054-117">拒否</span><span class="sxs-lookup"><span data-stu-id="99054-117">block</span></span>|<span data-ttu-id="99054-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="99054-118">2</span></span>|<span data-ttu-id="99054-119">デバイスによる Exchange へのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="99054-119">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="99054-120">済み</span><span class="sxs-lookup"><span data-stu-id="99054-120">quarantine</span></span>|<span data-ttu-id="99054-121">1/3</span><span class="sxs-lookup"><span data-stu-id="99054-121">3</span></span>|<span data-ttu-id="99054-122">Exchange でデバイスを検疫します。</span><span class="sxs-lookup"><span data-stu-id="99054-122">Quarantine the device in Exchange.</span></span>|





