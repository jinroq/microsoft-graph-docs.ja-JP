---
title: win32LobAppRegistryDetectionType 列挙型
description: すべて含まれているレジストリ データの検出の種類をサポートします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 188f206e42b55e0c2cc2f8b6ed831f19a4b2052a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411086"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a><span data-ttu-id="7794e-103">win32LobAppRegistryDetectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7794e-103">win32LobAppRegistryDetectionType enum type</span></span>

> <span data-ttu-id="7794e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7794e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7794e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7794e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7794e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7794e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7794e-107">すべて含まれているレジストリ データの検出の種類をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7794e-107">Contains all supported registry data detection type.</span></span>

## <a name="members"></a><span data-ttu-id="7794e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7794e-108">Members</span></span>
|<span data-ttu-id="7794e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="7794e-109">Member</span></span>|<span data-ttu-id="7794e-110">値</span><span class="sxs-lookup"><span data-stu-id="7794e-110">Value</span></span>|<span data-ttu-id="7794e-111">説明</span><span class="sxs-lookup"><span data-stu-id="7794e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7794e-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7794e-112">notConfigured</span></span>|<span data-ttu-id="7794e-113">0</span><span class="sxs-lookup"><span data-stu-id="7794e-113">0</span></span>|<span data-ttu-id="7794e-114">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="7794e-114">Not configured.</span></span>|
|<span data-ttu-id="7794e-115">存在します。</span><span class="sxs-lookup"><span data-stu-id="7794e-115">exists</span></span>|<span data-ttu-id="7794e-116">1</span><span class="sxs-lookup"><span data-stu-id="7794e-116">1</span></span>|<span data-ttu-id="7794e-117">指定したレジストリ キーまたは値が存在します。</span><span class="sxs-lookup"><span data-stu-id="7794e-117">The specified registry key or value exists.</span></span>|
|<span data-ttu-id="7794e-118">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="7794e-118">doesNotExist</span></span>|<span data-ttu-id="7794e-119">2</span><span class="sxs-lookup"><span data-stu-id="7794e-119">2</span></span>|<span data-ttu-id="7794e-120">指定したレジストリ キーまたは値が存在しません。</span><span class="sxs-lookup"><span data-stu-id="7794e-120">The specified registry key or value does not exist.</span></span>|
|<span data-ttu-id="7794e-121">string</span><span class="sxs-lookup"><span data-stu-id="7794e-121">string</span></span>|<span data-ttu-id="7794e-122">3</span><span class="sxs-lookup"><span data-stu-id="7794e-122">3</span></span>|<span data-ttu-id="7794e-123">値型の文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="7794e-123">String value type.</span></span>|
|<span data-ttu-id="7794e-124">integer</span><span class="sxs-lookup"><span data-stu-id="7794e-124">integer</span></span>|<span data-ttu-id="7794e-125">4</span><span class="sxs-lookup"><span data-stu-id="7794e-125">4</span></span>|<span data-ttu-id="7794e-126">整数値型。</span><span class="sxs-lookup"><span data-stu-id="7794e-126">Integer value type.</span></span>|
|<span data-ttu-id="7794e-127">version</span><span class="sxs-lookup"><span data-stu-id="7794e-127">version</span></span>|<span data-ttu-id="7794e-128">5</span><span class="sxs-lookup"><span data-stu-id="7794e-128">5</span></span>|<span data-ttu-id="7794e-129">バージョンの値の型。</span><span class="sxs-lookup"><span data-stu-id="7794e-129">Version value type.</span></span>|




