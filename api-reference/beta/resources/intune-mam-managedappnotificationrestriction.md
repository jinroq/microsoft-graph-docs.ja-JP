---
title: managedAppNotificationRestriction 列挙型
description: 管理対象アプリの通知を制限する
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3de441b820f58dc728bc060291f99044c26fbd92
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002631"
---
# <a name="managedappnotificationrestriction-enum-type"></a><span data-ttu-id="ecb69-103">managedAppNotificationRestriction 列挙型</span><span class="sxs-lookup"><span data-stu-id="ecb69-103">managedAppNotificationRestriction enum type</span></span>

> <span data-ttu-id="ecb69-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecb69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecb69-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ecb69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecb69-106">管理対象アプリの通知を制限する</span><span class="sxs-lookup"><span data-stu-id="ecb69-106">Restrict managed app notification</span></span>

## <a name="members"></a><span data-ttu-id="ecb69-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ecb69-107">Members</span></span>
|<span data-ttu-id="ecb69-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ecb69-108">Member</span></span>|<span data-ttu-id="ecb69-109">値</span><span class="sxs-lookup"><span data-stu-id="ecb69-109">Value</span></span>|<span data-ttu-id="ecb69-110">説明</span><span class="sxs-lookup"><span data-stu-id="ecb69-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecb69-111">使う</span><span class="sxs-lookup"><span data-stu-id="ecb69-111">allow</span></span>|<span data-ttu-id="ecb69-112">.0</span><span class="sxs-lookup"><span data-stu-id="ecb69-112">0</span></span>|<span data-ttu-id="ecb69-113">すべての通知を共有します。</span><span class="sxs-lookup"><span data-stu-id="ecb69-113">Share all notifications.</span></span>|
|<span data-ttu-id="ecb69-114">blockOrganizationalData</span><span class="sxs-lookup"><span data-stu-id="ecb69-114">blockOrganizationalData</span></span>|<span data-ttu-id="ecb69-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ecb69-115">1</span></span>|<span data-ttu-id="ecb69-116">通知では、Orgnizational を共有しないでください。</span><span class="sxs-lookup"><span data-stu-id="ecb69-116">Do not share Orgnizational data in notifications.</span></span>|
|<span data-ttu-id="ecb69-117">拒否</span><span class="sxs-lookup"><span data-stu-id="ecb69-117">block</span></span>|<span data-ttu-id="ecb69-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ecb69-118">2</span></span>|<span data-ttu-id="ecb69-119">通知を共有しないでください。</span><span class="sxs-lookup"><span data-stu-id="ecb69-119">Do not share notifications.</span></span>|





