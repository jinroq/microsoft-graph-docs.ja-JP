---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
ms.openlocfilehash: b7eac8337d6c8286e538bbe98b5ecbc13a448628
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072253"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="c7be8-103">automaticUpdateMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="c7be8-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="c7be8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c7be8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7be8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7be8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7be8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7be8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7be8-107">自動更新モードを使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="c7be8-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="c7be8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c7be8-108">Members</span></span>
|<span data-ttu-id="c7be8-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c7be8-109">Member</span></span>|<span data-ttu-id="c7be8-110">値</span><span class="sxs-lookup"><span data-stu-id="c7be8-110">Value</span></span>|<span data-ttu-id="c7be8-111">説明</span><span class="sxs-lookup"><span data-stu-id="c7be8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7be8-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="c7be8-112">userDefined</span></span>|<span data-ttu-id="c7be8-113">0</span><span class="sxs-lookup"><span data-stu-id="c7be8-113">0</span></span>|<span data-ttu-id="c7be8-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="c7be8-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c7be8-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="c7be8-115">notifyDownload</span></span>|<span data-ttu-id="c7be8-116">1</span><span class="sxs-lookup"><span data-stu-id="c7be8-116">1</span></span>|<span data-ttu-id="c7be8-117">ダウンロード時に通知します。</span><span class="sxs-lookup"><span data-stu-id="c7be8-117">Notify on download.</span></span>|
|<span data-ttu-id="c7be8-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c7be8-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="c7be8-119">2</span><span class="sxs-lookup"><span data-stu-id="c7be8-119">2</span></span>|<span data-ttu-id="c7be8-120">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="c7be8-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="c7be8-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c7be8-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="c7be8-122">3</span><span class="sxs-lookup"><span data-stu-id="c7be8-122">3</span></span>|<span data-ttu-id="c7be8-123">自動インストールおよびメンテナンス時に再起動します。</span><span class="sxs-lookup"><span data-stu-id="c7be8-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="c7be8-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="c7be8-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="c7be8-125">4</span><span class="sxs-lookup"><span data-stu-id="c7be8-125">4</span></span>|<span data-ttu-id="c7be8-126">自動インストールし、スケジュールされた時刻に再起動します。</span><span class="sxs-lookup"><span data-stu-id="c7be8-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="c7be8-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="c7be8-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="c7be8-128">5</span><span class="sxs-lookup"><span data-stu-id="c7be8-128">5</span></span>|<span data-ttu-id="c7be8-129">自動インストールし、エンドユーザーの制御に再起動します</span><span class="sxs-lookup"><span data-stu-id="c7be8-129">Auto-install and restart without end-user control</span></span>|





