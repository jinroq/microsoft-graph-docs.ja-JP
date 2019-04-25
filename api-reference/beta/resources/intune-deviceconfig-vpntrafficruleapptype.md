---
title: vpnTrafficRuleAppType 列挙型
description: VPN トラフィックルールが関連付けられているアプリの種類を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85ca96848d22dcc726bc3e79bbbe3f8518964698
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555032"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="d5e9f-103">vpnTrafficRuleAppType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d5e9f-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="d5e9f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5e9f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5e9f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5e9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5e9f-106">VPN トラフィックルールが関連付けられているアプリの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="d5e9f-106">Indicates the type of app that a VPN traffic rule is associated with.</span></span>

## <a name="members"></a><span data-ttu-id="d5e9f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5e9f-107">Members</span></span>
|<span data-ttu-id="d5e9f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5e9f-108">Member</span></span>|<span data-ttu-id="d5e9f-109">値</span><span class="sxs-lookup"><span data-stu-id="d5e9f-109">Value</span></span>|<span data-ttu-id="d5e9f-110">説明</span><span class="sxs-lookup"><span data-stu-id="d5e9f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5e9f-111">なし</span><span class="sxs-lookup"><span data-stu-id="d5e9f-111">none</span></span>|<span data-ttu-id="d5e9f-112">.0</span><span class="sxs-lookup"><span data-stu-id="d5e9f-112">0</span></span>|<span data-ttu-id="d5e9f-113">トラフィックルールがアプリに関連付けられていません。</span><span class="sxs-lookup"><span data-stu-id="d5e9f-113">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="d5e9f-114">コンピューター</span><span class="sxs-lookup"><span data-stu-id="d5e9f-114">desktop</span></span>|<span data-ttu-id="d5e9f-115">1 </span><span class="sxs-lookup"><span data-stu-id="d5e9f-115">1</span></span>|<span data-ttu-id="d5e9f-116">トラフィックルールは、デスクトップアプリに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="d5e9f-116">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="d5e9f-117">ユニバーサル</span><span class="sxs-lookup"><span data-stu-id="d5e9f-117">universal</span></span>|<span data-ttu-id="d5e9f-118">2 </span><span class="sxs-lookup"><span data-stu-id="d5e9f-118">2</span></span>|<span data-ttu-id="d5e9f-119">トラフィックルールはユニバーサルアプリに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="d5e9f-119">The traffic rule is associated with a Universal app.</span></span>|





