---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 08389dca4379b6fc0222068545ebb9bed250ba94
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863414"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="add4d-103">automaticUpdateMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="add4d-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="add4d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="add4d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="add4d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="add4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="add4d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="add4d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="add4d-107">自動更新モードを使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="add4d-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="add4d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="add4d-108">Members</span></span>
|<span data-ttu-id="add4d-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="add4d-109">Member</span></span>|<span data-ttu-id="add4d-110">値</span><span class="sxs-lookup"><span data-stu-id="add4d-110">Value</span></span>|<span data-ttu-id="add4d-111">説明</span><span class="sxs-lookup"><span data-stu-id="add4d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="add4d-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="add4d-112">userDefined</span></span>|<span data-ttu-id="add4d-113">0</span><span class="sxs-lookup"><span data-stu-id="add4d-113">0</span></span>|<span data-ttu-id="add4d-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="add4d-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="add4d-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="add4d-115">notifyDownload</span></span>|<span data-ttu-id="add4d-116">1</span><span class="sxs-lookup"><span data-stu-id="add4d-116">1</span></span>|<span data-ttu-id="add4d-117">ダウンロード時に通知します。</span><span class="sxs-lookup"><span data-stu-id="add4d-117">Notify on download.</span></span>|
|<span data-ttu-id="add4d-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="add4d-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="add4d-119">2</span><span class="sxs-lookup"><span data-stu-id="add4d-119">2</span></span>|<span data-ttu-id="add4d-120">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="add4d-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="add4d-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="add4d-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="add4d-122">3</span><span class="sxs-lookup"><span data-stu-id="add4d-122">3</span></span>|<span data-ttu-id="add4d-123">自動インストールおよびメンテナンス時に再起動します。</span><span class="sxs-lookup"><span data-stu-id="add4d-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="add4d-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="add4d-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="add4d-125">4</span><span class="sxs-lookup"><span data-stu-id="add4d-125">4</span></span>|<span data-ttu-id="add4d-126">自動インストールし、スケジュールされた時刻に再起動します。</span><span class="sxs-lookup"><span data-stu-id="add4d-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="add4d-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="add4d-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="add4d-128">5</span><span class="sxs-lookup"><span data-stu-id="add4d-128">5</span></span>|<span data-ttu-id="add4d-129">自動インストールし、エンドユーザーの制御に再起動します</span><span class="sxs-lookup"><span data-stu-id="add4d-129">Auto-install and restart without end-user control</span></span>|





