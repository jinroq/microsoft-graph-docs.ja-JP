---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07a6b410289ea6455d0f6756efa7d1ec4d735ce4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849988"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="15cb7-103">automaticUpdateMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="15cb7-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="15cb7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15cb7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15cb7-105">自動更新モードを使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="15cb7-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="15cb7-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="15cb7-106">Members</span></span>
|<span data-ttu-id="15cb7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="15cb7-107">Member</span></span>|<span data-ttu-id="15cb7-108">値</span><span class="sxs-lookup"><span data-stu-id="15cb7-108">Value</span></span>|<span data-ttu-id="15cb7-109">説明</span><span class="sxs-lookup"><span data-stu-id="15cb7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15cb7-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="15cb7-110">userDefined</span></span>|<span data-ttu-id="15cb7-111">0</span><span class="sxs-lookup"><span data-stu-id="15cb7-111">0</span></span>|<span data-ttu-id="15cb7-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="15cb7-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="15cb7-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="15cb7-113">notifyDownload</span></span>|<span data-ttu-id="15cb7-114">1</span><span class="sxs-lookup"><span data-stu-id="15cb7-114">1</span></span>|<span data-ttu-id="15cb7-115">ダウンロード時に通知します。</span><span class="sxs-lookup"><span data-stu-id="15cb7-115">Notify on download.</span></span>|
|<span data-ttu-id="15cb7-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="15cb7-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="15cb7-117">2</span><span class="sxs-lookup"><span data-stu-id="15cb7-117">2</span></span>|<span data-ttu-id="15cb7-118">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="15cb7-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="15cb7-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="15cb7-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="15cb7-120">3</span><span class="sxs-lookup"><span data-stu-id="15cb7-120">3</span></span>|<span data-ttu-id="15cb7-121">自動インストールおよびメンテナンス時に再起動します。</span><span class="sxs-lookup"><span data-stu-id="15cb7-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="15cb7-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="15cb7-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="15cb7-123">4</span><span class="sxs-lookup"><span data-stu-id="15cb7-123">4</span></span>|<span data-ttu-id="15cb7-124">自動インストールし、スケジュールされた時刻に再起動します。</span><span class="sxs-lookup"><span data-stu-id="15cb7-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="15cb7-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="15cb7-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="15cb7-126">5</span><span class="sxs-lookup"><span data-stu-id="15cb7-126">5</span></span>|<span data-ttu-id="15cb7-127">自動インストールし、エンドユーザーの制御に再起動します</span><span class="sxs-lookup"><span data-stu-id="15cb7-127">Auto-install and restart without end-user control</span></span>|



