---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6c2dd85ba053c3b1493dc598741f2417eb6c0aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412360"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="cfa79-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="cfa79-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="cfa79-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cfa79-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cfa79-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfa79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfa79-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cfa79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfa79-107">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="cfa79-107">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>

## <a name="members"></a><span data-ttu-id="cfa79-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="cfa79-108">Members</span></span>
|<span data-ttu-id="cfa79-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="cfa79-109">Member</span></span>|<span data-ttu-id="cfa79-110">値</span><span class="sxs-lookup"><span data-stu-id="cfa79-110">Value</span></span>|<span data-ttu-id="cfa79-111">説明</span><span class="sxs-lookup"><span data-stu-id="cfa79-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfa79-112">lockWorkstation</span><span class="sxs-lookup"><span data-stu-id="cfa79-112">lockWorkstation</span></span>|<span data-ttu-id="cfa79-113">0</span><span class="sxs-lookup"><span data-stu-id="cfa79-113">0</span></span>|<span data-ttu-id="cfa79-114">操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="cfa79-114">No Action</span></span>|
|<span data-ttu-id="cfa79-115">noAction</span><span class="sxs-lookup"><span data-stu-id="cfa79-115">noAction</span></span>|<span data-ttu-id="cfa79-116">1</span><span class="sxs-lookup"><span data-stu-id="cfa79-116">1</span></span>|<span data-ttu-id="cfa79-117">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="cfa79-117">Lock Workstation</span></span>|
|<span data-ttu-id="cfa79-118">forceLogoff</span><span class="sxs-lookup"><span data-stu-id="cfa79-118">forceLogoff</span></span>|<span data-ttu-id="cfa79-119">2</span><span class="sxs-lookup"><span data-stu-id="cfa79-119">2</span></span>|<span data-ttu-id="cfa79-120">ログオフを強制します。</span><span class="sxs-lookup"><span data-stu-id="cfa79-120">Force Logoff</span></span>|
|<span data-ttu-id="cfa79-121">disconnectRemoteDesktopSession</span><span class="sxs-lookup"><span data-stu-id="cfa79-121">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="cfa79-122">3</span><span class="sxs-lookup"><span data-stu-id="cfa79-122">3</span></span>|<span data-ttu-id="cfa79-123">場合、リモートのリモート デスクトップ サービス セッションを切断します。</span><span class="sxs-lookup"><span data-stu-id="cfa79-123">Disconnect if a remote Remote Desktop Services session</span></span>|




