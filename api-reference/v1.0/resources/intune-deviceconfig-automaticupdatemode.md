---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
ms.openlocfilehash: c98927e1c1f66e3bf10fa07496aa54ac91bad20b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020659"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="61a0c-103">automaticUpdateMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="61a0c-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="61a0c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="61a0c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61a0c-105">自動更新モードを使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="61a0c-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="61a0c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="61a0c-106">Members</span></span>
|<span data-ttu-id="61a0c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="61a0c-107">Member</span></span>|<span data-ttu-id="61a0c-108">値</span><span class="sxs-lookup"><span data-stu-id="61a0c-108">Value</span></span>|<span data-ttu-id="61a0c-109">説明</span><span class="sxs-lookup"><span data-stu-id="61a0c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61a0c-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="61a0c-110">userDefined</span></span>|<span data-ttu-id="61a0c-111">0</span><span class="sxs-lookup"><span data-stu-id="61a0c-111">0</span></span>|<span data-ttu-id="61a0c-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="61a0c-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="61a0c-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="61a0c-113">notifyDownload</span></span>|<span data-ttu-id="61a0c-114">1</span><span class="sxs-lookup"><span data-stu-id="61a0c-114">1</span></span>|<span data-ttu-id="61a0c-115">ダウンロード時に通知します。</span><span class="sxs-lookup"><span data-stu-id="61a0c-115">Notify on download.</span></span>|
|<span data-ttu-id="61a0c-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="61a0c-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="61a0c-117">2</span><span class="sxs-lookup"><span data-stu-id="61a0c-117">2</span></span>|<span data-ttu-id="61a0c-118">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="61a0c-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="61a0c-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="61a0c-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="61a0c-120">3</span><span class="sxs-lookup"><span data-stu-id="61a0c-120">3</span></span>|<span data-ttu-id="61a0c-121">自動インストールおよびメンテナンス時に再起動します。</span><span class="sxs-lookup"><span data-stu-id="61a0c-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="61a0c-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="61a0c-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="61a0c-123">4</span><span class="sxs-lookup"><span data-stu-id="61a0c-123">4</span></span>|<span data-ttu-id="61a0c-124">自動インストールし、スケジュールされた時刻に再起動します。</span><span class="sxs-lookup"><span data-stu-id="61a0c-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="61a0c-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="61a0c-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="61a0c-126">5</span><span class="sxs-lookup"><span data-stu-id="61a0c-126">5</span></span>|<span data-ttu-id="61a0c-127">自動インストールし、エンドユーザーの制御に再起動します</span><span class="sxs-lookup"><span data-stu-id="61a0c-127">Auto-install and restart without end-user control</span></span>|



