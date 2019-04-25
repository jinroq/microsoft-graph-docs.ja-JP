---
title: applisttype 列挙型
description: コンプライアンスアプリリストの可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379ec2e10e68d62353875cd2b49c0944fe11f4da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575101"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="2525c-103">applisttype 列挙型</span><span class="sxs-lookup"><span data-stu-id="2525c-103">appListType enum type</span></span>

> <span data-ttu-id="2525c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2525c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2525c-105">コンプライアンスアプリリストの可能な値。</span><span class="sxs-lookup"><span data-stu-id="2525c-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="2525c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="2525c-106">Members</span></span>
|<span data-ttu-id="2525c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2525c-107">Member</span></span>|<span data-ttu-id="2525c-108">値</span><span class="sxs-lookup"><span data-stu-id="2525c-108">Value</span></span>|<span data-ttu-id="2525c-109">説明</span><span class="sxs-lookup"><span data-stu-id="2525c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2525c-110">なし</span><span class="sxs-lookup"><span data-stu-id="2525c-110">none</span></span>|<span data-ttu-id="2525c-111">.0</span><span class="sxs-lookup"><span data-stu-id="2525c-111">0</span></span>|<span data-ttu-id="2525c-112">既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="2525c-112">Default value, no intent.</span></span>|
|<span data-ttu-id="2525c-113">appsinlistcompliant</span><span class="sxs-lookup"><span data-stu-id="2525c-113">appsInListCompliant</span></span>|<span data-ttu-id="2525c-114">1 </span><span class="sxs-lookup"><span data-stu-id="2525c-114">1</span></span>|<span data-ttu-id="2525c-115">リストは、準拠していると見なされるアプリを表します (リスト上のアプリのみが準拠しています)。</span><span class="sxs-lookup"><span data-stu-id="2525c-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="2525c-116">appsnotinlistcompliant</span><span class="sxs-lookup"><span data-stu-id="2525c-116">appsNotInListCompliant</span></span>|<span data-ttu-id="2525c-117">2 </span><span class="sxs-lookup"><span data-stu-id="2525c-117">2</span></span>|<span data-ttu-id="2525c-118">このリストは、非準拠と見なされるアプリを表します (すべてのアプリはリスト上のアプリ以外に準拠しています)。</span><span class="sxs-lookup"><span data-stu-id="2525c-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



