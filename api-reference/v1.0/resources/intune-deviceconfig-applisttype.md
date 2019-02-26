---
title: applisttype 列挙型
description: コンプライアンスアプリリストの可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379ec2e10e68d62353875cd2b49c0944fe11f4da
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254325"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="e4c26-103">applisttype 列挙型</span><span class="sxs-lookup"><span data-stu-id="e4c26-103">appListType enum type</span></span>

> <span data-ttu-id="e4c26-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e4c26-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4c26-105">コンプライアンスアプリリストの可能な値。</span><span class="sxs-lookup"><span data-stu-id="e4c26-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="e4c26-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e4c26-106">Members</span></span>
|<span data-ttu-id="e4c26-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e4c26-107">Member</span></span>|<span data-ttu-id="e4c26-108">値</span><span class="sxs-lookup"><span data-stu-id="e4c26-108">Value</span></span>|<span data-ttu-id="e4c26-109">説明</span><span class="sxs-lookup"><span data-stu-id="e4c26-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4c26-110">none</span><span class="sxs-lookup"><span data-stu-id="e4c26-110">none</span></span>|<span data-ttu-id="e4c26-111">.0</span><span class="sxs-lookup"><span data-stu-id="e4c26-111">0</span></span>|<span data-ttu-id="e4c26-112">既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="e4c26-112">Default value, no intent.</span></span>|
|<span data-ttu-id="e4c26-113">appsinlistcompliant</span><span class="sxs-lookup"><span data-stu-id="e4c26-113">appsInListCompliant</span></span>|<span data-ttu-id="e4c26-114">1-d</span><span class="sxs-lookup"><span data-stu-id="e4c26-114">1</span></span>|<span data-ttu-id="e4c26-115">リストは、準拠していると見なされるアプリを表します (リスト上のアプリのみが準拠しています)。</span><span class="sxs-lookup"><span data-stu-id="e4c26-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="e4c26-116">appsnotinlistcompliant</span><span class="sxs-lookup"><span data-stu-id="e4c26-116">appsNotInListCompliant</span></span>|<span data-ttu-id="e4c26-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e4c26-117">2</span></span>|<span data-ttu-id="e4c26-118">このリストは、非準拠と見なされるアプリを表します (すべてのアプリはリスト上のアプリ以外に準拠しています)。</span><span class="sxs-lookup"><span data-stu-id="e4c26-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



