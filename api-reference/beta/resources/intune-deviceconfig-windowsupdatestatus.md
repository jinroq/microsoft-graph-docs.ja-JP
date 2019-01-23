---
title: windowsUpdateStatus 列挙型
description: ビジネス構成のデバイスの状態の windows を更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74493359eeccdbc6df1c351ecec771b5990649b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431654"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="e24ef-103">windowsUpdateStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="e24ef-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="e24ef-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e24ef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e24ef-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e24ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e24ef-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e24ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e24ef-107">ビジネス構成のデバイスの状態の windows を更新します。</span><span class="sxs-lookup"><span data-stu-id="e24ef-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="e24ef-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e24ef-108">Members</span></span>
|<span data-ttu-id="e24ef-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e24ef-109">Member</span></span>|<span data-ttu-id="e24ef-110">値</span><span class="sxs-lookup"><span data-stu-id="e24ef-110">Value</span></span>|<span data-ttu-id="e24ef-111">説明</span><span class="sxs-lookup"><span data-stu-id="e24ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e24ef-112">古く</span><span class="sxs-lookup"><span data-stu-id="e24ef-112">upToDate</span></span>|<span data-ttu-id="e24ef-113">0</span><span class="sxs-lookup"><span data-stu-id="e24ef-113">0</span></span>|<span data-ttu-id="e24ef-114">保留中の更新プログラム、更新プログラムの再起動や障害が発生した更新保留中の不要はありません。</span><span class="sxs-lookup"><span data-stu-id="e24ef-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="e24ef-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="e24ef-115">pendingInstallation</span></span>|<span data-ttu-id="e24ef-116">1</span><span class="sxs-lookup"><span data-stu-id="e24ef-116">1</span></span>|<span data-ttu-id="e24ef-117">保留中の承認されていない更新プログラムを含むインストールの更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="e24ef-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="e24ef-118">再起動の保留中の更新はありません、ない障害が発生した更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="e24ef-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="e24ef-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="e24ef-119">pendingReboot</span></span>|<span data-ttu-id="e24ef-120">2</span><span class="sxs-lookup"><span data-stu-id="e24ef-120">2</span></span>|<span data-ttu-id="e24ef-121">再起動を必要とする更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="e24ef-121">There are updates that requires reboot.</span></span> <span data-ttu-id="e24ef-122">更新が失敗したことがありません。</span><span class="sxs-lookup"><span data-stu-id="e24ef-122">There are not failed updates.</span></span>|
|<span data-ttu-id="e24ef-123">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="e24ef-123">failed</span></span>|<span data-ttu-id="e24ef-124">3</span><span class="sxs-lookup"><span data-stu-id="e24ef-124">3</span></span>|<span data-ttu-id="e24ef-125">デバイスのインストールに失敗した更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="e24ef-125">There are updates failed to install on the device.</span></span>|




