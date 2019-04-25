---
title: win32LobAppRegistryDetectionType 列挙型
description: サポートされているすべてのレジストリデータ検出の種類が含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c19d2dfa0c19be1d61178c25fdd04615d2f9dbd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534424"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a><span data-ttu-id="b10f1-103">win32LobAppRegistryDetectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b10f1-103">win32LobAppRegistryDetectionType enum type</span></span>

> <span data-ttu-id="b10f1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b10f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b10f1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b10f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b10f1-106">サポートされているすべてのレジストリデータ検出の種類が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b10f1-106">Contains all supported registry data detection type.</span></span>

## <a name="members"></a><span data-ttu-id="b10f1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b10f1-107">Members</span></span>
|<span data-ttu-id="b10f1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b10f1-108">Member</span></span>|<span data-ttu-id="b10f1-109">値</span><span class="sxs-lookup"><span data-stu-id="b10f1-109">Value</span></span>|<span data-ttu-id="b10f1-110">説明</span><span class="sxs-lookup"><span data-stu-id="b10f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b10f1-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b10f1-111">notConfigured</span></span>|<span data-ttu-id="b10f1-112">.0</span><span class="sxs-lookup"><span data-stu-id="b10f1-112">0</span></span>|<span data-ttu-id="b10f1-113">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="b10f1-113">Not configured.</span></span>|
|<span data-ttu-id="b10f1-114">ある</span><span class="sxs-lookup"><span data-stu-id="b10f1-114">exists</span></span>|<span data-ttu-id="b10f1-115">1 </span><span class="sxs-lookup"><span data-stu-id="b10f1-115">1</span></span>|<span data-ttu-id="b10f1-116">指定されたレジストリキーまたは値が存在します。</span><span class="sxs-lookup"><span data-stu-id="b10f1-116">The specified registry key or value exists.</span></span>|
|<span data-ttu-id="b10f1-117">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="b10f1-117">doesNotExist</span></span>|<span data-ttu-id="b10f1-118">2 </span><span class="sxs-lookup"><span data-stu-id="b10f1-118">2</span></span>|<span data-ttu-id="b10f1-119">指定したレジストリキーまたは値が存在しません。</span><span class="sxs-lookup"><span data-stu-id="b10f1-119">The specified registry key or value does not exist.</span></span>|
|<span data-ttu-id="b10f1-120">string</span><span class="sxs-lookup"><span data-stu-id="b10f1-120">string</span></span>|<span data-ttu-id="b10f1-121">3 </span><span class="sxs-lookup"><span data-stu-id="b10f1-121">3</span></span>|<span data-ttu-id="b10f1-122">文字列型 (String) の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b10f1-122">String value type.</span></span>|
|<span data-ttu-id="b10f1-123">整数</span><span class="sxs-lookup"><span data-stu-id="b10f1-123">integer</span></span>|<span data-ttu-id="b10f1-124">4 </span><span class="sxs-lookup"><span data-stu-id="b10f1-124">4</span></span>|<span data-ttu-id="b10f1-125">整数型 (Integer) の値です。</span><span class="sxs-lookup"><span data-stu-id="b10f1-125">Integer value type.</span></span>|
|<span data-ttu-id="b10f1-126">バージョン</span><span class="sxs-lookup"><span data-stu-id="b10f1-126">version</span></span>|<span data-ttu-id="b10f1-127">5 </span><span class="sxs-lookup"><span data-stu-id="b10f1-127">5</span></span>|<span data-ttu-id="b10f1-128">バージョン値の種類。</span><span class="sxs-lookup"><span data-stu-id="b10f1-128">Version value type.</span></span>|





