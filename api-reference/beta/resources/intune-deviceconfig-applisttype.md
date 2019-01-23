---
title: appListType 列挙型
description: 準拠のアプリケーションのリストで使用できる値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf8930136b00b7b5579ec5e7266b6a77a9a11968
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415223"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="3e433-103">appListType 列挙型</span><span class="sxs-lookup"><span data-stu-id="3e433-103">appListType enum type</span></span>

> <span data-ttu-id="3e433-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3e433-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e433-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e433-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e433-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3e433-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e433-107">準拠のアプリケーションのリストで使用できる値です。</span><span class="sxs-lookup"><span data-stu-id="3e433-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="3e433-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3e433-108">Members</span></span>
|<span data-ttu-id="3e433-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="3e433-109">Member</span></span>|<span data-ttu-id="3e433-110">値</span><span class="sxs-lookup"><span data-stu-id="3e433-110">Value</span></span>|<span data-ttu-id="3e433-111">説明</span><span class="sxs-lookup"><span data-stu-id="3e433-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e433-112">none</span><span class="sxs-lookup"><span data-stu-id="3e433-112">none</span></span>|<span data-ttu-id="3e433-113">0</span><span class="sxs-lookup"><span data-stu-id="3e433-113">0</span></span>|<span data-ttu-id="3e433-114">既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="3e433-114">Default value, no intent.</span></span>|
|<span data-ttu-id="3e433-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="3e433-115">appsInListCompliant</span></span>|<span data-ttu-id="3e433-116">1</span><span class="sxs-lookup"><span data-stu-id="3e433-116">1</span></span>|<span data-ttu-id="3e433-117">一覧は、考慮される準拠 (準拠では、リスト上のアプリ) 専用のアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="3e433-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="3e433-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="3e433-118">appsNotInListCompliant</span></span>|<span data-ttu-id="3e433-119">2</span><span class="sxs-lookup"><span data-stu-id="3e433-119">2</span></span>|<span data-ttu-id="3e433-120">リストと見なされます非準拠のアプリケーションを表します (すべてのアプリケーション準拠では、リスト上のアプリを除く)。</span><span class="sxs-lookup"><span data-stu-id="3e433-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




