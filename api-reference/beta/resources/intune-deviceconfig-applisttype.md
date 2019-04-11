---
title: applisttype 列挙型
description: コンプライアンスアプリリストの可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a05fc37f692d58a4d5d434037fd9d1ebe09ecaa9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798727"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="a21bd-103">applisttype 列挙型</span><span class="sxs-lookup"><span data-stu-id="a21bd-103">appListType enum type</span></span>

> <span data-ttu-id="a21bd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a21bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a21bd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a21bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a21bd-106">コンプライアンスアプリリストの可能な値。</span><span class="sxs-lookup"><span data-stu-id="a21bd-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="a21bd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a21bd-107">Members</span></span>
|<span data-ttu-id="a21bd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a21bd-108">Member</span></span>|<span data-ttu-id="a21bd-109">値</span><span class="sxs-lookup"><span data-stu-id="a21bd-109">Value</span></span>|<span data-ttu-id="a21bd-110">説明</span><span class="sxs-lookup"><span data-stu-id="a21bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a21bd-111">none</span><span class="sxs-lookup"><span data-stu-id="a21bd-111">none</span></span>|<span data-ttu-id="a21bd-112">.0</span><span class="sxs-lookup"><span data-stu-id="a21bd-112">0</span></span>|<span data-ttu-id="a21bd-113">既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="a21bd-113">Default value, no intent.</span></span>|
|<span data-ttu-id="a21bd-114">appsinlistcompliant</span><span class="sxs-lookup"><span data-stu-id="a21bd-114">appsInListCompliant</span></span>|<span data-ttu-id="a21bd-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a21bd-115">1</span></span>|<span data-ttu-id="a21bd-116">リストは、準拠していると見なされるアプリを表します (リスト上のアプリのみが準拠しています)。</span><span class="sxs-lookup"><span data-stu-id="a21bd-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="a21bd-117">appsnotinlistcompliant</span><span class="sxs-lookup"><span data-stu-id="a21bd-117">appsNotInListCompliant</span></span>|<span data-ttu-id="a21bd-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a21bd-118">2</span></span>|<span data-ttu-id="a21bd-119">このリストは、非準拠と見なされるアプリを表します (すべてのアプリはリスト上のアプリ以外に準拠しています)。</span><span class="sxs-lookup"><span data-stu-id="a21bd-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





