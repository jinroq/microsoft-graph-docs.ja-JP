---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20aa217838848af6d85c023fd6587afe3427e82b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913269"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="5bf8a-103">automaticUpdateMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="5bf8a-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="5bf8a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5bf8a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bf8a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bf8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5bf8a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5bf8a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5bf8a-107">自動更新モードを使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="5bf8a-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="5bf8a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5bf8a-108">Members</span></span>
|<span data-ttu-id="5bf8a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5bf8a-109">Member</span></span>|<span data-ttu-id="5bf8a-110">値</span><span class="sxs-lookup"><span data-stu-id="5bf8a-110">Value</span></span>|<span data-ttu-id="5bf8a-111">説明</span><span class="sxs-lookup"><span data-stu-id="5bf8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bf8a-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="5bf8a-112">userDefined</span></span>|<span data-ttu-id="5bf8a-113">0</span><span class="sxs-lookup"><span data-stu-id="5bf8a-113">0</span></span>|<span data-ttu-id="5bf8a-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="5bf8a-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="5bf8a-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="5bf8a-115">notifyDownload</span></span>|<span data-ttu-id="5bf8a-116">1</span><span class="sxs-lookup"><span data-stu-id="5bf8a-116">1</span></span>|<span data-ttu-id="5bf8a-117">ダウンロード時に通知します。</span><span class="sxs-lookup"><span data-stu-id="5bf8a-117">Notify on download.</span></span>|
|<span data-ttu-id="5bf8a-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="5bf8a-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="5bf8a-119">2</span><span class="sxs-lookup"><span data-stu-id="5bf8a-119">2</span></span>|<span data-ttu-id="5bf8a-120">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="5bf8a-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="5bf8a-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="5bf8a-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="5bf8a-122">3</span><span class="sxs-lookup"><span data-stu-id="5bf8a-122">3</span></span>|<span data-ttu-id="5bf8a-123">自動インストールおよびメンテナンス時に再起動します。</span><span class="sxs-lookup"><span data-stu-id="5bf8a-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="5bf8a-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="5bf8a-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="5bf8a-125">4</span><span class="sxs-lookup"><span data-stu-id="5bf8a-125">4</span></span>|<span data-ttu-id="5bf8a-126">自動インストールし、スケジュールされた時刻に再起動します。</span><span class="sxs-lookup"><span data-stu-id="5bf8a-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="5bf8a-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="5bf8a-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="5bf8a-128">5</span><span class="sxs-lookup"><span data-stu-id="5bf8a-128">5</span></span>|<span data-ttu-id="5bf8a-129">自動インストールし、エンドユーザーの制御に再起動します</span><span class="sxs-lookup"><span data-stu-id="5bf8a-129">Auto-install and restart without end-user control</span></span>|





