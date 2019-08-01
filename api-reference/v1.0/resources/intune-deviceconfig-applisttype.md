---
title: appListType 列挙型
description: コンプライアンスアプリリストの可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a02b8ed105206f53894ddb8d35dc24106eebebc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028603"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="b2f15-103">appListType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b2f15-103">appListType enum type</span></span>

> <span data-ttu-id="b2f15-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b2f15-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2f15-105">コンプライアンスアプリリストの可能な値。</span><span class="sxs-lookup"><span data-stu-id="b2f15-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="b2f15-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="b2f15-106">Members</span></span>
|<span data-ttu-id="b2f15-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b2f15-107">Member</span></span>|<span data-ttu-id="b2f15-108">値</span><span class="sxs-lookup"><span data-stu-id="b2f15-108">Value</span></span>|<span data-ttu-id="b2f15-109">説明</span><span class="sxs-lookup"><span data-stu-id="b2f15-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2f15-110">none</span><span class="sxs-lookup"><span data-stu-id="b2f15-110">none</span></span>|<span data-ttu-id="b2f15-111">.0</span><span class="sxs-lookup"><span data-stu-id="b2f15-111">0</span></span>|<span data-ttu-id="b2f15-112">既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="b2f15-112">Default value, no intent.</span></span>|
|<span data-ttu-id="b2f15-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="b2f15-113">appsInListCompliant</span></span>|<span data-ttu-id="b2f15-114">1-d</span><span class="sxs-lookup"><span data-stu-id="b2f15-114">1</span></span>|<span data-ttu-id="b2f15-115">リストは、準拠していると見なされるアプリを表します (リスト上のアプリのみが準拠しています)。</span><span class="sxs-lookup"><span data-stu-id="b2f15-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="b2f15-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="b2f15-116">appsNotInListCompliant</span></span>|<span data-ttu-id="b2f15-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b2f15-117">2</span></span>|<span data-ttu-id="b2f15-118">このリストは、非準拠と見なされるアプリを表します (すべてのアプリはリスト上のアプリ以外に準拠しています)。</span><span class="sxs-lookup"><span data-stu-id="b2f15-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



