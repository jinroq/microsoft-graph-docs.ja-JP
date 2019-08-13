---
title: managedAppNotificationRestriction 列挙型
description: 管理対象アプリの通知を制限する
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 78d031f4aa7b7aef5c154cc1d485fd71753855b8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332100"
---
# <a name="managedappnotificationrestriction-enum-type"></a><span data-ttu-id="0bdd3-103">managedAppNotificationRestriction 列挙型</span><span class="sxs-lookup"><span data-stu-id="0bdd3-103">managedAppNotificationRestriction enum type</span></span>

> <span data-ttu-id="0bdd3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bdd3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bdd3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0bdd3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bdd3-106">管理対象アプリの通知を制限する</span><span class="sxs-lookup"><span data-stu-id="0bdd3-106">Restrict managed app notification</span></span>

## <a name="members"></a><span data-ttu-id="0bdd3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0bdd3-107">Members</span></span>
|<span data-ttu-id="0bdd3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0bdd3-108">Member</span></span>|<span data-ttu-id="0bdd3-109">値</span><span class="sxs-lookup"><span data-stu-id="0bdd3-109">Value</span></span>|<span data-ttu-id="0bdd3-110">説明</span><span class="sxs-lookup"><span data-stu-id="0bdd3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bdd3-111">使う</span><span class="sxs-lookup"><span data-stu-id="0bdd3-111">allow</span></span>|<span data-ttu-id="0bdd3-112">.0</span><span class="sxs-lookup"><span data-stu-id="0bdd3-112">0</span></span>|<span data-ttu-id="0bdd3-113">すべての通知を共有します。</span><span class="sxs-lookup"><span data-stu-id="0bdd3-113">Share all notifications.</span></span>|
|<span data-ttu-id="0bdd3-114">blockOrganizationalData</span><span class="sxs-lookup"><span data-stu-id="0bdd3-114">blockOrganizationalData</span></span>|<span data-ttu-id="0bdd3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0bdd3-115">1</span></span>|<span data-ttu-id="0bdd3-116">通知では、Orgnizational を共有しないでください。</span><span class="sxs-lookup"><span data-stu-id="0bdd3-116">Do not share Orgnizational data in notifications.</span></span>|
|<span data-ttu-id="0bdd3-117">拒否</span><span class="sxs-lookup"><span data-stu-id="0bdd3-117">block</span></span>|<span data-ttu-id="0bdd3-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0bdd3-118">2</span></span>|<span data-ttu-id="0bdd3-119">通知を共有しないでください。</span><span class="sxs-lookup"><span data-stu-id="0bdd3-119">Do not share notifications.</span></span>|



