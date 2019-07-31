---
title: win32LobAppRegistryDetectionType 列挙型
description: サポートされているすべてのレジストリデータ検出の種類が含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 45f961236363f25205763a3d9765453fc8760ad5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012234"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a><span data-ttu-id="a50b7-103">win32LobAppRegistryDetectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a50b7-103">win32LobAppRegistryDetectionType enum type</span></span>

> <span data-ttu-id="a50b7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a50b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a50b7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a50b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a50b7-106">サポートされているすべてのレジストリデータ検出の種類が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a50b7-106">Contains all supported registry data detection type.</span></span>

## <a name="members"></a><span data-ttu-id="a50b7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a50b7-107">Members</span></span>
|<span data-ttu-id="a50b7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a50b7-108">Member</span></span>|<span data-ttu-id="a50b7-109">値</span><span class="sxs-lookup"><span data-stu-id="a50b7-109">Value</span></span>|<span data-ttu-id="a50b7-110">説明</span><span class="sxs-lookup"><span data-stu-id="a50b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a50b7-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a50b7-111">notConfigured</span></span>|<span data-ttu-id="a50b7-112">.0</span><span class="sxs-lookup"><span data-stu-id="a50b7-112">0</span></span>|<span data-ttu-id="a50b7-113">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="a50b7-113">Not configured.</span></span>|
|<span data-ttu-id="a50b7-114">ある</span><span class="sxs-lookup"><span data-stu-id="a50b7-114">exists</span></span>|<span data-ttu-id="a50b7-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a50b7-115">1</span></span>|<span data-ttu-id="a50b7-116">指定されたレジストリキーまたは値が存在します。</span><span class="sxs-lookup"><span data-stu-id="a50b7-116">The specified registry key or value exists.</span></span>|
|<span data-ttu-id="a50b7-117">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="a50b7-117">doesNotExist</span></span>|<span data-ttu-id="a50b7-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a50b7-118">2</span></span>|<span data-ttu-id="a50b7-119">指定したレジストリキーまたは値が存在しません。</span><span class="sxs-lookup"><span data-stu-id="a50b7-119">The specified registry key or value does not exist.</span></span>|
|<span data-ttu-id="a50b7-120">string</span><span class="sxs-lookup"><span data-stu-id="a50b7-120">string</span></span>|<span data-ttu-id="a50b7-121">1/3</span><span class="sxs-lookup"><span data-stu-id="a50b7-121">3</span></span>|<span data-ttu-id="a50b7-122">文字列型 (String) の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a50b7-122">String value type.</span></span>|
|<span data-ttu-id="a50b7-123">整数</span><span class="sxs-lookup"><span data-stu-id="a50b7-123">integer</span></span>|<span data-ttu-id="a50b7-124">2/4</span><span class="sxs-lookup"><span data-stu-id="a50b7-124">4</span></span>|<span data-ttu-id="a50b7-125">整数型 (Integer) の値です。</span><span class="sxs-lookup"><span data-stu-id="a50b7-125">Integer value type.</span></span>|
|<span data-ttu-id="a50b7-126">バージョン</span><span class="sxs-lookup"><span data-stu-id="a50b7-126">version</span></span>|<span data-ttu-id="a50b7-127">5</span><span class="sxs-lookup"><span data-stu-id="a50b7-127">5</span></span>|<span data-ttu-id="a50b7-128">バージョン値の種類。</span><span class="sxs-lookup"><span data-stu-id="a50b7-128">Version value type.</span></span>|





